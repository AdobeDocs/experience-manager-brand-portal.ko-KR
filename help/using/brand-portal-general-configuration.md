---
title: 일반 임차인 구성 관리
seo-title: 일반 임차인 구성 관리
description: 다운로드 가속화, 공개 스마트 [! Uicontrol Collection] 제작, 공개 [! Uicontrol 컬렉션] 작성 시 관리 사용자가 테넌트에서 자산을 삭제할 수 있습니다.
seo-description: 다운로드 가속화, 공개 스마트 [! Uicontrol Collection] 제작, 공개 [! Uicontrol 컬렉션] 작성 시 관리 사용자가 테넌트에서 자산을 삭제할 수 있습니다.
uuid: 3 C 46 CD 7 C-C 38 B -4 BC 7-B 566-93 F 977 BC 8227
contentOwner: Mgulati
topic-tags: 관리
content-type: 참조
products: sg_ Experiencemanager/brand_ portal
discoiquuid: f 4 c 237 bc-f 6 a 4-4 bc 4-af 56-3 d 9 c 3027 daf 4
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 일반 임차인 구성 관리 {#administer-general-tenant-configurations}

조직에서는 AEM Assets 브랜드 포털을 사용하여 특정 임차인에 대해 다음 기능을 구성할 수 있습니다.

* 관리자별 자산 삭제
* 관리자가 아닌 사용자도 공개 컬렉션 작성
* 관리자가 아닌 사용자의 공개 스마트 컬렉션 작성
* 다운로드 가속화
* 관리자가 아닌 사용자에게 표시되는 공유 폴더의 상위 계층 구조

이러한 구성은 관리 도구 패널에서 **[!UICONTROL 일반 설정]** 구성으로 제공됩니다.

![](assets/general-configs.png)

**관리자가 브랜드 포털에서 자산을 삭제할 수 있도록** 하는 구성. (기본값이 활성화되어 있음)

**b** 구성을 참조하십시오. (기본값이 활성화되어 있음)

**C** 구성을 참조하십시오. (기본값이 활성화되어 있음)

**d** 구성을 참조하십시오. (기본값은 비활성화됨)

**공유 폴더의 폴더 계층 구조를 관리자가 아닌 사용자 (편집자, 뷰어, 손님 사용자) 에게 보여주는 전자** 구성입니다. (기본값은 비활성화됨)

## 일반 구성 활성화/비활성화 {#enable-disable-general-configurations}

이러한 각 구성을 활성화/비활성화하려면:

1. 관리자 권한으로 로그인합니다.
2. 맨 위의 도구 모음에서 관리 도구에 액세스하려면 AEM 로고를 선택합니다.
3. 관리 도구 패널에서 **[!UICONTROL 일반을 선택하여]** **[!UICONTROL 일반 설정]** 페이지를 엽니다.
4. 각 전환 스위치를 사용하여 일반 구성을 활성화/비활성화합니다.
5. **[!UICONTROL 변경 사항을 저장합니다.]**
6. 로그아웃하면 변경 사항이 적용됩니다.

## 관리 사용자가 브랜드 포털에서 에셋을 삭제할 수 있도록 허용 {#allow-admin-users-to-delete-assets-from-brand-portal}

**[!UICONTROL 조직에서는 구성을 Delet]** 로 허용하여 조직에서 관리자 권한으로 사용자를 허용하거나 제한하여 브랜드 포털에서 자산과 폴더를 삭제할 수 있습니다.

## 관리자가 아닌 사람이 공개 컬렉션 작성 허용 {#allow-public-collections-creation-by-non-admins}

[[! Uicontrol 공개 컬렉션 작성 허용]](../using/brand-portal-share-collection.md#main-pars-text-1915052376) 구성이 아닌 경우 관리자가 브랜드 포털에서 공개 컬렉션을 만들 수 있는지 여부를 제어합니다. 구성은 기본적으로 활성화되어 있습니다. 구성 조직을 비활성화하면 시스템 공간을 저장할 수 있도록 포털에 많은 공개 컬렉션이 있을 수 없습니다.

## 관리자가 아닌 사용자도 공개 스마트 컬렉션 작성 허용 {#allow-public-smart-collections-creation-by-non-admins}

[[! Uicontrol 공개 스마트 컬렉션 작성 허용]](../using/brand-portal-searching.md#main-pars-header-500620467) 구성을 사용하면 관리자가 아닌 사용자가 스마트 컬렉션으로 검색을 저장하고 해당 임차인에 대해 공개할 수 있는지 여부를 지정할 수 있습니다. 구성은 기본적으로 활성화되어 있습니다. 구성을 비활성화하면 조직의 브랜드 포털에서 관리자가 아닌 사용자가 만든 대량의 공개 스마트 컬렉션이 없을 수 있습니다.

## 다운로드 가속화 허용 {#allow-download-acceleration}

[[! Uicontrol를 사용하면 다운로드 가속화 기능을 사용할 수 있습니다](../using/accelerated-download.md) . 애플리케이션은 독점적 기술을 사용하여 TCP 오버헤드를 제거합니다.

## 폴더 계층 구조 사용 {#enable-folder-hierarchy}

[[! Uicontrol의 폴더 계층 활성화]](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) 구성을 사용하면 관리자가 관리자가 아닌 사용자 (편집자, 뷰어 및 게스트 사용자) 가 로그인 후 공유 폴더를 보는 방법을 제어할 수 있습니다.
