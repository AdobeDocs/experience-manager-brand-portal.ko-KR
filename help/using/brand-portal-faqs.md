---
title: FAQ
seo-title: null
description: Adobe Experience Manager Assets Brand Portal에서 자주 묻는 질문에 대한 통찰력을 얻으십시오.
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 1%

---

# FAQ {#frequently-asked-questions}

Brand Portal FAQ는 최종 사용자 쿼리와 최신 Experience Manager Assets Brand Portal 6.4.6 릴리스 또는 이전 버전을 사용하는 동안 발생할 수 있는 문제에 중점을 둡니다.


## Brand Portal 6.4.6 FAQ  {#faqs-bp646}

**골동품. 기존 레거시 OAuth 끝점(`https://legacy-oauth.cloud.adobe.io/login`)이(가) 작동하지 않습니다. 무엇이 가능한 이유가 될 수 있을까?**

**Ans.** 이전 OAuth 구성은 더 이상 사용되지 않습니다. Experience Manager Assets 작성자 인스턴스를 최신 서비스 팩으로 업그레이드하고 Adobe Developer 콘솔을 통해 구성해야 합니다. 자세한 내용은 [Brand Portal에서 Experience Manager Assets 구성](configure-aem-assets-with-brand-portal.md)을 참조하십시오. 그러나 업그레이드 전까지 이전 OAuth 구성이 작동하려면 이전 OAuth 끝점을 로 업데이트하십시오. `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**골동품. Adobe Developer 콘솔로 업그레이드한 후 Brand Portal에서 Experience Manager Assets으로 기여 폴더의 자산을 게시할 수 없습니다. 내 작성자 인스턴스는 Experience Manager Assets 6.5.4에 있습니다. 무엇이 가능한 이유가 될 수 있을까?**

**Ans.** 예. 기여도 폴더의 자산을 Adobe Developer 콘솔을 통해 Experience Manager Assets 6.5.4에 게시하는 동안 알려진 문제가 있습니다.

이 문제는 Experience Manager Assets 6.5.5에서 해결되었습니다. Experience Manager Assets 인스턴스를 최신 서비스 팩으로 업그레이드하고 [구성 업그레이드](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) Adobe Developer 콘솔에서 게시할 수 있습니다.

<!--
Broken link of download hotfix, comment out this section until we have the latest URL.

For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your AEM author instance.
-->

**골동품. Experience Manager Assets의 Brand Portal에서 게시된 기여 폴더의 컨텐츠가 표시되지 않습니다. 무엇이 가능한 이유가 될 수 있을까?**

**Ans.** Experience Manager Assets 관리자에게 문의하여 구성을 확인하고 Brand Portal 테넌트가 Experience Manager Assets 작성자 인스턴스를 하나만 사용하여 구성되었는지 확인하십시오.

이 문제는 여러 Experience Manager Assets 작성자 인스턴스에 Brand Portal 테넌트를 구성한 경우 발생할 수 있습니다. 예를 들어 관리자는 스테이징 및 프로덕션 환경의 Experience Manager Assets 작성자 인스턴스에서 동일한 Brand Portal 테넌트를 구성합니다. 이 경우 에셋 게시는 Brand Portal에서 트리거되지만 Experience Manager Assets 작성자 인스턴스는 복제 에이전트가 요청 토큰을 받지 않는 에셋 코드를 가져올 수 없습니다.


**골동품. Experience Manager Assets에서 Brand Portal으로 자산을 게시할 수 없습니다. 복제 로그 상태는 연결 시간이 초과되었음을 나타냅니다. 빠른 해결 방법이 있습니까?**

**Ans.** 일반적으로 복제 큐에 보류 중인 요청이 여러 개 있는 경우 시간 초과 오류와 함께 게시가 실패합니다. 이 문제를 해결하려면 복제 에이전트가 시간 초과를 방지하도록 구성되었는지 확인합니다.

복제 에이전트를 구성하려면 다음 단계를 수행하십시오.

1. Experience Manager Assets 작성자 인스턴스에 로그인합니다.
1. 다음에서 **도구** 패널, 다음으로 이동 **[!UICONTROL 배포]** > **[!UICONTROL 복제]**.
1. 복제 페이지에서 **[!UICONTROL 작성자의 에이전트]**&#x200B;를 클릭합니다. Brand Portal 테넌트에 대한 4개의 복제 에이전트를 볼 수 있습니다.
1. 복제 에이전트 URL을 클릭하여 에이전트 세부 정보를 엽니다.
1. 클릭 **[!UICONTROL 편집]** 복제 에이전트 설정을 수정합니다.
1. 에이전트 설정에서 다음을 클릭합니다. **[!UICONTROL 확장됨]** 탭.
1. 다음 항목 선택 **[!UICONTROL 연결 닫기]** 확인란.
1. 4단계부터 7단계까지 반복하여 4개의 복제 에이전트를 모두 구성합니다.
1. 서버를 다시 시작하고 연결을 확인합니다.


## Brand Portal 6.4.5 FAQ  {#faqs-bp645}

**골동품. Brand Portal 6.4.5 릴리스의 주요 변경 사항은 무엇입니까?**

**Ans.** Experience Manager Assets Brand Portal 6.4.5는 Brand Portal 사용자가 관리자 권한 없이 Brand Portal 인스턴스 내에서 콘텐츠를 업로드하고 기여도 폴더를 다시 Experience Manager Assets에 게시할 수 있는 기능 릴리스입니다.
자세한 내용은 [Brand Portal의 에셋 소싱](brand-portal-asset-sourcing.md).



**골동품. 기존 에셋, 기능 또는 내가 만든 구성에 대한 액세스 권한을 잃게 됩니까?**

**Ans.** 모든 기존 기능과 구성이 그대로 유지됩니다. 최종 사용자는 영향을 받지 않으며 콘텐츠는 그대로 유지됩니다.



**골동품. 언제 Brand Portal의 새 버전으로 이동합니까?**

**Ans.** Brand Portal 6.4.5는 2019년 10월에 프로덕션에 출시되었습니다. 그리고 다음 Brand Portal 버전은 2020년 3분기에 출시될 예정입니다.
업데이트 및 버전 변경의 경우 [릴리스 정보](brand-portal-release-notes.md) 및 [Brand Portal의 새로운 기능](whats-new.md).



**골동품. 내 사용자가 영향을 받습니까?**

**Ans.** Brand Portal 6.4.5 릴리스는 전적으로 Brand Portal 내에 있으므로 최종 사용자에게 영향을 주지 않습니다.



**골동품. Brand Portal 사용자로서 내 작업에 필요한 작업이 있습니까?**

**Ans.** Brand Portal 6.4.5 릴리스에는 Asset Sourcing이라는 새로운 기능이 포함되어 있습니다. 관리자는 Experience Manager Assets 사용자가 이 기능을 사용할 수 있도록 Brand Portal에서 에셋 소싱 기능을 구성해야 합니다. 자세한 내용은 다음을 참조하십시오. [자산 소싱 활성화](brand-portal-asset-sourcing.md).



**골동품. 기여도 폴더를 만들 수 있는 사용자는 누구입니까?**

**Ans.** Experience Manager Assets에서 새 폴더를 만들 수 있는 권한이 있는 모든 Experience Manager Assets 사용자는 **기여도** 폴더를 삭제합니다. 을(를) 만들려면 **기여도** 폴더, 유형의 새 폴더 만들기 **자산 기여**.
이 폴더는 기여를 위해 활성 Brand Portal 사용자와 공유됩니다.



**골동품. 기여 폴더에는 어떤 항목이 포함되어 있습니까?**

**Ans.** **기여도** 폴더에는 두 개의 하위 폴더가 있습니다. **새로 만들기** 및 **공유됨**. 처음에는 NEW 폴더가 비어 있고 SHARED 폴더에 Brand Portal 사용자에 대한 참조 콘텐츠(재사용 가능한 에셋)가 포함되어 있습니다.
Brand Portal 사용자는 **기여도** 폴더에 있는 컨텐츠 폴더 및 업로드 **새로 만들기** 폴더를 삭제합니다.



**골동품.  기존 기여도 폴더의 이름을 수정할 수 있습니까?**

**Ans.** **아니요**&#x200B;기존 의 이름은 수정할 수 없습니다 **기여도** 폴더를 삭제합니다.



**골동품. 자산 요구 사항 w.r.t. 기여도는 무엇입니까?**

**Ans.** 다음 **개요** 문서에 첨부된 문서 **기여도** 폴더에 업로드된 폴더 및 참조 콘텐츠(재사용 가능한 에셋) **공유됨** 폴더는 Brand Portal 사용자가 기여자로서의 기여와 기대의 필요성을 이해할 수 있도록 도와주며, 이를 통칭하여 에셋 요구 사항이라고 합니다.



**골동품. 허용된 폴더에 에셋을 업로드할 수 있습니까?**

**Ans.** 허용된 폴더 중 일부만 사용할 수 있습니다. Brand Portal 사용자는 콘텐츠만 업로드할 수 있습니다. **기여도** Experience Manager Assets 또는 Brand Portal 관리자가 공유하는 폴더입니다.



**골동품. 기여도 폴더에 액세스하려면 어떻게 합니까?**

**Ans.** 다음에 액세스할 수 있습니다. **기여도** 폴더는 사용자와 공유된 경우에만 표시합니다. 기여도 폴더가 공유될 때마다 이메일/펄스 알림을 받게 됩니다. 이메일에 공유된 링크를 통해 기여도 폴더에 액세스하거나 Brand Portal 인스턴스에 로그인하고 벨 아이콘으로 이동하여 기여도 폴더에 액세스할 수 있습니다.

>[!NOTE]
>
>기존 Brand Portal 사용자가 아닌 경우 Experience Manager Assets 관리자에게 Admin Console에서 사용자를 만들고 Brand Portal 사용자 목록의 사용자 구성 파일에 프로필을 추가하도록 요청하십시오.

**골동품. 사용자 가져오기에 대한 CSV 파일의 형식은 무엇입니까?**

**Ans.** 형식은 대량 사용자 가져오기에 대해 Admin Console이 지원하는 것과 같습니다. 이메일, 이름 및 성은 필수입니다.



**골동품. 자산 기여 사용자 드롭다운에서 사용자(Brand Portal 기여자) 목록을 채우는 것은 무엇입니까?**

**Ans.** 드롭다운의 사용자는 Experience Manager Assets에 업로드된 Brand Portal 사용자 구성(.csv) 파일에서 채워집니다.



**골동품. 가져오기 및 게시 작업의 상태는 어디에서 볼 수 있습니까?**

**Ans.** Experience Manager Assets에서 가져오기의 상태를 확인할 수 있습니다. **비동기** 작업 페이지입니다. Brand Portal에서 게시 작업의 상태를 볼 수 있습니다. **[!UICONTROL 도구 > 자산 기여 상태]**.



**골동품. Experience Manager 시 정기적으로 실행되는 가져오기 작업의 빈도는 얼마입니까?**

**Ans.** Experience Manager Assets에서 폴링은 5분마다 실행됩니다.



**골동품. Brand Portal에서 Experience Manager Assets으로 폴더를 게시할 수 있는 횟수에 대한 임계값이 있습니까?**

**Ans.** 아니요, 의 모든 자산입니다. **새로 만들기** 폴더는 이전에 게시된 사실과 관계없이 Experience Manager Assets에 게시됩니다. 항상 **기여도** 폴더가 Brand Portal에서 Experience Manager Assets으로 게시되며, 의 콘텐츠를 무시합니다. **새로 만들기** 폴더를 삭제합니다.



**골동품. 기여 폴더에 새 에셋을 업로드하는 방법**

**Ans.** 다음에 대한 자세한 설명서를 참조하십시오. [기여 폴더에 자산 업로드 중](brand-portal-publish-contribution-folder-to-brand-portal.md).



**골동품. Brand Portal 사용자가 NEW 폴더에 업로드한 자산에 대한 썸네일/미리보기가 표시되지 않습니까?**

**Ans.** 설계된 대로 Brand Portal 끝에서는 실행 중인 워크플로우가 없습니다.



**골동품. 유동적인 Experience Manager Assets에서 Brand Portal으로 폴더를 게시하면 어떻게 됩니까?**

**Ans.** Experience Manager Assets에서는 폴더가 Brand Portal에 게시될 때마다 로그가 유지됩니다. 게시 시 Brand Portal에 게시되지 않은 모든 자산은 복제 큐에 저장됩니다. 게시 작업이 트리거된 후 폴더에 추가된 모든 자산은 Brand Portal에 게시되지 않습니다. Experience Manager Assets 사용자가 폴더를 다시 게시하면 이전에 게시되지 않은 자산(복제 큐에 있음)만 Brand Portal에 게시됩니다.
Experience Manager Assets에서 Brand Portal으로 게시된 모든 폴더와 기여도 폴더 내의 공유 폴더에 대해 적용됩니다.

**골동품. 누구에게 문의해야 합니까?**

**Ans.** Adobe 계정 관리자 또는 고객 지원 센터에 문의하십시오.

>[!NOTE]
>
>릴리스 일정은 잠정적이며 변경될 수 있습니다. 업데이트된 릴리스 일정을 얻으려면 Adobe 계정 관리자 또는 고객 지원 센터에 문의하십시오.


## 제품 액세스 및 지원(제한된 사이트) {#product-access-and-support-restricted-sites}

이러한 사이트는 고객만 사용할 수 있습니다. 고객이고 액세스 권한이 필요한 경우 Adobe 계정 관리자에게 문의하십시오.

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Support]()
-->
