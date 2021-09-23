---
title: Brand Portal에 대한 게스트 액세스
seo-title: Guest Access to Brand Portal
description: 게스트 액세스를 허용하고 인증 없이 많은 사용자를 온보딩하는 데 드는 노력을 절약할 수 있습니다.
seo-description: Allow guest access and save the effort to onboard numerous users without authentication.
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: VG
topic-tags: introduction
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
exl-id: ecce0a45-abae-41c4-9ea7-5dfdcf19e5ea
source-git-commit: e7877973da87362c5fddd6c3aa8135719eff044a
workflow-type: tm+mt
source-wordcount: '998'
ht-degree: 1%

---

# Brand Portal에 대한 게스트 액세스 {#guest-access-to-brand-portal}

Experience Manager Assets Brand Portal을 통해 게스트가 포털에 액세스할 수 있습니다. 게스트 사용자는 포털에 액세스하는 데 자격 증명이 필요하지 않으며 포털의 공개 자산(및 컬렉션)에 액세스할 수 있습니다. 게스트 세션의 사용자는 게스트 사용자가 [[!UICONTROL 종료 세션]](#exit-guest-session)을 선택하지 않는 한 세션이 시작될 때까지 Lightbox(개인 컬렉션)에 자산을 추가하고 다운로드할 수 있습니다.

게스트 액세스 기능을 통해 조직에서 [승인된 자산](../using/brand-portal-sharing-folders.md#how-to-share-folders)을 온보딩할 필요 없이 규모에 맞게 의도한 대상과 빠르게 공유할 수 있습니다. Brand Portal 6.4.2 버전은 여러 동시 게스트 사용자를 제공할 수 있으며, 이는 조직당 총 사용자 할당량 10%의 수치입니다. 게스트 액세스를 허용하면 Brand Portal에서 제한된 기능을 가진 수십 명의 사용자를 관리하고 온보드 방식으로 관리하는 데 시간이 절약됩니다.\
조직은 관리 도구 패널의 **[!UICONTROL 액세스]** 설정에서 **[!UICONTROL 게스트 액세스 허용]** 옵션을 사용하여 조직의 Brand Portal 계정에 대한 게스트 액세스를 활성화(또는 비활성화)할 수 있습니다.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## 게스트 세션 시작 {#begin-guest-session}

Brand Portal을 익명으로 입력하려면 **[!UICONTROL 여기에**[!UICONTROL &#x200B;게스트 액세스에 해당하는 ]**을 클릭하세요.]** Brand Portal 시작 화면 Brand Portal 사용 액세스 권한을 부여하려면 captcha 보안 검사를 입력합니다.

![](assets/bp-login-screen.png)

## 게스트 세션 기간 {#guest-session-duration}


게스트 사용자 세션이 15분 동안 활성 상태로 유지됩니다.
즉, **[!UICONTROL Lightbox]**&#x200B;의 상태는 세션 시작 시간부터 15분 동안 유지되며, 현재 게스트 세션이 다시 시작된 후에는 Lightbox 상태가 손실됩니다.

예를 들어 게스트 사용자가 1500시간에 Brand Portal에 로그인하고 15:05시간에 다운로드하도록 **[!UICONTROL Lightbox]**&#x200B;에 자산을 추가합니다. 사용자가 15:15시간(로그인 시 15분 이내) 전에 **[!UICONTROL Lightbox]** 컬렉션(또는 해당 자산)을 다운로드하지 않으면 세션을 다시 시작해야 합니다. **[!UICONTROL Lightbox]**&#x200B;가 비어 있으면 세션이 손실된 경우 업로드된 자산을 더 이상 사용할 수 없습니다.

## 동시 게스트 세션 허용 {#concurrent-guest-sessions-allowed}

동시 게스트 세션 수는 조직당 총 사용자 할당량의 10%로 제한됩니다. 즉, 사용자 할당량이 200명인 조직의 경우 최대 20명의 게스트 사용자가 동시에 작업할 수 있습니다. 21번째 사용자는 액세스가 거부되며 20명의 활성 게스트 사용자의 세션이 종료되는 경우에만 게스트로 액세스할 수 있습니다.

## Brand Portal과의 게스트 사용자 상호 작용 {#guest-user-interaction-with-brand-portal}

### 게스트 UI 탐색

Brand Portal을 게스트로 입력하면 사용자가 [에 공유된 모든 자산 및 폴더(](../using/brand-portal-sharing-folders.md#sharefolders))를 공개적 또는 게스트 사용자만 사용할 수 있습니다. 이 보기는 카드, 목록 또는 열 레이아웃 중 하나에 자산을 표시하는 컨텐츠 전용 보기입니다.

![](assets/disabled-folder-hierarchy1.png)

그러나 Guest 사용자는 관리자가 [폴더 계층 구조 활성화](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) 구성을 활성화한 경우 Brand Portal에 로그인하면 폴더 트리(루트 폴더부터 시작)와 각 상위 폴더 내에 배치된 공유 폴더가 표시됩니다.

이러한 상위 폴더는 가상 폴더이며, 가상 폴더에 대해 작업을 수행할 수 없습니다. 잠금 아이콘을 사용하여 이러한 가상 폴더를 인식할 수 있습니다.

공유 폴더와 달리 **[!UICONTROL 카드 보기]**&#x200B;에서 작업을 선택하거나 마우스로 선택할 때 작업 작업이 표시되지 않습니다. **** 열 보기 및 목록 보기에서 가상 폴더를 선택할 때  **[!UICONTROL 개요]** 단추 **[!UICONTROL 가 표시됩니다]**.

>[!NOTE]
>
>가상 폴더의 기본 축소판은 첫 번째 공유 폴더의 축소판 이미지입니다.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

**[!UICONTROL 보기]** 설정 옵션을 사용하면 게스트 사용자가 카드 보기 또는 열 **[!UICONTROL 에서]** 목록 보기에 표시할 카드 크기 **[!UICONTROL 를 조정할 수 있습니다]**.

![](assets/nav-guest-user.png)

**[!UICONTROL 컨텐츠 트리]**&#x200B;를 사용하면 자산 계층 구조를 통해 이동할 수 있습니다.

![](assets/guest-login-ui.png)

Brand Portal은 게스트 사용자에게 선택한 자산/폴더의 **[!UICONTROL 자산 속성]**&#x200B;을 볼 수 있는 **[!UICONTROL 개요]** 옵션을 제공합니다. **[!UICONTROL 개요]** 옵션이 표시됩니다.

* 자산/폴더 선택 시 맨 위의 도구 모음에서 를 클릭합니다.
* 드롭다운에서 레일 선택기 를 선택합니다.

자산/폴더를 선택하는 동안 **[!UICONTROL 개요]** 옵션을 선택할 때 사용자가 자산을 만든 제목, 경로 및 시간을 볼 수 있습니다. 반면에 자산 세부 사항 페이지에서 **[!UICONTROL 개요]** 옵션을 선택하면 자산의 메타데이터를 볼 수 있습니다.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

**** 왼쪽 레일의 탐색 옵션을 사용하면 파일에서 컬렉션으로 탐색하고 게스트 세션으로 다시 돌아와 사용자가 파일이나 컬렉션의 자산을 검색할 수 있습니다.

**** 필터 옵션을 사용하면 게스트 사용자가 관리자가 설정한 검색 설명을 사용하여 자산 파일과 폴더를 필터링할 수 있습니다.

### 게스트 사용자 기능

게스트 사용자는 Brand Portal에서 공개 자산에 액세스할 수 있으며, 추가로 설명된 대로 거의 제한 사항이 없습니다.

**게스트 사용자는 다음을 수행할 수** 있습니다.

* 모든 Brand Portal 사용자를 위한 모든 공용 폴더 및 컬렉션에 액세스합니다.
* 모든 공용 폴더 및 컬렉션의 구성원에 대한 전체 자산 보기를 사용하여 구성원, 세부 정보 페이지를 찾아봅니다.
* 공용 폴더 및 컬렉션에서 자산을 검색합니다.
* 라이트박스 컬렉션에 자산 추가 이러한 컬렉션 변경 사항은 세션 중에 유지됩니다.
* 자산을 직접 또는 Lightbox 컬렉션을 통해 다운로드합니다.

**게스트 사용자는 다음을 수행할 수 없습니다**.

* 컬렉션과 저장된 검색을 만들거나 더 많이 공유할 수 있습니다.
* 폴더 및 컬렉션 설정에 액세스합니다.
* 자산을 링크로 공유.

### 게스트 세션에서 자산 다운로드

게스트 사용자는 Brand Portal에서 공유되거나 게스트 사용자와 독점적으로 공유된 자산을 직접 다운로드할 수 있습니다. 게스트 사용자는 또한 **[!UICONTROL Lightbox]**(공개 컬렉션)에 자산을 추가하고, 세션이 만료되기 전에 **[!UICONTROL Lightbox]** 컬렉션을 다운로드할 수 있습니다.

자산 및 컬렉션을 다운로드하려면 다음 위치에서 다운로드 아이콘을 사용하십시오.

* 자산 또는 컬렉션 위로 마우스를 가져가면 표시되는 빠른 작업 축소판
* 자산 또는 컬렉션을 선택할 때 표시되는 맨 위의 도구 모음

![](assets/download-on-guest.png)

**[!UICONTROL 다운로드] 대화 상자에서 [!UICONTROL 다운로드 가속화]**&#x200B;를 선택하면 [다운로드 성능을 향상시킬 수 있습니다](../using/accelerated-download.md).

## 종료 게스트 세션 {#exit-guest-session}

게스트 세션을 종료하려면 헤더에서 사용할 수 있는 옵션에서 **[!UICONTROL 종료 세션]**&#x200B;을 사용하십시오. 그러나 게스트 세션에 사용된 브라우저 탭이 비활성 상태인 경우 2시간 동안 활동이 없으면 세션이 자동으로 만료됩니다.

![](assets/end-guest-session.png)

## 게스트 사용자 활동 모니터링 {#monitoring-guest-user-activities}

관리자는 Brand Portal와의 게스트 사용자 상호 작용을 모니터링할 수 있습니다. Brand Portal에서 생성된 보고서는 게스트 사용자 활동에 대한 주요 통찰력을 제공할 수 있습니다. 예를 들어 **[!UICONTROL 다운로드]** 보고서를 사용하여 게스트 사용자가 다운로드한 자산의 수를 추적할 수 있습니다. **[!UICONTROL 사용자]** 로그인 보고서는 Guest 사용자가 마지막으로 포털에 로그인한 시점과 지정된 기간 동안의 로그인 빈도를 알려줄 수 있습니다.
