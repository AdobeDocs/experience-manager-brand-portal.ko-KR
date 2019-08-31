---
title: 브랜드 포털에 병렬 게시 문제 해결
seo-title: 브랜드 포털에 병렬 게시 문제 해결
description: 병렬 게시 문제 해결
seo-description: 병렬 게시 문제 해결
uuid: 51 e 45 cca -8 c 96-4 c 69-84 ef -2 ef 34 f 3 bcde 2
products: sg_ Experiencemanager/brand_ portal
content-type: 참조
topic-tags: 브랜드 포털
discoiquuid: A 4801024-B 509-4 C 51-AFD 8-E 337417 E 658 B
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 브랜드 포털에 병렬 게시 문제 해결 {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

브랜드 포털은 AEM Assets 와의 통합을 지원하여 AEM Assets 작성자 인스턴스에서 매끄러운 인제스트 (또는 퍼블리싱) 된 브랜드 에셋을 보유하게 합니다. [통합된](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html)AEM 작성자는 브랜드 포털 사용자가 승인된 사용을 위해 선택한 자산을 브랜드 포털 클라우드 서비스에 복제하기 위해 복제 에이전트를 사용합니다. AEM 6.2 SP 1-CFP 5], AEM CFP 6.3.0.2 및 이상 버전을 사용하여 고속 병렬 출판을 허용합니다.

>[!NOTE]
>
>AEM Assets 브랜드 포털이 AEM Assets와 성공적으로 통합되도록 AEM 6.4.1.0로 업그레이드하는 것이 좋습니다. AEM 6.4 에서는 브랜드 포털과의 통합을 구성하는 동안 오류가 발생하고 복제에 실패합니다.

/etc/cloudservice 아래의 [!UICONTROL 브랜드 포털에 대한 클라우드 서비스 구성에서]필요한 모든 사용자와 토큰은 자동으로 생성되어 보관소에 저장됩니다. 클라우드 서비스 구성이 만들어지면 복제 및 복제 에이전트에게 컨텐츠를 복제해야 하는 서비스 사용자가 생성됩니다. 이렇게 하면 네 개의 복제 에이전트가 만들어집니다. 따라서 AEM에서 브랜드 포털에 다양한 에셋을 게시할 때 이러한 에셋은 큐에 있는 Robin를 통해 이러한 복제 에이전트 간에 큐에 추가되고 배포됩니다.

그러나 큰 Sling 작업, AEM 작성자 인스턴스의 네트워크 및 [!UICONTROL 디스크 I/O] 증가, AEM 작성자 인스턴스의 성능 저하 등으로 인해 게시가 간헐적으로 실패할 수 있습니다. 따라서 게시를 시작하기 전에 복제 에이전트와의 연결을 테스트하도록 권장합니다.

![](assets/test-connection.png)

## 처음 게시 시 오류 문제 해결: 게시 구성 유효성 확인 {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

게시 구성을 확인하려면 다음을 수행하십시오.

1. 오류 로그 확인
2. 복제 에이전트가 작성되는지 여부 확인
3. 연결 테스트

**클라우드 서비스를 만드는 동안 테일 로그**

테일 로그를 확인합니다. 복제 에이전트가 만들어졌는지 여부를 확인합니다. 복제 에이전트 생성에 실패하는 경우 클라우드 서비스에서 사소한 변경을 수행하여 클라우드 서비스를 편집할 수 있습니다. 복제 에이전트가 만들어졌는지 여부를 확인하고 다시 확인합니다. 그렇지 않은 경우 서비스를 다시 편집합니다.

클라우드 서비스를 반복해서 편집하는 경우 제대로 구성되지 않은 경우 Daycare 티켓을 보고합니다.

**복제 에이전트와의 연결 테스트**

복제 로그에서 오류가 발견되는 경우 로그 보기:

1. Adobe 지원에 문의하십시오.

2. 정리를 다시 시도하고 [게시](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) 구성을 다시 만듭니다.

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

### 기존 브랜드 포털 게시 구성 정리 {#clean-up-existing-config}

게시가 작동하지 않는 대부분의 경우 다음과 같이 게시할 수 있습니다. [!UICONTROL mac-&lt; tenantid &gt;-replication]에 최신 개인 키가 없으므로, "401 권한 없는" 오류가 발생하고 다른 오류는 복제 에이전트 로그에 보고되지 않습니다. 문제를 해결하고 대신 새 구성을 만들 수 있습니다. 새 구성이 제대로 작동하려면 AEM 작성자 설정에서 다음을 정리합니다.

