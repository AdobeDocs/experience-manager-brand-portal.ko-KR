---
title: Brand Portal을 사용하여 Experience Manager Assets 구성
seo-title: Configure Experience Manager Assets with Brand Portal
description: Brand Portal을 사용하여 Experience Manager Assets 구성에 대한 통찰력을 얻으십시오.
seo-description: Get an insight into configuring Experience Manager Assets with Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
role: Admin
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: 454b05c05359a2068cc29124f826d5bd25a1bad1
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 8%

---

# Brand Portal을 사용하여 Experience Manager Assets 구성 {#configure-integration}

Brand Portal과 함께 Adobe Experience Manager Assets을 구성하면 Brand Portal 사용자에게 자산 게시, 자산 배포 및 자산 기여 기능이 활성화됩니다. 이를 통해 Experience Manager Assets 사용자는 Brand Portal 사용자와 함께 에셋을 게시하고 배포할 수 있습니다. Brand Portal 사용자는 새 에셋을 에셋 기여 폴더에 업로드하고 다시 Experience Manager Assets에 게시하여 공유 에셋에 액세스하고 기여할 수 있습니다.

Brand Portal을 사용하여 Experience Manager Assets 구성은에서 지원됩니다.

* Experience Manager Assets as a Cloud Service
* Experience Manager Assets(On-Premise 및 Managed Service) 6.5 이상

Experience Manager Assets as a Cloud Service Cloud Manager에서 Brand Portal을 활성화하여 Brand Portal을 자동으로 구성합니다. 활성화 워크플로우는 백엔드에서 필요한 구성을 만들고 Experience Manager Assets as a Cloud Service 인스턴스와 동일한 IMS 조직에서 Brand Portal을 활성화합니다.

반면 Experience Manager Assets(On-Premise 및 Managed Service)는 Brand Portal 테넌트의 인증을 위해 Adobe IMS(Identity Management Services) 토큰을 조달하는 Adobe Developer Console을 사용하여 Brand Portal으로 수동으로 구성됩니다.

>[!NOTE]
>
>***Experience Manager Assets 6.5 이상의 경우***
>
>이전에는 Brand Portal이 기존 OAuth 게이트웨이를 통해 클래식 인터페이스에 구성되었으며, 이 게이트웨이는 인증을 위해 IMS 토큰을 가져오는 데 JSON 웹 토큰(JWT) 교환을 사용합니다.
>
>기존 OAuth를 통한 구성은 2020년 4월 6일부터 더 이상 지원되지 않으며, Adobe 개발자 콘솔을 통한 구성으로 변경되었습니다.


>[!TIP]
>
>***기존 고객 전용(온-프레미스 및 관리 서비스)***
>
>기존 OAuth 게이트웨이 구성이 기존 고객에 대해 계속 작동합니다.
>
>기존 OAuth 게이트웨이 구성 문제가 발생하는 경우 기존 구성을 삭제하고 Adobe Developer Console을 통해 새 구성을 만드십시오.

Brand Portal에서 AEM Assets을 구성하는 단계는 AEM 버전과 처음 구성하는 것인지 아니면 기존 구성을 업그레이드하는 것인지에 따라 다릅니다.

| **AEM 버전** | **새 구성** | **구성 업그레이드** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Brand Portal 활성화](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5(6.5.4.0 이상)** | [구성 만들기](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [구성 업그레이드](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
