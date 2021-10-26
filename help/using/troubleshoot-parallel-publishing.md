---
title: Brand Portal에 동시 게시 문제 해결
seo-title: Troubleshoot issues in parallel publishing to Brand Portal
description: 병렬 게시 문제 해결.
seo-description: Troubleshoot parallel publishing.
uuid: 51e45cca-8c96-4c69-84ef-2ef34f3bcde2
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: brand-portal
discoiquuid: a4801024-b509-4c51-afd8-e337417e658b
role: Admin
exl-id: 631beabc-b145-49ba-a8e4-f301497be6da
source-git-commit: 72cd0ebbf05067287d94e1dc4e1b68f5fb6c2888
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 3%

---

# Brand Portal에 동시 게시 문제 해결 {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Brand Portal은 Experience Manager Assets 작성자 인스턴스에서 원활하게 수집되거나 게시된 브랜드 자산을 승인하도록 Experience Manager Assets으로 구성됩니다. 한 번 [구성](../using/configure-aem-assets-with-brand-portal.md), Experience Manager 작성자 은 복제 에이전트를 사용하여 Brand Portal 사용자가 승인한 사용을 위해 선택한 자산을 Brand Portal 클라우드 서비스에 복제합니다. 여러 복제 에이전트가 Experience Manager 6.2 SP1-CFP5, Experience Manager CFP 6.3.0.2 및 이상에서 사용하여 고속 병렬 게시를 허용합니다.

>[!NOTE]
>
>Adobe은 Experience Manager Assets Brand Portal이 Experience Manager Assets으로 성공적으로 구성되었는지 확인하기 위해 Experience Manager 6.4.1.0으로 업그레이드할 것을 권장합니다. Experience Manager 6.4의 제한 사항으로 인해 Brand Portal 및 복제가 포함된 Experience Manager Assets을 구성할 때 오류가 발생합니다.

Brand Portal에 대한 클라우드 서비스 구성 **[!UICONTROL /etc/cloudservice]**&#x200B;필요한 모든 사용자와 토큰은 자동으로 생성되어 저장소에 저장됩니다. 클라우드 서비스 구성이 생성되면 복제 및 복제 에이전트가 컨텐츠를 복제하는 데 필요한 서비스 사용자도 생성됩니다. 4개의 복제 에이전트를 생성합니다. 따라서 Experience Manager에서 Brand Portal으로 많은 자산을 게시하면 자산이 라운드 로빈을 통해 복제 에이전트 간에 큐에 올라가 배포됩니다.

그러나 큰 슬링 작업, 네트워크 증가 및 **[!UICONTROL 디스크 I/O]** Experience Manager 작성자 인스턴스에서 선택하거나 Experience Manager 작성자 인스턴스의 성능을 낮춥니다. 따라서 게시를 시작하기 전에 복제 에이전트와의 연결을 테스트하는 것이 좋습니다.

![](assets/test-connection.png)

## 첫 번째 게시에서 오류 해결: 게시 구성 확인 {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

게시 구성을 확인하려면:

1. 오류 로그 확인
1. 복제 에이전트가 작성되었는지 확인
1. 연결 테스트

**Cloud Service을 만드는 동안 테일 로그**

테일 로그를 확인합니다. 복제 에이전트가 작성되었는지 확인합니다. 복제 에이전트를 만들지 못하면 클라우드 서비스를 약간 변경하여 클라우드 서비스를 편집합니다. 복제 에이전트가 생성되었는지 확인하고 다시 확인하십시오. 그렇지 않은 경우 서비스를 다시 편집합니다.

클라우드 서비스를 반복적으로 편집하는 경우 올바르게 구성되지 않으면 daycare 티켓을 보고합니다.

**복제 에이전트와의 연결 테스트**

복제 로그에 오류가 있는 경우 로그 보기:

1. 고객 지원에 문의하십시오.

1. 다시 시도 [정리](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) 게시 구성을 다시 만듭니다.

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

## 기존 Brand Portal 게시 구성 정리 {#clean-up-existing-config}

