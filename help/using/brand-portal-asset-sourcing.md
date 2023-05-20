---
title: Brand Portal의 에셋 소싱
seo-title: Asset Sourcing in Brand Portal
description: Adobe Experience Manager Assets Brand Portal에 릴리스된 에셋 소싱 기능에 대한 통찰력을 얻으십시오.
seo-description: Get an insight into the asset sourcing feature released in the Adobe Experience Manager Assets Brand Portal.
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
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 1%

---

# 에셋 소싱 개요 {#overview-asset-sourcing-in-bp}

**자산 소싱** Experience Manager Assets 사용자(관리자/관리자가 아닌 사용자)가 추가 기능을 사용하여 새 폴더를 만들 수 있도록 허용합니다 **자산 기여** Brand Portal 사용자가 만든 새 폴더를 자산 제출에 열어 두는 속성. 그러면 두 개의 추가 하위 폴더(이라고 함)를 만드는 워크플로우가 자동으로 트리거됩니다. **공유됨** 및 **새로 만들기**, 새로 만든 항목 내 **기여도** 폴더를 삭제합니다. 그런 다음 관리자는 기여도 폴더에 추가해야 하는 에셋 유형과 일련의 기준 에셋에 대한 간략한 개요를 업로드하여 요구 사항을 정의합니다 **공유됨** BP 사용자에게 필요한 참조 정보가 있는지 확인하기 위한 폴더입니다. 그런 다음 관리자는 활성 Brand Portal 사용자에게 새로 만든 폴더를 게시하기 전에 기여 폴더에 대한 액세스 권한을 부여할 수 있습니다 **기여도** 폴더를 Brand Portal에 추가합니다. 사용자가 의 콘텐츠 추가를 완료하면 **새로 만들기** 폴더에서 기여도 폴더를 다시 Experience Manager 작성자 환경에 게시할 수 있습니다. 가져오기를 완료하고 Experience Manager Assets 내에 새로 게시된 콘텐츠를 반영하는 데 몇 분 정도 걸릴 수 있습니다.

또한 기존의 모든 기능은 변경되지 않습니다. Brand Portal 사용자는 기여 폴더와 다른 허용된 폴더에서 자산을 보고, 검색하고, 다운로드할 수 있습니다. 또한 관리자는 기여 폴더를 공유하고, 속성을 수정하고, 컬렉션을 통해 에셋을 추가할 수 있습니다.

![Brand Portal 에셋 소싱](assets/asset-sourcing.png)

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

## 사전 요구 사항 {#prerequisites}

* Experience Manager Assets as a Cloud Service 인스턴스, Experience Manager Assets 6.5.2 이상.
* Experience Manager Assets 인스턴스가 Brand Portal으로 구성되었는지 확인합니다. 다음을 참조하십시오. [Brand Portal을 사용하여 Experience Manager Assets 구성](../using/configure-aem-assets-with-brand-portal.md).

<!--
* Ensure that your Brand Portal tenant is configured with one AEM Assets author instance.
-->

>[!NOTE]
>
>에셋 소싱 기능은 기본적으로 Experience Manager Assets as a Cloud Service, Experience Manager Assets 6.5.9 이상에서 활성화됩니다.
>
>기존 구성은 이전 버전에서 계속 작동합니다.

>[!NOTE]
>
>Experience Manager Assets 6.5.4에 알려진 문제가 있습니다. Brand Portal 사용자는 Adobe Developer 콘솔로 업그레이드할 때 기여 폴더의 자산을 Experience Manager Assets에 게시할 수 없습니다.
>
>이 문제는 Experience Manager Assets 6.5.5에서 해결되었습니다. Experience Manager Assets 인스턴스를 최신 서비스 팩으로 업그레이드하고 [구성 업그레이드](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) Adobe Developer 콘솔에서 게시할 수 있습니다.

<!--

>For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your author instance.
-->

<!--
## Configure Asset Sourcing {#configure-asset-sourcing}

**Asset Sourcing** is configured from within the AEM Assets author instance. The administrators can enable the Asset Sourcing feature flag configuration from the **AEM Web Console Configuration** and upload the active Brand Portal users list in **AEM Assets**.

