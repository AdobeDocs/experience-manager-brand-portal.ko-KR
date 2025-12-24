---
title: Brand Portal의 자산 소싱
description: insight을 Adobe Experience Manager Assets Brand Portal에 릴리스된 에셋 소싱 기능으로 안내합니다.
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
sub-product: assets
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: Experience Manager 6.5
kt: 3838
exl-id: 2c132a7a-ed10-4856-8378-67939167ea60
source-git-commit: 9b8a415fa3a19e462ea797cfc9c3ea9b9323723e
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 11%

---

# 자산 소싱 개요 {#overview-asset-sourcing-in-bp}

**자산 소싱**&#x200B;을 통해 Experience Manager Assets 사용자(관리자/관리자가 아닌 사용자)는 추가 **자산 기여** 속성을 사용하여 새 폴더를 만들 수 있으므로 Brand Portal 사용자가 만든 새 폴더가 자산 제출에 열려 있도록 합니다. 이렇게 하면 새로 만든 **기여도** 폴더 내에 **SHARED** 및 **NEW**&#x200B;이라는 두 개의 추가 하위 폴더를 만드는 워크플로가 자동으로 트리거됩니다. 관리자는 기여도 폴더에 추가해야 하는 에셋 유형에 대한 간단한 개요를 업로드하여 요구 사항을 정의합니다. 기준선 에셋 집합을 **SHARED** 폴더에 업로드하여 Brand Portal 사용자에게 필요한 참조 정보를 제공합니다. 그런 다음 관리자는 새로 만든 **기여도** 폴더를 Brand Portal에 게시하기 전에 활성 Brand Portal 사용자에게 기여도 폴더에 대한 액세스 권한을 부여할 수 있습니다. 사용자가 **NEW** 폴더에 콘텐츠를 추가했으면 기여 폴더를 다시 Experience Manager 작성 환경에 게시할 수 있습니다. 가져오기를 완료하고 Experience Manager Assets 내에 새로 게시된 콘텐츠를 반영하는 데 몇 분 정도 걸릴 수 있습니다.

또한 기존의 모든 기능은 변경되지 않습니다. Brand Portal 사용자는 기여 폴더와 다른 허용된 폴더에서 자산을 보고, 검색하고, 다운로드할 수 있습니다. 관리자는 추가적으로 기여 폴더를 공유하고, 속성을 수정하고, 컬렉션에 자산을 추가할 수 있습니다.

![Brand Portal 자산 소싱](assets/asset-sourcing.png)

>[!VIDEO](https://video.tv.adobe.com/v/32893/?captions=kor&quality=12)

## 사전 요구 사항 {#prerequisites}

* Experience Manager Assets as a Cloud Service 인스턴스, Experience Manager Assets 6.5.2 이상.
* Experience Manager Assets 인스턴스가 Brand Portal으로 구성되었는지 확인합니다. [Brand Portal으로 Experience Manager Assets 구성](../using/configure-aem-assets-with-brand-portal.md)을 참조하세요.

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
>Experience Manager Assets 6.5.4에 알려진 문제가 있습니다. Brand Portal 사용자는 Adobe Developer Console으로 업그레이드할 때 기여 폴더의 자산을 Experience Manager Assets에 게시할 수 없습니다.
>
>이 문제는 Experience Manager Assets 6.5.5에서 해결되었습니다. Experience Manager Assets 인스턴스를 최신 서비스 팩으로 업그레이드하고 Adobe Developer Console에서 [구성을 업그레이드](https://experienceleague.adobe.com/ko/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal#upgrade-integration-65)할 수 있습니다.

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
>Experience Manager Assets 인스턴스가 Brand Portal으로 구성되었는지 확인합니다. [Brand Portal으로 Experience Manager Assets 구성](../using/configure-aem-assets-with-brand-portal.md)을 참조하세요.

>[!NOTE]
>
>CSV 파일의 형식은 대량 사용자 가져오기용 Admin Console에서 지원되는 것과 동일합니다. 이메일, 이름, 성은 필수입니다.

관리자는 Admin Console에서 새 사용자를 추가할 수 있습니다. 자세한 내용을 보려면 [사용자 관리](brand-portal-adding-users.md)(으)로 이동하십시오. Admin Console에서 사용자를 추가한 후 이러한 사용자를 Brand Portal 사용자 구성 파일에 추가한 다음 기여도 폴더에 액세스할 수 있는 권한을 할당할 수 있습니다.

**Brand Portal 사용자 목록을 업로드하려면:**

1. Experience Manager Assets 인스턴스에 로그인.
1. [!UICONTROL 도구] 패널에서 **[!UICONTROL Assets]** > **[!UICONTROL Brand Portal 사용자]**(으)로 이동합니다.

1. Brand Portal 업로드 기여자 창이 열립니다.
로컬 컴퓨터에서 활성 Brand Portal 사용자 목록을 포함하는 **구성 파일(.csv)을 업로드**&#x200B;합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   ![](assets/upload-user-list2.png)

관리자는 기여 폴더를 구성하는 동안 이 사용자 목록에서 특정 사용자에게 액세스 권한을 제공할 수 있습니다. 기여 폴더에 할당된 사용자만 기여 폴더에 액세스하고 Brand Portal에서 Experience Manager Assets으로 에셋을 게시할 수 있습니다.

## 추가 참조 {#reference-articles}

* [기여도 폴더 구성 및 Brand Portal에 게시](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [Experience Manager Assets에 기여 폴더 게시](brand-portal-publish-contribution-folder-to-aem-assets.md)
