---
title: 브랜드 포털의 자산 소싱
seo-title: 브랜드 포털의 자산 소싱
description: Adobe Experience Manager 자산 브랜드 포털에서 제공하는 자산 소싱 기능에 대한 통찰력을 얻을 수 있습니다.
seo-description: Adobe Experience Manager 자산 브랜드 포털에서 제공하는 자산 소싱 기능에 대한 통찰력을 얻을 수 있습니다.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
product: experience-manager
sub-product: 자산
feature: brand-portal
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
translation-type: tm+mt
source-git-commit: 9c937603cf325919cb49d3418b06266fa1b93cf1
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 7%

---


# 자산 소싱 개요 {#overview-asset-sourcing-in-bp}

**자산** 소스를 사용하면 AEM 사용자(관리자/비관리 사용자)가 추가 자산  **기여도** 속성을 사용하여 새 폴더를 만들 수 있으므로, 브랜드 포털 사용자가 만든 새 폴더를 자산 제출에 열도록 할 수 있습니다. 이렇게 하면 새로 만든 **기여도** 폴더 내에서 **SHARED** 및 **NEW**&#x200B;라는 두 개의 추가 하위 폴더를 만드는 워크플로우가 자동으로 트리거됩니다. 그러면 AEM 관리자는 BP 사용자가 필요한 참조 정보를 갖도록 하기 위해 기여도 폴더에 추가해야 하는 자산 유형과 기준 자산 세트에 대한 간단한 내용을 **SHARED** 폴더에 업로드하여 요구 사항을 정의합니다. 그러면 관리자는 새로 만든 **기여도** 폴더를 브랜드 포털에 게시하기 전에 기여도 폴더에 대한 액세스 권한을 활성 브랜드 포털 사용자에게 부여할 수 있습니다. 사용자가 **NEW** 폴더에 콘텐트를 추가했으면 기여도 폴더를 다시 AEM 작성자 환경에 게시할 수 있습니다. 가져오기를 완료하고 AEM Assets 내에 새로 게시된 컨텐츠를 반영하려면 몇 분 정도 걸릴 수 있습니다.

또한 모든 기존 기능은 변경되지 않습니다. 브랜드 포털 사용자는 기여도 폴더뿐만 아니라 허용된 다른 폴더에서 자산을 보고, 검색하고, 다운로드할 수 있습니다. 또한 관리자는 기여도 폴더를 추가로 공유하고, 속성을 수정하고, 컬렉션에 자산을 추가할 수 있습니다.

## 전제 조건 {#prerequisites}

* AEM 6.5.2 이상
* AEM Assets 인스턴스가 브랜드 포털로 구성되어 있는지 확인합니다. 참조: [브랜드 포털과 함께 AEM Assets 구성](../using/configure-aem-assets-with-brand-portal.md).
* 브랜드 포털 테넌트가 하나의 AEM Assets 작성자 인스턴스로 구성되어 있는지 확인합니다.

>[!NOTE]
>
>자산 소싱은 AEM Assets에서 Cloud Service으로 지원되지 않습니다.


>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

![브랜드 포털 자산 소싱](assets/asset-sourcing.png)


>[!NOTE]
>
>AEM 6.5.4에서 알려진 문제가 있습니다. 브랜드 포털 사용자는 Adobe 개발자 콘솔로 업그레이드하기 위해 기여도 폴더의 자산을 AEM Assets에 게시할 수 없습니다.
>
>AEM 6.5.5에서 문제가 해결되었습니다. Adobe 개발자 콘솔에서 AEM Assets 인스턴스를 최신 서비스 팩 AEM 6.5.5로 업그레이드하고 [을(를) 업그레이드 할 수 있습니다.](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65)
>
>AEM 6.5.4를 즉시 수정하려면 [핫픽스를 다운로드](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041)하고 작성자 인스턴스에 설치하는 것이 좋습니다.


## 참고 항목 {#reference-articles}

**관리자**

* [AEM에서 자산 소싱 구성](brand-portal-configure-asset-sourcing.md)
* [브랜드 포털 사용자 목록 업로드](brand-portal-configure-asset-sourcing.md)
* [기여도 폴더 구성](brand-portal-contribution-folder.md)
* [기여도 폴더에 기준 자산 업로드](brand-portal-upload-baseline-assets.md)
* [브랜드 포털에 기여도 폴더 게시](brand-portal-publish-contribution-folder-to-brand-portal.md)

**브랜드 포털 사용자의 경우**

* [자산 요구 사항 다운로드](brand-portal-download-asset-requirements.md)
* [기여도 폴더에 새 자산 업로드](brand-portal-upload-assets-to-contribution-folder.md)
* [AEM Assets에 기여도 폴더 게시](brand-portal-publish-contribution-folder-to-aem-assets.md)
