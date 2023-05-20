---
title: Brand Portal에 대한 관리자 액세스
seo-title: Administer user access on Brand Portal
description: Brand Portal에서 게스트 액세스 및 새 사용자 액세스를 구성합니다.
seo-description: Configure guest access and new users access on brand portal.
uuid: 522b499d-33a0-455f-ac7e-719face48009
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 393025b4-722d-4e81-8a47-f83415d0b9b6
role: Admin
exl-id: 27a9cd26-9bb3-473b-b1ac-37f77975c912
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 9%

---

# Brand Portal에 대한 관리자 액세스 {#administer-user-access-on-brand-portal}

Adobe Experience Manager Assets Brand Portal 6.4.2 이상에서는 관리자가 게스트 액세스를 구성하고 사용자가 조직의 Brand Portal에 대한 액세스를 요청할 수 있도록 권한을 부여합니다. 이러한 구성은 다음과 같이 제공되었습니다. **[!UICONTROL 액세스 설정]** 관리 패널의 구성 두 설정은 기본적으로 비활성화되어 있습니다.

![](assets/access-configs.png)

**A**   다음을 사용하여 Brand Portal에서 게스트 액세스를 허용하는 구성 **[!UICONTROL 게스트 액세스?]** Brand Portal 시작 화면의 링크. (기본값은 비활성화됨)

**B**   사용자가 다음을 사용하여 Brand Portal 액세스를 요청할 수 있도록 구성 **[!UICONTROL 액세스 권한이 필요하십니까?]** Brand Portal 시작 화면의 링크. (기본값은 비활성화됨)

## 게스트 액세스 허용 {#allow-guest-access}

게스트 액세스를 허용함으로써 사용자는 Brand Portal에 로그인하지 않고도 공개 자산에 액세스할 수 있습니다.
게스트 액세스를 허용하려면 관리자가 다음 단계를 수행해야 합니다.

1. 상단의 도구 모음에서 AEM 로고를 선택하여 관리 도구에 액세스합니다.
1. 관리 도구 패널에서 를 선택합니다. **[!UICONTROL 액세스]** 열다 **[!UICONTROL 액세스 설정]** 페이지를 가리키도록 업데이트하는 중입니다.
1. 활성화 **[!UICONTROL 게스트 액세스 허용]** 구성.
1. **[!UICONTROL 변경 사항을 저장합니다.]**
1. 로그아웃하여 변경 사항을 적용합니다.

![](assets/bp-welcome-screen.png)

## 사용자 액세스 요청 허용 {#allow-users-to-request-access}

관리자는 조직 사용자가 시작 화면에서 Brand Portal에 대한 액세스를 요청하도록 허용할 수 있습니다. 단, 관리자는 **[!UICONTROL 사용자가 액세스 권한을 요청하도록 허용]** 시작 화면에 액세스 요청 링크가 나타나도록 구성합니다.

조직 사용자가 Brand Portal에 대한 액세스 권한을 요청할 수 있도록 하려면 관리자는 다음을 수행해야 합니다.

1. 상단의 도구 모음에서 AEM 로고를 선택하여 관리 도구에 액세스합니다.
1. 관리 도구 패널에서 를 선택합니다. **[!UICONTROL 액세스]** 열다 **[!UICONTROL 액세스 설정]** 페이지를 가리키도록 업데이트하는 중입니다.
1. 활성화 **[!UICONTROL 사용자가 액세스 권한을 요청하도록 허용]** 구성.
1. **[!UICONTROL 변경 사항을 저장합니다.]**
1. 로그아웃하여 변경 사항을 적용합니다.
