---
title: Brand Portal에서 AEM Assets 구성
seo-title: Configure AEM Assets with Brand Portal
description: Brand Portal으로 AEM Assets 구성에 대한 통찰력을 얻을 수 있습니다.
seo-description: Get an insight into configuring AEM Assets with Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
role: Admin
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: ea3242459776037499b21b33ba40357afc8bf234
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 28%

---

# Brand Portal에서 AEM Assets 구성 {#configure-integration}

Brand Portal과 Adobe Experience Manager Assets를 구성하면 Brand Portal 사용자에 대한 자산 게시, 자산 분배 및 자산 기여 기능이 활성화됩니다. AEM Assets 사용자는 Brand Portal 사용자와 자산을 게시하고 배포할 수 있습니다. Brand Portal 사용자는 공유 자산에 액세스하고 새 자산을 자산 기여 폴더에 업로드하고 다시 AEM Assets에 게시하여 기여할 수 있습니다.

Brand Portal과 AEM Assets을 구성할 수 있습니다.

* AEM Assets as a Cloud Service
* AEM Assets (온-프레미스 및 관리 서비스) 6.3 이상

AEM Assets as a Cloud Service은 Cloud Manager에서 Brand Portal을 활성화하여 Brand Portal으로 자동으로 구성됩니다. 활성화 워크플로우는 백엔드에 필수 구성을 만들고 Cloud Service 인스턴스로 AEM Assets과 동일한 IMS 조직에서 Brand Portal을 활성화합니다.

반면, AEM Assets(온-프레미스 및 관리 서비스)는 Brand Portal 테넌트의 인증을 위해 IMS(Adobe Identity Management Services) 토큰을 전달하는 Adobe 개발자 콘솔을 사용하여 Brand Portal으로 수동으로 구성합니다.

>[!NOTE]
>
>***AEM Assets 6.3 이상용***
>
>이전에는 Brand Portal이 기존 OAuth 게이트웨이를 통해 클래식 인터페이스에 구성되었으며, 이 게이트웨이는 인증을 위해 IMS 토큰을 가져오는 데 JWT(JSON 웹 토큰) 교환을 사용합니다.
>
>기존 OAuth를 통한 구성은 2020년 4월 6일부터 더 이상 지원되지 않으며, Adobe 개발자 콘솔을 통한 구성으로 변경되었습니다.


>[!TIP]
>
>***기존 고객 전용(온-프레미스 및 관리 서비스)***
>
>기존 OAuth 게이트웨이 구성이 기존 고객을 위해 계속 작동합니다.
>
>기존 OAuth 게이트웨이 구성 문제가 발생하는 경우 기존 구성을 삭제하고 Adobe 개발자 콘솔을 통해 새 구성을 만드십시오.

Brand Portal으로 AEM Assets을 구성하는 단계는 AEM 버전과 처음 구성하는 것인지 아니면 기존 구성을 업그레이드하는 것인지에 따라 다릅니다.

| **AEM 버전** | **새 구성** | **구성 업그레이드** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Brand Portal 활성화](https://docs.adobe.com/content/help/ko/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5(6.5.4.0 이상)** | [구성 만들기](https://docs.adobe.com/content/help/ko/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [구성 업그레이드](https://docs.adobe.com/content/help/ko/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4(6.4.8.0 이상)** | [구성 만들기](https://docs.adobe.com/content/help/ko-KR/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [구성 업그레이드](https://docs.adobe.com/content/help/ko/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 이상)** | [구성 만들기](https://helpx.adobe.com/kr/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [구성 업그레이드](https://helpx.adobe.com/kr/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | 지원 문의 | 지원 문의 |
