---
title: Brand Portal의 자산 소싱
seo-title: Brand Portal의 자산 소싱
description: Adobe Experience Manager Assets Brand Portal에서 릴리스된 자산 소싱 기능에 대한 통찰력을 얻을 수 있습니다.
seo-description: Adobe Experience Manager Assets Brand Portal에서 릴리스된 자산 소싱 기능에 대한 통찰력을 얻을 수 있습니다.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
sub-product: assets
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
exl-id: 2c132a7a-ed10-4856-8378-67939167ea60
source-git-commit: e8bb1149582329f5304bda7e5e67e8dcc27cfc7b
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 7%

---

# 자산 소싱 개요 {#overview-asset-sourcing-in-bp}

**자산** 소스를 사용하면 AEM 사용자(관리자/관리자가 아닌 사용자)가 추가적인  **자산 기여 속성** 으로 새 폴더를 만들 수 있으므로 Brand Portal 사용자가 자산 제출을 위해 만든 새 폴더를 만들 수 있습니다. 이렇게 하면 새로 만든 **기여도** 폴더 내에서 **SHARED** 및 **NEW**&#x200B;라는 두 개의 추가 하위 폴더를 만드는 워크플로우가 자동으로 트리거됩니다. 그런 다음 AEM 관리자는 기여도 폴더에 추가해야 하는 자산 유형과 기준 자산 세트에 대한 요약을 **SHARED** 폴더에 업로드하여 BP 사용자에게 필요한 참조 정보가 있는지 확인함으로써 요구 사항을 정의합니다. 그런 다음 관리자는 새로 만든 **기여도** 폴더를 Brand Portal에 게시하기 전에 활성 Brand Portal 사용자에게 기여도 폴더에 대한 액세스 권한을 부여할 수 있습니다. 사용자가 **NEW** 폴더에서 컨텐츠를 추가했으면 기여 폴더를 다시 AEM 작성 환경에 게시할 수 있습니다. 가져오기를 완료하고 AEM Assets 내에 새로 게시된 콘텐츠를 반영하는 데 몇 분이 걸릴 수 있습니다.

또한 기존 기능은 모두 변경되지 않고 그대로 유지됩니다. Brand Portal 사용자는 기여 폴더 및 허용된 다른 폴더에서 자산을 보고 검색하고 다운로드할 수 있습니다. 또한 관리자는 기여도 폴더를 추가로 공유하고, 속성을 수정하고, 컬렉션에 자산을 추가할 수 있습니다.

## 전제 조건 {#prerequisites}

* AEM Assets을 Cloud Service 인스턴스로 AEM Assets 6.5.2 이상
* AEM Assets 인스턴스가 Brand Portal으로 구성되어 있는지 확인합니다. [Brand Portal으로 AEM Assets 구성](../using/configure-aem-assets-with-brand-portal.md)을 참조하십시오.
* Brand Portal 테넌트가 하나의 AEM Assets 작성자 인스턴스로 구성되어 있는지 확인합니다.

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

![Brand Portal 자산 소싱](assets/asset-sourcing.png)


