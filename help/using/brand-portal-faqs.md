---
title: FAQ
seo-title: null
description: Adobe Experience Manager Assets 브랜드 포털에서 자주 묻는 질문에 대한 통찰력을 얻을 수 있습니다.
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 2f6ec4ac56390b2243e1d1a2c2adb34eb9aad7b2
workflow-type: tm+mt
source-wordcount: '1521'
ht-degree: 3%

---


# FAQ {#frequently-asked-questions}

브랜드 포털 FAQ는 최신 AEM Assets Brand Portal 6.4.6 릴리스 또는 이전 버전으로 작업하는 동안 발생할 수 있는 최종 사용자 쿼리 및 문제에 중점을 둡니다.


## 브랜드 포털 6.4.6 FAQ {#faqs-bp646}

**방문자 수 기존 레거시 OAuth 끝점(`https://legacy-oauth.cloud.adobe.io/login`)이 작동하지 않습니다. 가능한 이유가 무엇입니까?**

**Ans.** 레거시 OAuth 구성은 더 이상 사용되지 않습니다. AEM Assets 작성자 인스턴스를 최신 서비스 팩으로 업그레이드하고 Adobe 개발자 콘솔을 통해 구성해야 합니다. 자세한 내용은 [Brand Portal에서 AEM Assets 구성](configure-aem-assets-with-brand-portal.md)을 참조하십시오. 그러나 업그레이드할 때까지 기존 OAuth 구성이 작동하려면 기존 OAuth 끝점을 `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`으로 업데이트하십시오.

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**방문자 수 Adobe 개발자 콘솔로 업그레이드한 후 기여도 폴더의 자산을 브랜드 포털에서 AEM Assets으로 게시할 수 없습니다. 작성자 인스턴스가 AEM 6.5.4에 있습니다. 가능한 이유는 무엇입니까?**

**Ans.** 예. Adobe 개발자 콘솔을 통해 AEM 6.5.4의 AEM Assets에 기여도 폴더의 에셋을 게시하는 동안 알려진 문제가 있습니다.

AEM 6.5.5에서 문제가 해결되었습니다. AEM Assets 인스턴스를 최신 서비스 팩 AEM으로 업그레이드하고 Adobe 개발자 콘솔에서 [구성을 업그레이드 할 수 있습니다.](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65)

AEM 6.5.4에 대한 즉각적인 픽스를 위해서는 [핫픽스](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041)를 다운로드하고 AEM 작성자 인스턴스에 설치하는 것이 좋습니다.

**방문자 수 AEM Assets의 브랜드 포털에서 게시한 기여도 폴더의 콘텐츠가 표시되지 않습니다. 가능한 이유가 무엇입니까?**

**Ans.** 구성을 확인하고 브랜드 포털 테넌트가 하나의 AEM Assets 작성자 인스턴스로만 구성되어 있는지 확인하려면 AEM Assets 관리자에게 문의하십시오.

이 문제는 여러 AEM Assets 작성자 인스턴스에서 브랜드 포털 테넌트를 구성한 경우에 발생할 수 있습니다. 예를 들어, 관리자는 스테이징 및 프로덕션 환경의 AEM Assets 작성자 인스턴스에 동일한 브랜드 포털 테넌트를 구성합니다. 이 경우 자산 게시는 브랜드 포털에서 트리거되지만 AEM Assets 작성자 인스턴스는 요청한 토큰을 받지 못하는 에셋 코드를 가져올 수 없습니다.


**방문자 수 AEM Assets에서 브랜드 포털에 자산을 게시할 수 없습니다. 복제 로그는 연결 시간이 초과되었음을 나타냅니다. 빠른 수정이 있습니까?**

**Ans.** 일반적으로 복제 대기열에 보류 중인 요청이 여러 개 있을 경우 게시 실패 시간 초과 오류가 발생합니다. 이 문제를 해결하려면 시간 초과를 방지하도록 복제 에이전트가 구성되어 있는지 확인하십시오.

복제 에이전트를 구성하려면 다음 단계를 수행하십시오.
1. AEM Assets 작성자 인스턴스에 로그인합니다.
1. **도구** 패널에서 **[!UICONTROL 배포]** > **[!UICONTROL 복제]**&#x200B;로 이동합니다.
1. 복제 페이지에서 **[!UICONTROL 작성자의 에이전트]**&#x200B;를 클릭합니다. 브랜드 포털 테넌트에 대한 4개의 복제 에이전트를 볼 수 있습니다.
1. 복제 에이전트 URL을 클릭하여 에이전트 세부 정보를 엽니다.
1. 복제 에이전트 설정을 수정하려면 **[!UICONTROL 편집]**&#x200B;을 클릭합니다.
1. [에이전트 설정]에서 **[!UICONTROL 확장]** 탭을 클릭합니다.
1. **[!UICONTROL 연결 닫기]** 확인란을 선택합니다.
1. 4-7단계를 반복하여 4개의 복제 에이전트를 모두 구성합니다.
1. 서버를 다시 시작하고 연결을 확인합니다.