>[!NOTE]
>
>Asset Sourcing is by default enabled on AEM Assets as a Cloud Service. The AEM administrator can directly upload the active Brand Portal users to allow them access to the Asset Sourcing feature.

>[!NOTE]
>
>Before you begin with the configuration, ensure that your AEM Assets instance is configured with Brand Portal. See, [Configure AEM Assets with Brand Portal](../using/configure-aem-assets-with-brand-portal.md). 

The following video demonstrates, how to configure Asset Sourcing on your AEM Assets author instance:

>[!VIDEO](https://video.tv.adobe.com/v/29771)
-->

<!--
### Enable Asset Sourcing {#enable-asset-sourcing}

AEM administrators can enable the Asset Sourcing feature flag from within the AEM Web Console Configuration (a.k.a Configuration Manager).

>[!NOTE]
>
>This step is not applicable for AEM Assets as a Cloud Service.


**To enable Asset Sourcing:**
1. Log in to your AEM Assets author instance and open Configuration Manager. 
Default URL: http:// localhost:4502/system/console/configMgr.
1. Search using the keyword **Asset Sourcing** to locate **[!UICONTROL Asset Sourcing Feature Flag Config]**.
1. Click **[!UICONTROL Asset Sourcing Feature Flag Config]** to open the configuration window.
1. Select the **[!UICONTROL feature.flag.active.status]** check box.
1. Click **[!UICONTROL Save]**.

![](assets/enable-asset-sourcing.png)
-->


### Brand Portal 사용자 목록 업로드 {#upload-bp-user-list}

Experience Manager Assets 관리자는 Experience Manager Assets의 활성 Brand Portal 사용자 목록이 포함된 Brand Portal 사용자 구성(.csv) 파일을 업로드하여 에셋 소싱 기능에 액세스할 수 있습니다.

기여 폴더는 사용자 목록에 정의된 활성 Brand Portal 사용자만 공유할 수 있습니다. 관리자는 구성 파일에 새 사용자를 추가하고 수정된 사용자 목록을 업로드할 수도 있습니다.

>[!NOTE]
>
>Experience Manager Assets 인스턴스가 Brand Portal으로 구성되었는지 확인합니다. 다음을 참조하십시오. [Brand Portal을 사용하여 Experience Manager Assets 구성](../using/configure-aem-assets-with-brand-portal.md).

>[!NOTE]
>
>CSV 파일의 형식은 대량 사용자 가져오기에 대해 Admin Console에서 지원되는 것과 같습니다. 이메일, 이름 및 성은 필수입니다.

관리자는 Admin Console에서 새 사용자를 추가할 수 있습니다. 다음을 참조하십시오. [사용자 관리](brand-portal-adding-users.md) 을 참조하십시오. Admin Console에서 사용자를 추가한 후 이러한 사용자를 Brand Portal 사용자 구성 파일에 추가한 다음 기여도 폴더에 액세스할 수 있는 권한을 할당할 수 있습니다.

**Brand Portal 사용자 목록을 업로드하려면:**

1. Experience Manager Assets 인스턴스에 로그인.
1. 다음에서 **도구**  패널, 다음으로 이동 **[!UICONTROL 에셋]** > **[!UICONTROL Brand Portal 사용자]**.

1. Brand Portal 업로드 기여자 창이 열립니다.
로컬 컴퓨터에서 검색 및 업로드 **구성 파일(.csv)** 활성 Brand Portal 사용자 목록을 포함합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   ![](assets/upload-user-list2.png)


관리자는 기여 폴더를 구성하는 동안 이 사용자 목록에서 특정 사용자에게 액세스 권한을 제공할 수 있습니다. 기여 폴더에 할당된 사용자만 기여 폴더에 액세스하고 Brand Portal에서 Experience Manager Assets으로 에셋을 게시할 수 있습니다.

## 참고 항목 {#reference-articles}

* [기여 폴더 구성 및 Brand Portal에 게시](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [기여 폴더를 Experience Manager Assets에 게시](brand-portal-publish-contribution-folder-to-aem-assets.md)