>[!NOTE]
>
>AEM Assets 6.5.4에서 알려진 문제가 있습니다. Brand Portal 사용자는 Adobe 개발자 콘솔로 업그레이드할 때 기여도 폴더의 자산을 AEM Assets에 게시할 수 없습니다.
>
>이 문제는 AEM 6.5.5에서 수정되었습니다. AEM Assets 인스턴스를 최신 서비스 팩 AEM 6.5.5로 업그레이드하고 Adobe 개발자 콘솔에서 ](https://docs.adobe.com/content/help/ko/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) 구성을 업그레이드할 수 있습니다.[
>
>AEM 6.5.4를 즉시 수정하려면 [핫픽스를 다운로드](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041)하고 작성자 인스턴스에 설치하는 것이 좋습니다.

## 자산 소싱 {#configure-asset-sourcing} 구성

**자산** 소스는 AEM Assets 작성자 인스턴스 내에서 구성됩니다. 관리자는 **AEM Web Console 구성**&#x200B;에서 Asset Sourcing 기능 플래그 구성을 활성화하고 **AEM Assets**&#x200B;에서 활성 Brand Portal 사용자 목록을 업로드할 수 있습니다.

>[!NOTE]
>
>기본적으로 AEM Assets에서 Cloud Service으로 자산 소싱이 활성화되어 있습니다. AEM 관리자는 활성 Brand Portal 사용자를 직접 업로드하여 자산 소싱 기능에 액세스할 수 있습니다.

>[!NOTE]
>
>구성을 시작하기 전에 AEM Assets 인스턴스가 Brand Portal으로 구성되어 있는지 확인하십시오. [Brand Portal으로 AEM Assets 구성](../using/configure-aem-assets-with-brand-portal.md)을 참조하십시오.

다음 비디오에서는 AEM Assets 작성자 인스턴스에서 자산 소싱을 구성하는 방법을 보여 줍니다.

>[!VIDEO](https://video.tv.adobe.com/v/29771)

### 자산 소싱 {#enable-asset-sourcing} 활성화

AEM 관리자는 AEM 웹 콘솔 구성(구성 관리자라고도 함) 내에서 자산 소싱 기능 플래그를 활성화할 수 있습니다.

>[!NOTE]
>
>이 단계는 AEM Assets as a Cloud Service에 적용할 수 없습니다.


**자산 소싱을 사용하려면**
1. AEM Assets 작성자 인스턴스에 로그인하고 구성 관리자를 엽니다.
기본 URL:http:// localhost:4502/system/console/configMgr 을 참조하십시오.
1. **자산 소싱** 키워드를 사용하여 **[!UICONTROL 자산 소싱 기능 플래그 구성]**&#x200B;을 찾습니다.
1. **[!UICONTROL 자산 소싱 기능 플래그 구성]**&#x200B;을 클릭하여 구성 창을 엽니다.
1. **[!UICONTROL feature.flag.active.status]** 확인란을 선택합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

![](assets/enable-asset-sourcing.png)

### Brand Portal 사용자 목록 업로드 {#upload-bp-user-list}

AEM 관리자는 AEM Assets에서 활성 Brand Portal 사용자 목록이 포함된 Brand Portal 사용자 구성(.csv) 파일을 업로드할 수 있습니다. 기여 폴더는 사용자 목록에 정의된 활성 Brand Portal 사용자만 공유할 수 있습니다. 관리자는 구성 파일에 새 사용자를 추가하고 수정된 사용자 목록을 업로드할 수도 있습니다.

>[!NOTE]
>
>CSV 파일의 형식은 대량 사용자 가져오기에 대해 Admin Console에서 지원되는 형식과 동일합니다. 이메일, 이름 및 성은 필수입니다.

관리자는 AEM Admin Console에서 새 사용자를 추가할 수 있습니다. 자세한 내용은 [사용자 관리](brand-portal-adding-users.md)를 참조하십시오. Admin Console에서 사용자를 추가하면 이러한 사용자를 Brand Portal 사용자 구성 파일에 추가한 다음 기여도 폴더에 액세스할 수 있는 권한을 할당할 수 있습니다.

**Brand Portal 사용자 목록을 업로드하려면 다음을 수행하십시오.**
1. AEM Assets 인스턴스에 로그인합니다.
1. **도구** 패널에서 **[!UICONTROL 자산]** > **[!UICONTROL Brand Portal 사용자]**&#x200B;로 이동합니다.

1. Brand Portal 업로드 기여자 창이 열립니다.
로컬 시스템에서 탐색하고 활성 Brand Portal 사용자 목록이 포함된 **구성(.csv) 파일**&#x200B;을(를) 업로드합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   ![](assets/upload-user-list2.png)


관리자는 기여 폴더를 구성하는 동안 이 사용자 목록에서 특정 사용자에게 액세스 권한을 제공할 수 있습니다. 기여도 폴더에 지정된 사용자만 기여도 폴더에 액세스하고 Brand Portal의 자산을 AEM Assets에 게시할 수 있습니다.

## 참고 항목 {#reference-articles}

* [기여도 폴더를 Brand Portal에 구성 및 게시](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [AEM Assets에 기여도 폴더 게시](brand-portal-publish-contribution-folder-to-aem-assets.md)
