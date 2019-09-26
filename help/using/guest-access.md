---
title: 브랜드 포털에 대한 게스트 액세스
seo-title: 브랜드 포털에 대한 게스트 액세스
description: 게스트 액세스 허용 및 인증을 받을 필요가 없는 수많은 사용자가 참가할 수 있도록 비용을 절감할 수 있습니다.
seo-description: 게스트 액세스 허용 및 인증을 받을 필요가 없는 수많은 사용자가 참가할 수 있도록 비용을 절감할 수 있습니다.
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: 밀라티
topic-tags: 소개
content-type: 참조
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
translation-type: tm+mt
source-git-commit: 9763a57a83db22cd6686701dcbd8fcde16bcbb31

---


# 브랜드 포털에 대한 게스트 액세스 {#guest-access-to-brand-portal}

AEM 브랜드 포털을 통해 고객이 포털에 액세스할 수 있습니다. 손님 사용자는 포털에 입장할 자격 증명이 필요하지 않으며 포털의 공개 자산(및 컬렉션)에 액세스할 수 있습니다. 게스트 세션의 사용자는 Lightbox(비공개 컬렉션)에 에셋을 추가하고 게스트 사용자가 [[!UICONTROL End Session]을 선택하지 않는 한 세션이 끝날 때까지 동일한 에셋을 다운로드할 수 있습니다](#exit-guest-session).

게스트 액세스 기능을 통해 조직은 승인된 자산을 [](../using/brand-portal-sharing-folders.md#how-to-share-folders) 도입 없이 규모에 맞게 대상 고객과 신속하게 공유할 수 있습니다. Brand Portal 6.4.2 버전부터는 여러 명의 동시 게스트 사용자를 지원할 수 있습니다. 이는 조직당 총 사용자 할당량의 10%입니다. 게스트 액세스를 허용하면 브랜드 포털에서 제한된 기능을 사용해야 하는 많은 사용자와 관리에 소요되는 시간을 절약할 수 있습니다.\
조직은 관리 도구 패널의 액세스 설정에서 손님 액세스 허용 옵션을 사용하여 조직의 브랜드 포털 계정에서 손님 액세스를 활성화(또는 비활성화) **** **[!UICONTROL 할]** 수있습니다.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## 손님 세션 시작 {#begin-guest-session}

익명으로 브랜드 포털에 들어가려면 **[!UICONTROL 손님 액세스에 해당하는 여기를]** 클릭 **[!UICONTROL 옵션을 선택하십시오.]** 브랜드 포털 시작 화면 사용자는 액세스 권한을 요청하고 관리자가 인증 권한을 부여하여 브랜드 포털 사용을 기다릴 필요가 없습니다.

![](assets/bp-login-screen.png)

## 게스트 세션 기간 {#guest-session-duration}

게스트 사용자 세션은 2시간 동안 활성 상태로 유지됩니다. 즉, Lightbox의 상태는 세션 시작 [!UICONTROL 시간으로부터] 1시간, 2시간 후 현재 게스트 세션이 다시 시작되어 Lightbox 상태가 손실됩니다.\
예를 들어 게스트 사용자는 1500시간에 브랜드 포털에 로그인하고 16:50시간에 다운로드할 수 있도록 Lightbox에 자산을 추가합니다. 사용자가 17:00 [!UICONTROL 시간 전에 Lightbox] 컬렉션(또는 해당 에셋)을 [!UICONTROL 다운로드하지 않으면] 사용자가 1시간(1700시간)이 끝날 때 세션을 다시 시작해야 하므로 Lightbox는 비어 있게 됩니다.

## 동시 손님 세션 허용됨 {#concurrent-guest-sessions-allowed}

동시 손님 세션 수는 조직당 총 사용자 할당량의 10%로 제한됩니다. 이는 사용자 할당량이 200명인 조직의 경우 최대 20명의 게스트 사용자가 동시에 작업할 수 있음을 의미합니다. 21번째 사용자는 액세스가 거부되며 20명의 활성 게스트 사용자의 세션이 종료되는 경우에만 손님으로 액세스할 수 있습니다.

## 브랜드 포털과의 게스트 사용자 인터랙션 {#guest-user-interaction-with-brand-portal}

### 게스트 UI 탐색

손님으로 브랜드 포털에 입장할 때, 사용자는 공개적으로 공유되거나 손님 사용자만 [공유하는](../using/brand-portal-sharing-folders.md#sharefolders) 모든 자산과 폴더를 볼 수 있습니다. 이 보기는 카드, 목록 또는 열 레이아웃 중 하나에 자산을 표시하는 컨텐츠 전용 보기입니다.

![](assets/disabled-folder-hierarchy1.png)

하지만, 관리자가 폴더 계층 구성 활성화를 활성화한 경우 게스트 사용자는 폴더 트리(루트 폴더에서 시작)와 브랜드 포털에 로그인할 때 각각의 상위 폴더 내에 배열된 공유 [폴더를 볼 수](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) 있습니다.

이러한 상위 폴더는 가상 폴더이며, 가상 폴더에 대해 작업을 수행할 수 없습니다. 이러한 가상 폴더는 잠금 아이콘을 사용하여 인식할 수 있습니다.

공유 폴더와 달리 카드 보기에서 마우스로 가리키거나 선택할 [!UICONTROL 때]작업 작업을 볼 수 없습니다. [!UICONTROL [개요] ] 단추는 [열 보기] 및 [목록 보기]에서 가상 [!UICONTROL 폴더를] 선택할 때 [!UICONTROL 표시됩니다].

>[!NOTE]
>
>가상 폴더의 기본 축소판은 첫 번째 공유 폴더의 축소판 이미지입니다.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

[!UICONTROL [설정] 보기] 옵션을 사용하면 손님 사용자가 [카드 보기]에서 카드 크기를 조정하거나 [ [!UICONTROL 목록 보기] ]에 표시할 열을 조정할 [!UICONTROL 수]있습니다.

![](assets/nav-guest-user.png)

컨텐츠 [!UICONTROL 트리를] 사용하면 자산 계층 구조에서 이동할 수 있습니다.

![](assets/guest-login-ui.png)

브랜드 포털에서는 게스트 [!UICONTROL 사용자가] 선택한 자산/폴더의 [!UICONTROL 자산] 속성을 볼 수 있는 개요 옵션을 제공합니다. 개요 [!UICONTROL 옵션은] 다음과 같습니다.

* 자산/폴더 선택 상단에 있는 도구 모음에서.
* 레일 선택기 선택 드롭다운에서

자산/ [!UICONTROL 폴더를] 선택한 동안 개요 옵션을 선택하면 제목, 경로 및 자산 생성 시간을 볼 수 있습니다. 반면에 자산 세부 사항 페이지에서 개요 [!UICONTROL 옵션을 선택하면] 사용자가 자산의 메타데이터를 볼 수 있습니다.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)<br />

**[!UICONTROL 왼쪽 레일의 탐색]** 옵션을 사용하면 파일에서 컬렉션으로 이동하고 게스트 세션에서 다시 탐색할 수 있으므로 사용자는 파일이나 컬렉션의 자산을 검색할 수 있습니다.

**[!UICONTROL 필터]** 옵션을 사용하면 게스트 사용자가 관리자가 설정한 검색 조건자를 사용하여 자산 파일과 폴더를 필터링할 수 있습니다.

### 게스트 사용자 기능

게스트 사용자는 브랜드 포털에서 공개 에셋에 액세스할 수 있으며, 이에 대한 추가 논의와 같이 제한된 사항도 거의 없습니다.

게스트 사용자는 다음을 수행할 수 있습니다.

* 모든 브랜드 포털 사용자에 대한 모든 공개 폴더 및 컬렉션에 액세스합니다.
* 검색 구성원, 세부 사항 페이지, 모든 공용 폴더 및 컬렉션의 구성원에 대한 전체 자산 보기 등이 있습니다.
* 공개 폴더 및 컬렉션에서 에셋을 검색할 수 있습니다.
* lightbox 컬렉션에 에셋 추가 컬렉션에 대한 이러한 변경 사항은 세션 중에 유지됩니다.
* 직접 또는 lightbox 컬렉션을 통해 에셋을 다운로드할 수 있습니다.

게스트 사용자는 다음을 수행할 수 없습니다.

* 컬렉션 및 저장된 검색을 만들거나 추가로 공유할 수 있습니다.
* 액세스 폴더 및 컬렉션 설정에 액세스할 수 있습니다.
* 에셋을 링크로 공유합니다.

### 게스트 세션에서 에셋 다운로드

게스트 사용자는 공개적으로 공유되거나 Brand Portal에서 손님 사용자와 단독으로 공유된 자산을 직접 다운로드할 수 있습니다. 게스트 사용자는 세션이 만료되기 전에 Lightbox [!UICONTROL (공개] 컬렉션)에 에셋을 추가하고 [!UICONTROL Lightbox] 컬렉션을 다운로드할 수도 있습니다.

자산 및 컬렉션을 다운로드하려면 다운로드 아이콘을 사용합니다.

* 에셋 또는 컬렉션 위에 마우스를 올려 놓을 때 표시되는 빠른 작업 축소판
* 맨 위에 있는 도구 모음 - 자산 또는 컬렉션 선택 시 표시됨

![](assets/download-on-guest.png)

다운로드 **[!UICONTROL 대화 상자에서 다운로드 가속]** 사용을 [!UICONTROL 선택하면] 다운로드 성능을 [향상시킬 수 있습니다](../using/accelerated-download.md).

## 게스트 세션 종료 {#exit-guest-session}

게스트 세션을 종료하려면 헤더에서 **[!UICONTROL 사용할]** 수 있는 옵션에서 세션 종료를 사용합니다. 그러나 게스트 세션에 사용된 브라우저 탭이 비활성 상태인 경우 2시간 동안 활동이 없는 경우 세션이 자동으로 만료됩니다.

![](assets/end-guest-session.png)

## 손님 사용자 활동 모니터링 {#monitoring-guest-user-activities}

관리자는 브랜드 포털과의 게스트 사용자 상호 작용을 모니터링할 수 있습니다. 브랜드 포털에서 생성된 보고서는 게스트 사용자 활동에 대한 주요 통찰력을 제공할 수 있습니다. 예를 들어 **[!UICONTROL 다운로드]** 보고서를 사용하여 게스트 사용자가 다운로드한 자산의 수를 추적할 수 있습니다. **[!UICONTROL 사용자 로그인]** 보고서는 게스트 사용자가 마지막으로 포털에 로그인한 날짜와 지정된 기간 동안 로그인 빈도를 알릴 수 있습니다.