1. localhost로 [!UICONTROL 이동: 4502/crx/de] (localhost에서 [!UICONTROL 작성자 인스턴스를 실행하는 경우: 4502]):\
   i. 삭제 /etc/replication/agents.author/mp_replication *\
   ii. /etc/cloudservices/mediaportal/ &lt; config_ name &gt; 삭제

2. localhost로 [!UICONTROL 이동: 4502/Useradmin]:\
   사용자를 검색합니다 [! Uicontrol Mac-&lt; tenantid &gt;-Replication
II 이 사용자 삭제

이제 시스템이 모두 정리되어 있습니다. 이제 새로운 Cloudservice 구성을 만들어 https://legacy-oauth.cloud.adobe.io/에서 [기존의 JWT 애플리케이션을 계속 사용할](https://legacy-oauth.cloud.adobe.io/)수 있습니다. 새 애플리케이션을 만들 필요가 없습니다. 새로 만든 클라우드 구성에서 공개 키만 업데이트해야 합니다.

## Developer Connection JWT 애플리케이션 임차인 가시성 문제 {#developer-connection-jwt-application-tenant-visibility-issue}

[https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/)에서 현재 사용자가 시스템 관리자가 있는 모든 ORG (테넌트) 가 나열됩니다. 여기에서 조직 이름을 찾을 수 없거나 여기에서 필수 임차인에 대한 응용 프로그램을 만들 수 없는 경우, 충분한 (시스템 관리자) 권한이 있는지 확인하십시오.

이 사용자 인터페이스에는 최상위 10 개의 애플리케이션만 표시되도록 하는 알려진 문제가 있습니다. 애플리케이션을 만들 때 해당 페이지에 머무르고 URL를 책갈피에 추가합니다. 애플리케이션의 목록 페이지로 이동하여 만든 애플리케이션을 찾을 필요가 없습니다. 책갈피가 지정된 이 URL를 직접 히트하고 필요할 때마다 애플리케이션을 업데이트/삭제할 수 있습니다.

JWT 애플리케이션이 제대로 표시되지 않을 수 있습니다. 따라서 JWT 애플리케이션을 만드는 동안 URL를 메모하거나 책갈피에 추가하도록 권장됩니다.

## 실행 중인 구성 작동 중지 {#running-configuration-stops-working}

<!--
Comment Type: draft

<p>If the running configuration stops working, either of the following two possibilities
<g class="gr_ gr_15 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar multiReplace" data-gr-id="15" id="15" style="font-size: 12px;">
are
</g> there:</p>
<p>1.
<g class="gr_ gr_14 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="14" id="14">
Connection
</g> has failed, or</p>
<p>2. Publish has failed with permission to dam-replication-service denied, while connection has passed </p>
<p>If the connection has failed [1], the
<g class="gr_ gr_10 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling ins-del multiReplace" data-gr-id="10" id="10">
fail safe
</g> way to fix it is to <a href="../using/troubleshoot-parallel-publishing.md#main-pars-header-1664955658">clean up</a> the existing Brand Portal publish configuration and recreate a publish configuration. </p>
<p>However, if the
<g class="gr_ gr_18 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling" data-gr-id="18" id="18">
publish
</g> has failed with
<g class="gr_ gr_16 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="16" id="16">
permission
</g> denied to dam-replication-service, raise a support ticket.</p>
-->

브랜드 포털에 게시 중인 복제 에이전트가 게시 작업 처리를 중지하는 경우 복제 로그를 확인합니다. AEM 에는 자동 재시도가 내장되어 있으므로 특정 자산을 게시하지 못할 경우 자동으로 다시 검색됩니다. 네트워크 오류와 같은 간헐적인 문제가 있을 경우 재시도하는 동안 성공할 수 있습니다.

연속 게시 오류가 있고 대기열이 차단된 경우 **[!UICONTROL 테스트 연결을]** 확인하고 보고되는 오류를 해결하려고 합니다.

오류를 기준으로, 브랜드 포털 엔지니어링 팀이 문제를 해결하는 데 도움을 줄 수 있도록 지원 티켓을 로깅하는 것이 좋습니다.
