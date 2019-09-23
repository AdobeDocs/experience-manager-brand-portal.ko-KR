---
title: 브랜드 포털에 동시 게시 문제 해결
seo-title: 브랜드 포털에 동시 게시 문제 해결
description: 병렬 게시 문제를 해결합니다.
seo-description: 병렬 게시 문제를 해결합니다.
uuid: 51e45cca-8c96-4c69-84ef-2ef34f3bcde2
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: 참조
topic-tags: 브랜드 포털
discoiquuid: a4801024-b509-4c51-afd8-e37417e658b
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 브랜드 포털에 동시 게시 문제 해결 {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

브랜드 포털은 AEM Assets와의 통합을 지원하여 AEM Assets 작성자 인스턴스에서 원활하게 인제스트되거나 게시되도록 승인된 브랜드 자산을 지원합니다. 통합된 [](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html)AEM Author는 복제 에이전트를 사용하여 선택한 자산을 Brand Portal 클라우드 서비스에 복제하여 브랜드 포털 사용자의 승인을 받습니다. 여러 복제 에이전트가 AEM 6.2 SP1-CFP5], AEM CFP 6.3.0.2 및 이상 버전을 사용하여 고속 병렬 게시를 허용합니다.

>[!NOTE]
>
>AEM Assets 브랜드 포털이 AEM Assets와 성공적으로 통합되도록 AEM 6.4.1.0으로 업그레이드할 것을 권장합니다. AEM 6.4의 제한 사항은 브랜드 포털과의 통합을 구성하는 동안 오류가 발생하고 복제가 실패합니다.

브랜드 포털에 대한 클라우드 서비스를 구성할 때 [!UICONTROL /etc/cloudservice]아래에 필요한 모든 사용자 및 토큰이 자동으로 생성되고 보관소에 저장됩니다. 클라우드 서비스 구성이 생성되며, 복제 에이전트와 복제 에이전트가 컨텐츠를 복제하는 데 필요한 서비스 사용자도 생성됩니다. 이렇게 하면 4개의 복제 에이전트가 만들어집니다. 따라서 AEM에서 브랜드 포털에 많은 자산을 게시하면 이러한 자산은 라운드 로빈을 통해 이러한 복제 에이전트 간에 큐에 올라가 배포됩니다.

그러나 AEM 작성자 인스턴스에서 네트워크 및 디스크 입출력이 증가하거나 AEM 작성자 [!UICONTROL 인스턴스의 성능이 저하되어] 간헐적으로 게시할 수 없습니다. 따라서 게시를 시작하기 전에 복제 에이전트와의 연결을 테스트하는 것이 좋습니다.

![](assets/test-connection.png)

## 처음 게시할 때의 오류 문제 해결:게시 구성 유효성 확인 {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

게시 구성의 유효성을 확인하려면:

1. 오류 로그 확인
2. 복제 에이전트가 생성되었는지 확인
3. 연결 테스트

**클라우드 서비스를 만드는 동안 세부 로그**

꼬리 로그를 확인하십시오. 복제 에이전트가 생성되었는지 확인합니다. 복제 에이전트 만들기에 실패하는 경우 클라우드 서비스에서 일부를 변경하여 클라우드 서비스를 편집합니다. 복제 에이전트가 생성되었는지 확인하고 다시 확인합니다. 그렇지 않은 경우 서비스를 다시 편집합니다.

클라우드 서비스를 반복적으로 편집하는 경우 제대로 구성되지 않은 경우 탁아소를 보고합니다.

**복제 에이전트와의 연결 테스트**

복제 로그에 오류가 있는 경우 로그 보기:

1. Adobe 지원에 문의하십시오.

2. 다시 [정리하여](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) 게시 구성을 다시 만듭니다.

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

### 기존 브랜드 포털 게시 구성 정리 {#clean-up-existing-config}

게시 작업이 작동하지 않는 대부분의 경우 게시 중인 사용자가 원인일 수 있습니다(예: [!UICONTROL mac-&lt;tenantid&gt;-replication])에 최신 개인 키가 없으므로 "401 권한 없음" 오류가 발생하여 게시가 실패하고 다른 오류가 복제 에이전트 로그에 보고되지 않습니다. 문제를 해결하고 새 구성을 만들지 않으려는 경우가 있습니다. 새 구성이 제대로 작동하려면 AEM 작성자 설정에서 다음을 정리하십시오.

1. localhost: [!UICONTROL 4502/crx/de] ( [!UICONTROL localhost:4502에서 작성자 인스턴스를 실행 중임을 고려]):\
   i./etc/replication/agents.author/mp_replication* 삭제\
   ii. delete /etc/cloudservices/mediaportal/&lt;config_name&gt;

2. localhost: [!UICONTROL 4502/useradmin으로 이동합니다].\
   i search for user [!UICONTROL mac-&lt;tenantid&gt;-replicationii delete this user

이제 시스템이 모두 깨끗해졌습니다. 이제 새 cloudservice 구성을 만들고 https://legacy-oauth.cloud.adobe.io/에서 기존의 JWT 애플리케이션을 계속 사용할 수 [있습니다](https://legacy-oauth.cloud.adobe.io/). 새 애플리케이션을 만들 필요가 없으며 새로 만든 클라우드 구성에서 공개 키만 업데이트해야 합니다.

## 개발자 연결 JWT 응용 프로그램 테넌트 가시성 문제 {#developer-connection-jwt-application-tenant-visibility-issue}

https://legacy-oauth.cloud.adobe.io/ [에서](https://legacy-oauth.cloud.adobe.io/)현재 사용자가 시스템 관리자를 보유하고 있는 모든 조직(테넌트)이 나열됩니다. 여기에서 조직 이름을 찾을 수 없거나 여기에서 필수 테넌트에 대한 응용 프로그램을 만들 수 없는 경우 충분한(시스템 관리자) 권한이 있는지 확인하십시오.

이 사용자 인터페이스에 대해 상위 10개 애플리케이션만 볼 수 있는 알려진 문제가 하나 있습니다. 애플리케이션을 만들 때 해당 페이지에서 URL을 책갈피로 지정합니다. 애플리케이션의 목록 페이지로 이동하여 만든 애플리케이션을 찾을 필요가 없습니다. 이 책갈피가 지정된 URL을 직접 히트하고 필요할 때마다 애플리케이션을 업데이트/삭제할 수 있습니다.

JWT 애플리케이션이 적절하게 나열되지 않을 수 있습니다. 따라서 JWT 애플리케이션을 생성하는 동안 URL을 메모하거나 책갈피를 지정하는 것이 좋습니다.

## 구성 실행이 중지됩니다. {#running-configuration-stops-working}

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

브랜드 포털에 게시하던 복제 에이전트가 게시 작업 처리를 중지하면 복제 로그를 확인하십시오. AEM에는 자동 재시도가 내장되어 있으므로 특정 자산 게시에 실패하는 경우 자동으로 재시도됩니다. 네트워크 오류와 같은 간헐적인 문제가 있는 경우 다시 시도하는 동안 성공할 수 있습니다.

연속 게시 오류가 발생하여 큐가 차단된 경우 **[!UICONTROL 테스트 연결을]** 확인하고 보고되는 오류를 해결하려고 해야 합니다.

오류에 따라 Brand Portal 엔지니어링 팀이 문제를 해결하는 데 도움이 되도록 지원 티켓을 기록하는 것이 좋습니다.