## 브랜드 포털 6.4.5 FAQ {#faqs-bp645}

**방문자 수 브랜드 포털 6.4.5 릴리스의 주요 변경 사항은 무엇입니까?**

**Ans.** AEM Assets Brand Portal 6.4.5은 브랜드 포털 사용자가 관리자 권한 없이 브랜드 포털 인스턴스 내에서 콘텐츠를 업로드하고 기여도 폴더를 AEM Assets에 다시 게시할 수 있는 기능 릴리스입니다.
자세한 내용은 브랜드 포털의 [자산 소싱](brand-portal-asset-sourcing.md)을 참조하십시오.



**방문자 수 내가 만든 기존 자산, 기능 또는 구성에 대한 액세스 권한을 잃게 됩니까?**

**Ans.** 기존의 모든 기능과 구성은 그대로 유지됩니다. 최종 사용자는 영향을 받지 않으며 내용은 그대로 유지됩니다.



**방문자 수 새로운 버전의 브랜드 포털로 언제 이동합니까?**

**Ans.** 브랜드 포털 6.4.5은 2019년 10월 제작에 출시되었습니다. 다음 브랜드 포털 버전은 2020년 3분기에 출시될 예정입니다.
업데이트 및 버전 변경의 경우 [릴리스 노트](brand-portal-release-notes.md) 및 [브랜드 포털의 새로운 기능](whats-new.md)을 추적하는 것이 좋습니다.



**방문자 수 내 사용자에게 영향을 줍니까?**

**Ans.** 브랜드 포털 6.4.5 릴리스는 브랜드 포털 내에서만 제공되므로 최종 사용자에게는 영향을 주지 않습니다.



**방문자 수 브랜드 포털 사용자로서의 작업에 필요한 작업이 있습니까?**

**Ans.** 브랜드 포털 6.4.5 릴리스에는 자산 소싱이라는 새로운 기능이 포함되어 있습니다. AEM 관리자는 브랜드 포털 사용자에 대한 기능을 활성화하려면 AEM Assets에서 자산 소싱 기능을 구성해야 합니다. 자세한 내용은 [자산 소싱 활성화](brand-portal-configure-asset-sourcing.md)를 참조하십시오.



**방문자 수 누가 기여도 폴더를 만들 수 있습니까?**

**Ans.** AEM Assets에서 새 폴더를 만들 권한이 있는 모든 AEM 사용자는 Contribute 폴더를 만들 수  **** 있습니다. **기여도** 폴더를 만들려면 **자산 기여도** 유형의 새 폴더를 만듭니다.
이 폴더는 기여도를 위해 활성 브랜드 포털 사용자와 공유됩니다.



**방문자 수 기여도 폴더에 포함된 항목:**

**Ans.** **Contribute** 폴더에는 2개의 하위 폴더  **** NEW 및 SHARED **가 있습니다**. 처음에는 NEW 폴더가 비어 있고 SHARED 폴더에는 Brand Portal 사용자에 대한 참조 콘텐츠(재사용 가능한 자산)가 포함됩니다.
브랜드 포털 사용자는 **기여도** 폴더에 액세스하고 **NEW** 폴더에 콘텐트를 업로드합니다.



**방문자 수  기존 기여도 폴더의 이름을 수정할 수 있습니까?**

**Ans.** **아니요**, 기존 Contribute 폴더의 이름은 수정할 수  **** 없습니다.



**방문자 수 RR.t 기여도를 포함한 자산 요구 사항은 무엇입니까?**

**Ans.** 기여도  **** 폴더에 첨부된  **** 서류 및  **** SHAREDfolder에 업로드된 참조 컨텐츠(재사용 가능한 자산)는 브랜드 포털 사용자가 기여도와 기대치를 기여자로 이해하는 데 도움이 되며, 통칭하여 자산 요구 사항이라고 합니다.



**방문자 수 에셋을 허용된 폴더에 업로드할 수 있습니까?**

**Ans.** 일부 폴더가 허용된 것은 아닙니다. 브랜드 포털 사용자는 AEM 또는 브랜드 포털 관리자가 공유하는 **기여도** 폴더에만 컨텐츠를 업로드할 수 있습니다.



**방문자 수 기여도 폴더에 액세스하려면 어떻게 합니까?**

