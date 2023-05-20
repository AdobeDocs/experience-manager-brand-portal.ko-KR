---
title: Brand Portal에 동시 게시 문제 해결
seo-title: Troubleshoot issues in parallel publishing to Brand Portal
description: 병렬 게시 문제 해결
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

Brand Portal은 승인된 브랜드 자산을 Experience Manager Assets 작성자 인스턴스에서 원활하게 수집(또는 게시)하도록 Experience Manager Assets과 함께 구성됩니다. 한 번 [구성됨](../using/configure-aem-assets-with-brand-portal.md), Experience Manager 작성자는 복제 에이전트를 사용하여 Brand Portal 사용자가 승인된 사용을 위해 선택한 에셋을 Brand Portal cloud service로 복제합니다. 고속 병렬 게시를 허용하기 위해 Experience Manager 6.2 SP1-CFP5, Experience Manager CFP 6.3.0.2 이상에서 여러 복제 에이전트가 사용됩니다.

>[!NOTE]
>
>Adobe은 Experience Manager Assets Brand Portal이 Experience Manager Assets으로 성공적으로 구성되었는지 확인하려면 Experience Manager 6.4.1.0으로 업그레이드할 것을 권장합니다. Experience Manager 6.4의 제한으로 인해 Brand Portal으로 Experience Manager Assets을 구성하는 동안 오류가 발생하며 복제가 실패합니다.

Brand Portal에 대한 클라우드 서비스 구성 시 **[!UICONTROL /etc/cloudservice]**, 필요한 모든 사용자 및 토큰이 자동으로 생성되고 저장소에 저장됩니다. 클라우드 서비스 구성이 생성되며, 콘텐츠를 복제하기 위해 복제 및 복제 에이전트에 필요한 서비스 사용자도 생성됩니다. 4개의 복제 에이전트가 생성됩니다. 따라서 Experience Manager에서 Brand Portal으로 많은 자산을 게시하면 자산이 대기열에 추가되고 라운드 로빈을 통해 복제 에이전트 간에 분산됩니다.

그러나 대규모 슬링 작업, 네트워크 증가 및 **[!UICONTROL 디스크 I/O]** Experience Manager 작성자 인스턴스에서 또는 Experience Manager 작성자 인스턴스의 성능이 저하됩니다. 따라서 게시를 시작하기 전에 복제 에이전트와의 연결을 테스트하는 것이 좋습니다.

![](assets/test-connection.png)

## 최초 게시 오류 문제 해결: 게시 구성 확인 {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

게시 구성의 유효성을 검사하려면:

1. 오류 로그 확인
1. 복제 에이전트가 생성되었는지 확인
1. 연결 테스트

**Cloud Service을 만드는 동안 로그 추적**

테일 로그를 확인하십시오. 복제 에이전트가 생성되었는지 확인합니다. 복제 에이전트 만들기에 실패한 경우 클라우드 서비스에서 약간의 변경을 수행하여 클라우드 서비스를 편집합니다. 복제 에이전트가 생성되었는지 확인하고 다시 확인합니다. 그렇지 않으면 서비스를 다시 편집합니다.

클라우드 서비스를 반복적으로 편집할 때 제대로 구성되지 않으면 어린이집 티켓을 신고하십시오.

**복제 에이전트와의 연결 테스트**

복제 로그에 오류가 있는 경우 로그 보기:

1. 고객 지원 센터에 문의하십시오.

1. 다시 시도 [대청소](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) 게시 구성을 다시 만듭니다.

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

## 기존 Brand Portal 게시 구성 정리 {#clean-up-existing-config}

