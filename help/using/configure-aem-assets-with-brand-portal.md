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
source-git-commit: 59eeaedd7f66a0a5affa53f82f3ebbb2bcea535d
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 28%

---


# Brand Portal로 AEM Assets 구성 {#configure-integration}

브랜드 포털과 함께 Adobe Experience Manager 자산을 구성하면 브랜드 포털 사용자에 대한 자산 게시, 자산 배포 및 자산 기여도 기능을 사용할 수 있습니다. AEM Assets 사용자는 Brand Portal 사용자와 함께 에셋을 게시하고 배포할 수 있습니다. 브랜드 포털 사용자는 에셋 기여도 폴더에 새 에셋을 업로드하고 다시 AEM Assets에 게시하여 공유 에셋에 액세스하고 증여할 수 있습니다.

브랜드 포털에서 AEM Assets 구성이 지원됩니다.
* AEM Assets as a Cloud Service
* AEM Assets(온-프레미스 및 관리 서비스) 6.3 이상

AEM Assets은 Cloud Manager에서 브랜드 포털을 활성화하여 브랜드 포털로 자동으로 구성됩니다. 활성화 워크플로우는 백 엔드에 필수 구성을 생성하고 Cloud Service 인스턴스로 AEM Assets과 동일한 IMS 조직에 있는 브랜드 포털을 활성화합니다.

반면, AEM Assets(온-프레미스 및 관리 서비스)는 브랜드 포털 임차인 인증을 위해 Adobe Identity Management 서비스(IMS) 토큰을 조달하는 Adobe 개발자 콘솔을 사용하여 브랜드 포털로 수동으로 구성됩니다.

>[!NOTE]
>
>***AEM Assets 6.3 이상의 경우***
>
>이전에는 브랜드 포털이 JWT(JSON Web Token) 교환을 사용하여 인증에 대한 IMS 토큰을 입수하는 레거시 OAuth 게이트웨이를 통해 클래식 인터페이스에서 구성되었습니다.
>
>기존 OAuth를 통한 구성은 2020년 4월 6일부터 더 이상 지원되지 않으며, Adobe 개발자 콘솔을 통한 구성으로 변경되었습니다.


>[!TIP]
>
>***기존 고객의 경우(온-프레미스 및 관리 서비스)***
>
>기존 OAuth 게이트웨이 구성은 기존 고객을 위해 계속 작동합니다.
>
>기존 OAuth 게이트웨이 구성에 문제가 있는 경우 기존 구성을 삭제하고 Adobe 개발자 콘솔을 통해 새 구성을 만드십시오.

브랜드 포털로 AEM Assets을 구성하는 단계는 AEM 버전 및 처음 구성할지 또는 기존 구성을 업그레이드하는지에 따라 다릅니다.

| **AEM 버전** | **새 구성** | **업그레이드 구성** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [브랜드 포털 활성화](https://docs.adobe.com/content/help/ko-KR/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5(6.5.4.0 이상)** | [구성 만들기](https://docs.adobe.com/content/help/ko-KR/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [구성 업그레이드](https://docs.adobe.com/content/help/ko-KR/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 이상)** | [구성 만들기](https://docs.adobe.com/content/help/ko-KR/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [구성 업그레이드](https://docs.adobe.com/content/help/ko-KR/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3(6.3.3.8 이상)** | [구성 만들기](https://helpx.adobe.com/kr/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [구성 업그레이드](https://helpx.adobe.com/kr/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | 지원 문의 | 지원 문의 |