**Ans.** Contribute 폴더는 사용자와 공유된  **** 경우에만 액세스할 수 있습니다. 기여도 폴더가 사용자와 공유될 때마다 이메일/펄스 알림을 받게 됩니다. 이메일에 공유된 링크를 통해 기여도 폴더에 액세스하거나, 브랜드 포털 인스턴스에 로그인하고, 게시물 폴더에 액세스할 수 있는 알림을 위해 벨 아이콘으로 이동할 수 있습니다.

>[!NOTE]
>
>기존 브랜드 포털 사용자가 아닌 경우 AEM 관리자에게 AEM 관리 콘솔에서 사용자를 만들고 Brand Portal 사용자 목록의 사용자 구성 파일에 프로필을 추가하도록 요청하십시오. [브랜드 포털 사용자 ](brand-portal-configure-asset-sourcing.md) 추가를 참조하십시오.

**방문자 수 사용자 가져오기에 대한 CSV 파일의 형식은 무엇입니까?**

**Ans.** 형식은 대량 사용자 가져오기에 대해 Admin Console에서 지원하는 형식과 동일합니다. 이메일, 이름 및 성은 필수입니다.



**방문자 수 자산 기여도 사용자 드롭다운에서 사용자 목록(브랜드 포털 기여자)은 어떻게 됩니까?**

**Ans.** 드롭다운의 사용자는 AEM에 업로드된 브랜드 포털 사용자 구성(.csv) 파일에서 채워집니다.



**방문자 수 가져오기 및 게시 작업의 상태는 어디에서 볼 수 있습니까?**

**Ans.** AEM에서는 비동기 작업 페이지에서 가져오기 상태를 볼 수  **** 있습니다. 브랜드 포털에서는 **[!UICONTROL 도구 > 자산 기여도 상태]**&#x200B;에서 게시 작업의 상태를 볼 수 있습니다.



**방문자 수 AEM에서 정기적으로 실행되는 가져오기 작업의 빈도는 무엇입니까?**

**Ans.** AEM에서는 5분마다 여론 조사가 실시됩니다.



**방문자 수 브랜드 포털에서 AEM Assets으로 폴더를 게시할 수 있는 횟수에 대한 경고가 있습니까?**

**Ans.** 아니요. NEWfolder에 있는 모든  **** 에셋은 이전에 게시되었는지에 관계없이 AEM Assets에 게시됩니다. **기여도** 폴더가 브랜드 포털에서 AEM Assets으로 게시될 때마다 **NEW** 폴더의 내용이 무시됩니다.



**방문자 수 기여도 폴더에 새 자산을 업로드하는 방법?**

**Ans.** 기여도 폴더에 자산  [업로드에 대한 자세한 설명서를 참조하십시오](brand-portal-upload-assets-to-contribution-folder.md).



**방문자 수 브랜드 포털 사용자가 NEW 폴더에 업로드한 자산에 축소판/미리 보기가 표시되지 않습니다.**

**Ans.** 이는 설계된 대로 브랜드 포털 끝에서 실행되는 워크플로우가 없습니다.



**방문자 수 AEM Assets에서 Brand Portal에 유동적인 폴더를 게시하면 어떻게 됩니까?**

**Ans.** AEM에서는 폴더가 브랜드 포털에 게시될 때마다 로그가 유지됩니다. 게시 시 브랜드 포털에 게시되지 않은 모든 자산은 복제 대기열에 추가됩니다. 게시 작업이 트리거된 후 폴더에 추가된 모든 자산은 브랜드 포털에 게시되지 않습니다. AEM 사용자가 폴더를 다시 게시하면 이전에 게시되지 않은(복제 큐에 기존) 자산만 브랜드 포털에 게시됩니다.
AEM Assets에서 브랜드 포털로 게시된 모든 폴더 및 기여도 폴더 내의 공유 폴더에 대해 true입니다.

**방문자 수 질문 문의 사항은 누구에게 연락해야 합니까?**

**Ans.** Adobe 계정 관리자 또는 고객 지원에 문의하십시오.

>[!NOTE]
>
>출시 일정은 잠정적이며 변경될 수 있습니다. 업데이트된 릴리스 일정을 받으려면 Adobe 계정 관리자 또는 고객 지원에 문의하십시오.


## 제품 액세스 및 지원(제한된 사이트) {#product-access-and-support-restricted-sites}

다음 사이트는 고객만 사용할 수 있습니다. 고객이고 액세스 권한이 필요한 경우 Adobe 계정 관리자에게 문의하십시오.

* [](https://daycare.day.com) [제품 액세스](https://login.marketing.adobe.com)

* [Adobe 고객 지원](https://helpx.adobe.com/contact.html)