게시가 작동하지 않는 대부분의 경우 게시 중인 사용자(예: `mac-<tenantid>-replication` 에는 최신 개인 키가 없으므로 게시에 &quot;401 권한 없음&quot; 오류가 발생하고 복제 에이전트 로그에 다른 오류가 보고되지 않습니다. 문제를 해결하고 구성을 대신 만들지 않아도 됩니다. 새 구성이 제대로 작동하려면 Experience Manager 작성자 설정에서 다음 사항을 정리하십시오.

1. 이동 `localhost:4502/crx/de/` (localhost에서 작성자 인스턴스를 실행 중인 경우):4502:\
   나. delete `/etc/replication/agents.author/mp_replication`
ii. 삭제 
`/etc/cloudservices/mediaportal/<config_name>`

1. localhost:4502/useradmin으로 이동합니다.\
   나. 사용자 검색 `mac-<tenantid>replication`
ii. 이 사용자 삭제

이제 시스템이 모두 정리되었습니다. 이제 클라우드 서비스 구성을 만들고 기존 JWT 애플리케이션을 계속 사용할 수 있습니다. 새로 만든 클라우드 구성에서 공개 키를 업데이트하는 것이 아니라 애플리케이션을 만들 필요가 없습니다.

>[!NOTE]
>
>자동 생성된 설정은 수정하지 마십시오.


## Developer Connection JWT 애플리케이션 테넌트 가시성 문제 {#developer-connection-jwt-application-tenant-visibility-issue}

켜진 경우 `https://legacy-oauth.cloud.adobe.io/`에는 현재 사용자가 시스템 관리자를 보유하는 모든 조직(테넌트)이 나열됩니다. 여기에서 조직 이름을 찾을 수 없거나 여기에서 필수 테넌트에 대한 응용 프로그램을 만들 수 없는 경우 충분한(시스템 관리자) 권한이 있는지 확인하십시오.

이 사용자 인터페이스에서는 상위 10개의 애플리케이션만 표시되는 알려진 문제가 있습니다. 애플리케이션을 만들 때 해당 페이지에서 URL을 책갈피로 지정합니다. 애플리케이션의 목록 페이지로 이동하여 만든 응용 프로그램을 찾을 필요가 없습니다. 이 책갈피가 지정된 URL을 직접 누르고 필요할 때마다 애플리케이션을 업데이트/삭제할 수 있습니다.

JWT 애플리케이션이 적절하게 나열되지 않을 수 있습니다. 따라서 JWT 애플리케이션을 작성하는 동안 URL을 참고/책갈피로 지정하는 것이 좋습니다.

## 구성 실행 작동이 중지됩니다. {#running-configuration-stops-working}

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

Brand Portal에 게시하던 복제 에이전트가 게시 작업 처리를 중지하는 경우 복제 로그를 확인하십시오. Experience Manager에 자동 다시 시도 기본 기능이 있으므로 특정 자산 게시가 실패하면 자동으로 다시 시도됩니다. 네트워크 오류와 같은 일시적인 문제가 있을 경우 다시 시도하는 동안 성공할 수 있습니다.

지속적인 게시 오류가 있고 큐가 차단되는 경우 다음을 확인해야 합니다 **[!UICONTROL 연결 테스트]** 그리고 보고되고 있는 오류들을 해결하도록 노력하세요.

오류에 따라 Brand Portal 엔지니어링 팀이 문제를 해결하는 데 도움이 되도록 지원 티켓을 기록해야 합니다.

## Brand Portal IMS 구성 토큰이 만료되었습니다. {#token-expired}

Brand Portal 환경이 갑자기 중단되면 IMS 구성이 제대로 작동하지 않을 수 있습니다. 시스템은 비정상 IMS 구성을 표시하며 액세스 토큰이 만료된 오류 메시지(다음과 유사)를 반영합니다.

`com.adobe.granite.auth.oauth.AccessTokenProvider failed to get access token from authorization server status: 400 response: Unknown macro: {"error"}`

이 문제를 해결하려면 IMS 구성을 수동으로 저장 및 닫고 상태를 다시 확인하는 것이 좋습니다. 구성이 작동하지 않으면 기존 구성을 삭제하고 새 구성을 만드십시오.


## 연결 시간 제한 오류를 방지하도록 복제 에이전트를 구성합니다 {#connection-timeout}

일반적으로 복제 큐에 대기 중인 요청이 여러 개 있는 경우 게시 작업이 시간 초과 오류로 실패합니다. 이 문제를 해결하려면 복제 에이전트가 시간 제한을 방지하도록 구성되어 있는지 확인합니다.

복제 에이전트를 구성하려면:

1. AEM Assets 작성자 인스턴스에 로그인합니다.
1. 에서 **도구** 패널, 다음 위치로 이동 **[!UICONTROL 배포]** > **[!UICONTROL 복제]**.
1. 복제 페이지에서 **[!UICONTROL 작성자의 에이전트]**&#x200B;를 클릭합니다. Brand Portal 임차인의 4개의 복제 에이전트를 볼 수 있습니다.
1. 복제 에이전트 URL을 클릭하고 를 클릭합니다. **[!UICONTROL 편집]**.
1. 에이전트 설정에서 **[!UICONTROL 확장]** 탭.
1. 을(를) 선택합니다 **[!UICONTROL 연결 닫기]** 확인란을 선택합니다.
1. 4~7단계를 반복하여 4개의 복제 에이전트를 모두 구성합니다.
1. 서버를 다시 시작합니다.
