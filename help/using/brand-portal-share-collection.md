---
title: 컬렉션 공유
seo-title: 컬렉션 공유
description: AEM Assets 브랜드 포털 관리자는 컬렉션 또는 스마트 컬렉션을 권한이 있는 사용자와 공유 및 공유 해제할 수 있습니다. 편집자는 자신이 만든 컬렉션, 공유된 컬렉션 및 공개 컬렉션만 보고 공유할 수 있습니다.
seo-description: AEM Assets 브랜드 포털 관리자는 컬렉션 또는 스마트 컬렉션을 권한이 있는 사용자와 공유 및 공유 해제할 수 있습니다. 편집자는 자신이 만든 컬렉션, 공유된 컬렉션 및 공개 컬렉션만 보고 공유할 수 있습니다.
uuid: 965f39cd-1378-42c1-a58a-01e1bf825aa3
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f053013e-5981-419f-927e-b5bb1d47eae2
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 2%

---


# 브랜드 포털에서 컬렉션 공유 {#share-collections-bp}

AEM Assets 브랜드 포털 관리자는 컬렉션 또는 스마트 컬렉션을 권한이 있는 사용자와 공유 및 공유 해제할 수 있습니다. 편집자는 자신이 만든 컬렉션, 공유된 컬렉션 및 공개 컬렉션만 보고 공유할 수 있습니다. 그러나 편집자는 공개 컬렉션을 비공개 컬렉션으로 변경할 수 없습니다.

>[!NOTE]
>
>편집자는 공개 컬렉션을 비공개 컬렉션으로 변경할 수 없으므로 **[!UICONTROL 컬렉션 설정 대화 상자에서 공개 컬렉션]** 확인란을 사용할 수 **[!UICONTROL 없습니다]** .

## 컬렉션 공유 {#share-collection}

컬렉션을 공유하려면 다음 단계를 따르십시오.

1. 왼쪽의 오버레이 아이콘을 클릭하고 [탐색]을 **[!UICONTROL 선택합니다]**.

   ![](assets/contenttree-1.png)

1. 왼쪽에 있는 사이드레이어에서 **[!UICONTROL 컬렉션을 클릭합니다]**.

   ![](assets/access_collections.png)

1. 컬렉션 **[!UICONTROL 콘솔에서]** 다음 중 하나를 수행합니다.

   * 공유할 컬렉션 위로 포인터를 가져갑니다. 컬렉션에 사용할 수 있는 빠른 작업 축소판에서 **[!UICONTROL 설정]** 아이콘을 클릭합니다.

   ![](assets/settings_thumbnail.png)

   * 공유할 컬렉션을 선택합니다. 상단에 있는 도구 모음에서 **[!UICONTROL 설정을 클릭합니다]**.

   ![](assets/collection-sharing.png)

1. 컬렉션 [!UICONTROL 설정] 대화 상자에서 컬렉션을 공유할 사용자나 그룹을 선택하고 해당 사용자 또는 그룹의 전역 역할과 일치하는 역할을 선택합니다. 예를 들어 전역 편집기에 편집기 역할을 지정하고 전역 뷰어에 뷰어 역할을 지정합니다.

   또는 그룹 멤버십과 역할에 관계없이 모든 사용자가 컬렉션을 사용할 수 있게 하려면 **[!UICONTROL 공개 컬렉션]** 확인란을 선택하여 공개하십시오.

   >[!NOTE]
   >
   >하지만 시스템 공간을 저장할 수 있도록 관리자가 아닌 사용자는 공개 컬렉션을 만들 수 없도록 제한할 수 있습니다. 조직은 관리 도구 패널에서 사용 가능한 **[!UICONTROL 일반]** 설정에서 공개 컬렉션 제작  허용 구성을 비활성화할 수 있습니다.

   ![](assets/collection_sharingadduser.png)

   편집자는 공개 컬렉션을 비공개 컬렉션으로 변경할 수 없으므로 **[!UICONTROL 컬렉션 설정 대화 상자에서 공개 컬렉션]** 확인란을 사용할 수 **[!UICONTROL 없습니다]** .

   ![](assets/collection-setting-editor.png)

1. 추가 **[!UICONTROL 를]**&#x200B;선택한 다음 **[!UICONTROL 저장을 선택합니다]**. 컬렉션은 선택한 사용자와 공유됩니다.

   >[!NOTE]
   >
   >사용자 역할은 컬렉션 내의 자산 및 폴더에 대한 액세스를 관리합니다. 사용자에게 자산에 대한 액세스 권한이 없는 경우 빈 컬렉션은 사용자와 공유됩니다. 또한 사용자의 역할은 컬렉션에 사용할 수 있는 작업에 적용됩니다.

## 컬렉션 공유 취소 {#unshare-a-collection}

이전에 공유한 컬렉션의 공유를 취소하려면 다음을 수행하십시오.

1. 컬렉션 **[!UICONTROL 콘솔에서]** 공유를 취소할 컬렉션을 선택합니다.

   도구 모음에서 **[!UICONTROL 설정을 클릭합니다]**.

   ![](assets/collection_settings.png)

1. 컬렉션 **[!UICONTROL 설정]** 대화 상자의 **[!UICONTROL 멤버]**&#x200B;아래에서 사용자 또는 그룹 옆에 있는 **[!UICONTROL x]** 기호를 클릭하여 컬렉션을 공유한 사용자 목록에서 제거합니다.

   ![](assets/unshare_collection.png)

1. 경고 메시지 상자에서 **[!UICONTROL 확인을]** 클릭하여 공유 해제를 확인합니다.

   **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

1. 공유 목록에서 제거한 사용자의 자격 증명으로 브랜드 포털에 로그인합니다. 컬렉션이 **[!UICONTROL 컬렉션]** 콘솔에서 제거됩니다.
