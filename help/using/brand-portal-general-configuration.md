---
title: 관리자 일반 테넌트 구성
description: 다운로드 가속화, 공용 스마트 컬렉션 만들기, 공용 컬렉션 만들기를 구성하고 관리자가 테넌트의 자산을 삭제할 수 있도록 합니다.
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
role: Admin
exl-id: 5607be8e-0a7f-4692-b71b-5f66eb9ac5ee
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# 관리자 일반 테넌트 구성 {#administer-general-tenant-configurations}

Experience Manager Assets Brand Portal을 통해 조직에서는 특정 테넌트에 대해 다음 기능을 구성할 수 있습니다.

* 관리자가 에셋을 삭제하는 방법
* 관리자가 아닌 사용자에 의한 공개 컬렉션 만들기
* 관리자가 아닌 사용자에 의한 공용 스마트 컬렉션 만들기
* 공유 폴더의 상위 계층은 관리자가 아닌 사용자에게 표시됩니다

이러한 구성은 관리 도구 패널에서 **[!UICONTROL 일반 설정]** 구성으로 제공됩니다.

![](assets/general-config.png)

**A** - 관리자가 Brand Portal에서 에셋을 삭제할 수 있도록 하는 구성입니다. (기본값은 활성화됨)

**B** - 관리자가 아닌 사용자가 공용 컬렉션을 만들 수 있도록 하는 구성입니다. (기본값은 활성화됨)

**C** - 관리자가 아닌 사용자가 공용 스마트 컬렉션을 만들 수 있도록 하는 구성입니다. (기본값은 활성화됨)

**D** - 공유 폴더의 폴더 계층 구조(루트에서)를 관리자가 아닌 사용자(편집자, 뷰어, 게스트 사용자)에게 표시하는 구성입니다. (기본값은 비활성화됨)

## 일반 구성 활성화 또는 비활성화 {#enable-disable-general-configurations}

이러한 각 구성을 활성화하거나 비활성화하려면 다음 작업을 수행하십시오.

1. 관리자 권한으로 로그인합니다.
1. 상단의 도구 모음에서 Experience Manager 로고를 선택하여 관리 도구에 액세스합니다.
1. 관리 도구 패널에서 **[!UICONTROL 일반]**&#x200B;을 선택하여 **[!UICONTROL 일반 설정]** 페이지를 엽니다.
1. 각 토글 스위치를 사용하여 일반 구성을 활성화 또는 비활성화합니다.
1. 변경 내용을 **[!UICONTROL 저장]**&#x200B;합니다.
1. 변경 사항이 적용되도록 로그아웃합니다.

## 관리자 사용자가 Brand Portal에서 에셋을 삭제하도록 허용 {#allow-admin-users-to-delete-assets-from-brand-portal}

**[!UICONTROL 사용자 삭제 허용]** 구성을 사용하면 관리자 권한이 있는 사용자가 Brand Portal에서 에셋 및 폴더를 삭제할 수 있도록 허용(또는 제한)할 수 있습니다.

## 관리자가 아닌 사용자가 공용 컬렉션을 만들 수 있음 {#allow-public-collections-creation-by-non-admins}

[[!UICONTROL 공개 컬렉션 만들기 허용]](../using/brand-portal-share-collection.md#main-pars-text-1915052376) 구성은 관리자가 아닌 사용자가 Brand Portal에서 공개 컬렉션을 만들 수 있는지 여부를 제어합니다. 구성은 기본적으로 활성화되어 있습니다. 구성을 비활성화하면 조직은 포털에 많은 공개 컬렉션이 없는 것을 방지하여 시스템 공간을 절약할 수 있습니다.

## 관리자가 아닌 사용자가 공용 스마트 컬렉션을 만들 수 있도록 허용 {#allow-public-smart-collections-creation-by-non-admins}

[[!UICONTROL 공용 스마트 컬렉션 만들기 허용]](../using/brand-portal-searching.md#main-pars-header-500620467) 구성은 관리자가 아닌 사용자가 검색을 스마트 컬렉션으로 저장하고 해당 테넌트에 대해 공개로 설정할 수 있는지 여부를 제어합니다. 구성은 기본적으로 활성화되어 있습니다. 구성을 비활성화하면 조직은 조직의 Brand Portal에서 관리자가 아닌 사용자가 만든 공용 스마트 컬렉션을 너무 많이 사용하지 못하게 될 수 있습니다.

<!-- 
## Allow download acceleration {#allow-download-acceleration}

[[!UICONTROL Allow download acceleration]](../using/accelerated-download.md) configuration lets the organizations to allow accelerated downloads of assets from Brand Portal and shared links, by integrating with IBM Aspera Connect that is an install-on-demand application. The application uses proprietary technology to remove TCP overheads.
-->

## 폴더 계층 구조 사용 {#enable-folder-hierarchy}

[[!UICONTROL 폴더 계층 구조 사용]](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) 구성을 통해 관리자는 관리자가 아닌 사용자(편집자, 뷰어 및 게스트 사용자)가 로그인 후 공유 폴더를 보는 방법을 제어할 수 있습니다.
