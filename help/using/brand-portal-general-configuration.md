---
title: 일반 테넌트 구성 관리
seo-title: 일반 테넌트 구성 관리
description: 다운로드 가속화 구성, 공개 스마트 [!UICONTROL 컬렉션] 만들기, 공개 [!UICONTROL 컬렉션] 만들기, 관리 사용자가 테넌트의 자산을 삭제할 수 있도록 합니다.
seo-description: 다운로드 가속화 구성, 공개 스마트 [!UICONTROL 컬렉션] 만들기, 공개 [!UICONTROL 컬렉션] 만들기, 관리 사용자가 테넌트의 자산을 삭제할 수 있도록 합니다.
uuid: 3c46cd7c-c38b-4bc7-b566-93f977bc8227
contentOwner: 밀라티
topic-tags: 관리
content-type: 참조
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f4c237bc-f6a4-4bc4-af56-3d9c3027daf4
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 일반 테넌트 구성 관리 {#administer-general-tenant-configurations}

AEM Assets 브랜드 포털을 통해 조직은 특정 테넌트에 대해 다음 기능을 구성할 수 있습니다.

* 관리자의 자산 삭제
* 관리자가 아닌 사용자에 의한 공개 컬렉션 제작
* 관리자가 아닌 사용자에 의한 공개 스마트 컬렉션 제작
* 다운로드 가속
* 관리자가 아닌 사용자가 볼 수 있는 공유 폴더의 상위 계층

이러한 구성은 관리 도구 **[!UICONTROL 패널에서 일반]** 설정 구성으로 제공되었습니다.

![](assets/general-configs.png)

**관리자가** 브랜드 포털에서 자산을 삭제할 수 있도록 허용하는 구성. (기본값은 활성화됨)

**B** 구성 - 관리자가 아닌 사용자가 공개 컬렉션을 만들 수 있도록 허용합니다. (기본값은 활성화됨)

**C** 관리자가 아닌 사용자가 공개 스마트 컬렉션을 만들 수 있도록 하는 구성. (기본값은 활성화됨)

**D** 구성 - 포털과 공유 링크에서 다운로드한 에셋의 다운로드 가속화를 허용합니다. (기본값은 비활성화됨)

**e** 루트 폴더에서 비관리 사용자(편집기, 뷰어, 게스트 사용자)로 폴더 계층 구조를 표시하는 구성 (기본값은 비활성화됨)

## 일반 구성 활성화/비활성화 {#enable-disable-general-configurations}

이러한 각 구성을 활성화/비활성화하려면:

1. 관리자 권한으로 로그인합니다.
2. 맨 위의 도구 모음에서 관리 도구에 액세스하려면 AEM 로고를 선택합니다.
3. 관리 도구 패널에서 일반을 선택하여 **[!UICONTROL 일반]** 설정 **[!UICONTROL 페이지를 엽니다]** .
4. 각 전환 스위치를 사용하여 일반 구성을 활성화/비활성화합니다.
5. **[!UICONTROL 변경 사항을 저장합니다.]**
6. 로그아웃하여 변경 사항을 적용합니다.

## 관리자 사용자가 브랜드 포털에서 자산을 삭제하도록 허용 {#allow-admin-users-to-delete-assets-from-brand-portal}

**[!UICONTROL 사용자가 구성을 삭제하도록]** 허용하면 조직은 관리자 권한이 있는 사용자가 브랜드 포털에서 자산 및 폴더를 삭제하도록 허용(또는 제한)할 수 있습니다.

## 관리자가 아닌 사람이 공개 컬렉션 제작 허용 {#allow-public-collections-creation-by-non-admins}

[[!UICONTROL 공개 컬렉션 제작 허용]](../using/brand-portal-share-collection.md#main-pars-text-1915052376) 구성은 관리자가 아닌 사용자가 브랜드 포털에서 공개 컬렉션을 만들 수 있는지 여부를 제어합니다. 기본적으로 구성이 활성화됩니다. 구성 조직을 비활성화하면 시스템 공간을 저장할 수 있도록 포털에 수많은 공개 컬렉션이 표시되지 않을 수 있습니다.

## 관리자가 아닌 사람이 공용 스마트 컬렉션 제작 허용 {#allow-public-smart-collections-creation-by-non-admins}

[[!UICONTROL 공개 스마트 컬렉션 생성 허용]](../using/brand-portal-searching.md#main-pars-header-500620467) 구성은 관리자가 아닌 사용자가 자신의 검색을 스마트 컬렉션으로 저장하고 해당 테넌트에 대해 공개할 수 있는지 여부를 제어합니다. 기본적으로 구성이 활성화됩니다. 구성 조직을 비활성화하면 조직의 브랜드 포털에서 관리자가 아닌 사용자가 만든 많은 수의 공개 스마트 컬렉션이 만들어지지 않을 수 있습니다.

## 다운로드 가속 허용 {#allow-download-acceleration}

[[!UICONTROL 다운로드 가속 허용]](../using/accelerated-download.md) 구성을 사용하면 조직은 주문형 설치 애플리케이션인 IBM Aspera Connect와 통합하여 브랜드 포털에서 에셋을 신속하게 다운로드하고 공유 링크를 다운로드할 수 있습니다. 이 애플리케이션은 전용 기술을 사용하여 TCP 오버헤드를 제거합니다.

## 폴더 계층 구조 사용 {#enable-folder-hierarchy}

[[!UICONTROL 폴더 계층 구조 활성화]](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) 구성을 사용하면 관리자가 비관리 사용자(편집기, 뷰어 및 게스트 사용자)가 로그인 후 공유 폴더를 보는 방법을 제어할 수 있습니다.