게시가 작동하지 않는 경우가 대부분인데 그 이유는 게시 중인 사용자(예: `mac-<tenantid>-replication` 은 최신 개인 키가 없으므로 &quot;401 unauthorized&quot; 오류와 함께 게시가 실패하고 복제 에이전트 로그에 다른 오류가 보고되지 않습니다. 문제 해결을 피하고 대신 구성을 만들 수 있습니다. 새 구성이 제대로 작동하려면 Experience Manager 작성자 설정에서 다음을 정리하십시오.

1. 다음으로 이동 `localhost:4502/crx/de/` (localhost에서 작성자 인스턴스를 실행 중인 것으로 간주합니다.:4502:\
   i. 삭제 `/etc/replication/agents.author/mp_replication`
아.. 삭제 
`/etc/cloudservices/mediaportal/<config_name>`

1. localhost:4502/useradmin으로 이동:\
   i. 사용자 검색 `mac-<tenantid>replication`
아.. 이 사용자 삭제

이제 시스템이 모두 정리되었습니다. 이제 클라우드 서비스 구성을 만들고 기존 JWT 애플리케이션을 계속 사용할 수 있습니다. 애플리케이션을 만들지 않고 새로 만든 클라우드 구성에서 공개 키를 업데이트할 수 있습니다.

>[!NOTE]
>
>자동 생성된 설정은 수정하지 마십시오.


## 개발자 연결 JWT 애플리케이션 테넌트 가시성 문제 {#developer-connection-jwt-application-tenant-visibility-issue}

켜진 경우 `https://legacy-oauth.cloud.adobe.io/`: 현재 사용자가 시스템 관리자를 보유하는 모든 조직(테넌트)이 나열됩니다. 여기에서 조직 이름을 찾을 수 없거나 여기에서 필요한 테넌트에 대한 애플리케이션을 만들 수 없는 경우 충분한(시스템 관리자) 권한이 있는지 확인하십시오.

이 사용자 인터페이스에는 테넌트의 경우 상위 10개 애플리케이션만 표시되는 알려진 문제가 있습니다. 응용 프로그램을 만들 때 해당 페이지에 계속 머무르면서 URL을 책갈피로 지정합니다. 애플리케이션의 목록 페이지로 이동하여 작성한 애플리케이션을 찾을 필요가 없습니다. 이 책갈피가 지정된 URL을 직접 히트하고 필요할 때마다 애플리케이션을 업데이트/삭제할 수 있습니다.

JWT 응용 프로그램이 적절하게 나열되지 않을 수 있습니다. 따라서 JWT 애플리케이션을 만드는 동안 URL을 참고/책갈피로 지정하는 것이 좋습니다.

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

Brand Portal에 게시하는 복제 에이전트가 게시 작업 처리를 중지하는 경우 복제 로그를 확인하십시오. Experience Manager은 기본적으로 자동 재시도 기능이 있으므로 특정 에셋 게시가 실패하면 자동으로 재시도됩니다. 네트워크 오류와 같은 간헐적인 문제가 있는 경우 다시 시도하는 동안 성공할 수 있습니다.

지속적인 게시 실패가 있고 큐가 차단된 경우 다음을 확인해야 합니다. **[!UICONTROL 연결 테스트]** 그리고 보고되고 있는 오류를 해결해 보세요.

오류를 기준으로 Brand Portal 엔지니어링 팀이 문제 해결에 도움을 줄 수 있도록 지원 티켓을 기록하는 것이 좋습니다.

## Brand Portal IMS 구성 토큰 만료됨 {#token-expired}

Brand Portal 환경이 갑자기 중지되면 IMS 구성이 제대로 작동하지 않을 수 있습니다. 시스템은 비정상 IMS 구성을 표시하고 액세스 토큰이 만료되었다는 오류 메시지(다음과 유사)를 반영합니다.

`com.adobe.granite.auth.oauth.AccessTokenProvider failed to get access token from authorization server status: 400 response: Unknown macro: {"error"}`

이 문제를 해결하려면 IMS 구성을 수동으로 저장 및 닫고 상태를 다시 확인하는 것이 좋습니다. 구성이 작동하지 않으면 기존 구성을 삭제하고 새 구성을 만듭니다.


## 연결 시간 초과 오류를 방지하기 위해 복제 에이전트 구성 {#connection-timeout}

일반적으로 복제 큐에 대기 중인 요청이 여러 개 있는 경우 시간 초과 오류와 함께 게시 작업이 실패합니다. 이 문제를 해결하려면 복제 에이전트가 시간 초과를 방지하도록 구성되었는지 확인합니다.

복제 에이전트를 구성하려면 다음을 수행합니다.

1. AEM Assets 작성자 인스턴스에 로그인합니다.
1. 다음에서 **도구** 패널, 다음으로 이동 **[!UICONTROL 배포]** > **[!UICONTROL 복제]**.
1. 복제 페이지에서 **[!UICONTROL 작성자의 에이전트]**&#x200B;를 클릭합니다. Brand Portal 테넌트의 4개 복제 에이전트를 볼 수 있습니다.
1. 복제 에이전트 URL을 클릭하고 **[!UICONTROL 편집]**.
1. 에이전트 설정에서 다음을 클릭합니다. **[!UICONTROL 확장됨]** 탭.
1. 다음 항목 선택 **[!UICONTROL 연결 닫기]** 확인란.
1. 4단계부터 7단계까지 반복하여 4개의 복제 에이전트를 모두 구성합니다.
1. 서버를 다시 시작합니다.
