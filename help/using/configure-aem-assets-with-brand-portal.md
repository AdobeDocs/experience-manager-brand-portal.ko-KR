---
title: Brand Portal에서 AEM Assets 구성
seo-title: Brand Portal에서 AEM Assets 구성
description: 브랜드 포털에서 AEM Assets 구성에 대한 통찰력을 얻을 수 있습니다.
seo-description: 브랜드 포털에서 AEM Assets 구성에 대한 통찰력을 얻을 수 있습니다.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: ba8a1f09573766643f6a5013a8d181f0f0dbb4f2
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 29%

---


# Brand Portal로 AEM Assets 구성 {#configure-integration}

Adobe Experience Manager(AEM) 자산은 브랜드 포털 테넌트의 승인을 위해 IMS 토큰을 구입하는 Adobe 개발자 콘솔을 통해 브랜드 포털로 구성됩니다. 이제 AEM Assets 클라우드 서비스, AEM Assets 6.3 이상에서 브랜드 포털이 지원됩니다.

AEM Assets을 구성하여 브랜드 포털 사용자와 자산을 게시하고 배포할 수 있습니다. 반면, AEM 6.3 이상 버전에서 브랜드 포털을 구성하면 브랜드 포털 사용자에 대한 자산 게시, 자산 배포 및 자산 기여도 기능을 사용할 수 있습니다.

>[!NOTE]
>
>***AEM Assets 6.3 이상***
>
>이전에는 Brand Portal이 기존 OAuth 게이트웨이를 통해 클래식 UI에 구성되었으며, 이 게이트웨이는 인증을 위해 IMS 액세스 토큰을 가져오는 데 JWT 토큰 교환을 사용합니다.
>
>기존 OAuth를 통한 구성은 2020년 4월 6일부터 더 이상 지원되지 않으며, Adobe 개발자 콘솔을 통해 구성하도록 변경되었습니다.


>[!TIP]
>
>***기존 고객 전용***
>
>기존 OAuth 게이트웨이 구성은 기존 고객을 위해 계속 작동합니다.
>
>기존 OAuth 게이트웨이 구성에 문제가 있는 경우 기존 구성을 삭제하고 Adobe 개발자 콘솔을 통해 새 구성을 만드십시오.


Brand Portal에서 AEM Assets을 구성하는 단계는 AEM 버전과 처음 구성하는 것인지 아니면 기존 구성을 업그레이드하는 것인지에 따라 다릅니다:

| **AEM 버전** | **새 구성** | **업그레이드 구성** |
|---|---|---|
| **클라우드 서비스로서의 AEM Assets** | [구성 만들기](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5(6.5.4.0 이상)** | [구성 만들기](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [구성 업그레이드](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4(6.4.8.0 이상)** | [구성 만들기](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [구성 업그레이드](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3(6.3.3.8 이상)** | [구성 만들기](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [구성 업그레이드](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | 지원 문의 | 지원 문의 |


