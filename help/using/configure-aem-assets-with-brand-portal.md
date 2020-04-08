---
title: 브랜드 포털에서 AEM 자산 구성
seo-title: 브랜드 포털에서 AEM 자산 구성
description: 브랜드 포털에서 AEM 자산 구성에 대한 통찰력을 얻을 수 있습니다.
seo-description: 브랜드 포털에서 AEM 자산 구성에 대한 통찰력을 얻을 수 있습니다.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: dc10879caf91b81deda08682548143c60500fd1b

---


# 브랜드 포털에서 AEM 자산 구성 {#configure-integration}

AEM(Adobe Experience Manager) 자산은 Adobe I/O를 통해 브랜드 포털로 구성되며, 브랜드 포털 임차인의 승인을 위해 IMS 토큰을 조달합니다. 이제 브랜드 포털은 AEM Assets 클라우드 서비스, AEM Assets 6.3 이상에서 지원됩니다.

브랜드 포털에서 AEM 자산을 구성하면 브랜드 포털 사용자와 자산을 게시하고 배포할 수 있습니다. 반면에 AEM 6.3(및 이상)에서 브랜드 포털을 구성하면 브랜드 포털 사용자에 대한 자산 게시, 자산 배포 및 자산 기여도 기능을 사용할 수 있습니다.

>[!NOTE]
>
>***AEM Assets 6.3 이상***
>
>이전에는 브랜드 포털이 레거시 OAuth 게이트웨이를 통해 클래식 UI에 구성되었으며, 이 게이트웨이는 JWT 토큰 교환을 사용하여 인증에 대한 IMS 액세스 토큰을 획득했습니다.
>
>기존 OAuth를 통한 구성은 2020년 4월 6일부터 더 이상 지원되지 않으며, Adobe I/O를 통해 구성으로 변경되었습니다.


>[!TIP]
>
>***기존 고객만 해당***
>
>기존 레거시 OAuth 게이트웨이 구성을 계속 사용하는 것이 좋습니다. 기존 OAuth 게이트웨이 구성 문제가 발생하면 기존 구성을 삭제하고 Adobe I/O를 통해 새 구성을 만드십시오.


브랜드 포털과 함께 AEM 자산을 구성하는 단계는 AEM 버전, 최초 구성 여부 또는 기존 구성을 업그레이드하는지에 따라 다릅니다.

| **AEM 버전** | **새 구성** | **업그레이드 구성** |
|---|---|---|
| **클라우드 서비스로서의 AEM Assets** | [구성 만들기](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5(6.5.4.0 이상)** | [구성 만들기](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [업그레이드 구성](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4(6.4.8.0 이상)** | [구성 만들기](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [업그레이드 구성](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3(6.3.3.8 이상)** | [구성 만들기](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [업그레이드 구성](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | 지원 문의 | 지원 문의 |


<!--
   Comment Type: draft

   <li> </li>
   -->

<!--
   Comment Type: draft

   <li>Step text</li>
   -->
