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
source-git-commit: ea7fdd2df0696ed309227fa77e3f79d0141bcb58

---


# 일반 임차인 구성 관리 {#administer-general-tenant-configurations}

[!DNL AEM] 자산은 [!DNL Brand Portal] 조직이 특정 임차인에 대해 다음 기능을 구성할 수 있도록 해줍니다.

* 관리자별 자산 삭제
* 관리자가 아닌 사용자도 [!UICONTROL 공개 컬렉션] 작성
* 관리자가 아닌 사용자의 공개 스마트 [!UICONTROL 컬렉션] 작성
* 다운로드 가속화
* 관리자가 아닌 사용자에게 표시되는 공유 폴더의 상위 계층 구조

이러한 구성은 관리 도구 패널에서 **일반 설정** 구성으로 제공됩니다.

![](assets/general-configs.png)

**관리자가 자산을 삭제할 수 있도록 하는** 구성 [!DNL Brand Portal]. (기본값이 활성화되어 있음)

**b** 구성을 참조하십시오. (기본값이 활성화되어 있음)

**C** 구성을 참조하십시오. (기본값이 활성화되어 있음)

**d** 구성을 참조하십시오. (기본값은 비활성화됨)

**공유 폴더의 폴더 계층 구조를 관리자가 아닌 사용자 (편집자, 뷰어, 손님 사용자) 에게 보여주는 전자** 구성입니다. (기본값은 비활성화됨)

## 일반 구성 활성화/비활성화 {#enable-disable-general-configurations}

이러한 각 구성을 활성화/비활성화하려면:

1. 관리자 권한으로 로그인합니다.
2. 맨 위의 도구 모음에서 관리 도구에 액세스하려면 [!DNL AEM] 로고를 선택합니다.
3. 관리 도구 패널에서 **일반을 선택하여** **일반 설정** 페이지를 엽니다.
4. 각 전환 스위치를 사용하여 일반 구성을 활성화/비활성화합니다.
5. **변경 사항을 저장합니다.**
6. 로그아웃하면 변경 사항이 적용됩니다.

## 관리 사용자가 자산을 [!DNL Brand Portal]{#allow-admin-users-to-delete-assets-from-brand-portal}

**사용자가 구성을 삭제하도록** 허용하면 조직에서 관리자 권한이 있는 사용자를 허용 (또는 제한) 하여 자산과 폴더를 삭제할 [!DNL Brand Portal]수 있습니다.

## 관리자가 아닌 사람이 공개 컬렉션 작성 허용 {#allow-public-collections-creation-by-non-admins}

[공개 [!UICONTROL 컬렉션]작성 허용] (../using/brand-portal-share-[!UICONTROL collection]. md # main-pars-text -1915052376) 관리자가 아닌 사람이 [!UICONTROL 공개 컬렉션을]만들 [!DNL Brand Portal]수 있는지 여부를 제어합니다. 구성은 기본적으로 활성화되어 있습니다. 구성 조직을 비활성화하면 시스템 공간을 저장할 수 있도록 포털에 많은 [!UICONTROL 공개 컬렉션이]있을 수 없습니다.

## 관리자가 아닌 사용자도 공개 스마트 컬렉션 작성 허용 {#allow-public-smart-collections-creation-by-non-admins}

[공개 스마트 컬렉션 작성 허용](../using/brand-portal-searching.md#main-pars-header-500620467) 구성을 사용하면 관리자가 아닌 사용자가 스마트 [!UICONTROL 컬렉션으로] 검색을 저장하고 해당 임차인에 대해 공개할 수 있는지 여부를 지정할 수 있습니다. 구성은 기본적으로 활성화되어 있습니다. 구성을 비활성화하면 조직의 관리자가 아닌 사용자가 만든 대량의 공개 스마트 [!UICONTROL 컬렉션이] 없을 [!DNL Brand Portal]수 있습니다.

## 다운로드 가속화 허용 {#allow-download-acceleration}

[다운로드 가속화](../using/accelerated-download.md) [!DNL Brand Portal] 구성을 허용합니다. 애플리케이션은 독점적 기술을 사용하여 TCP 오버헤드를 제거합니다.

## 폴더 계층 구조 사용 {#enable-folder-hierarchy}

[폴더 계층](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) 구조 구성을 활성화하면 관리자가 관리자가 아닌 사용자 (편집자, 뷰어 및 게스트 사용자) 가 로그인 후 공유 폴더를 보는 방법을 제어할 수 있습니다.
