---
title: 컬렉션 공유
seo-title: Share a collection
description: Experience Manager Assets Brand Portal 관리자는 승인된 사용자와 컬렉션 또는 스마트 컬렉션을 공유하고 공유를 해제할 수 있습니다. 편집자는 자신이 만든 컬렉션, 공유 된 컬렉션 및 공용 컬렉션만 보고 공유할 수 있습니다.
seo-description: Experience Manager Assets Brand Portal Administrators can share and unshare a collection or a smart collection with authorized users. Editors can view and share only the collections created by them, shared with them, and public collections.
uuid: 965f39cd-1378-42c1-a58a-01e1bf825aa3
contentOwner: Vishabh Gupta
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f053013e-5981-419f-927e-b5bb1d47eae2
exl-id: 29b877f6-4200-4299-9b8d-81d88f4e8221
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 1%

---

# 컬렉션 공유 {#share-collections}

컬렉션은 Adobe Experience Manager Assets Brand Portal에 함께 저장된 관련 에셋 그룹을 나타냅니다. 사용자는 다음 방법으로 스마트 컬렉션을 만들 수 있습니다. [omnisearch 또는 facet 검색을 적용하여 관련 에셋 필터링](brand-portal-searching.md) 간편하게 액세스하고 다른 Brand Portal 사용자와 공유할 수 있도록 여러 파일을 함께 저장할 수 있습니다.

관리자는 권한이 부여 된 Brand Portal 사용자와 컬렉션를 공유 하 고 공유 안 함 수 있습니다. 편집자와 뷰어는 자신이 만든 컬렉션을 보고 공유 하 고, 공유 하 고, 공용 컬렉션을 공유할 수 있습니다.

>[!NOTE]
>
>편집자는 공용 컬렉션를 비공용 컬렉션으로 변경할 수 없으므로 컬렉션 설정 ]**대화 상자에서**[!UICONTROL  사용할 수 있는 공용 컬렉션 ]**확인란은**[!UICONTROL  없습니다.

## 컬렉션 공유 {#share-collection}

다음은 권한이 부여 된 Brand Portal 사용자와 컬렉션를 공유 하는 단계입니다.

1. Brand Portal 테 넌 트에 로그인 합니다. 기본적으로, **[!UICONTROL 게시 된 모든 자산 및 폴더를 포함 하는 파일]** 보기가 열립니다.

1. 맨 위에 있는 빠른 탐색에서 컬렉션 ]**을 클릭**[!UICONTROL  합니다.

1. 다음에서 **[!UICONTROL 컬렉션]** console에서 다음 중 하나를 수행합니다.

   * 공유할 컬렉션 위에 포인터를 놓습니다. 컬렉션에 사용할 수 있는 빠른 작업 썸네일에서 **[!UICONTROL 설정]** 아이콘.

      ![](assets/settings-icon.png)

   * 공유할 컬렉션을 선택하십시오. 맨 위에 있는 도구 모음에서 를 클릭합니다. **[!UICONTROL 설정]**.

      ![](assets/collection-console.png)

1. **[!UICONTROL 컬렉션 설정]** 대화 상자에서 컬렉션를 공유할 사용자를 선택 하 고 사용자의 전역 역할와 일치 하는 역할를 선택 합니다. 예를 들어, 전체 뷰어에 대 한 뷰어 역할를 글로벌 편집기에 편집기 역할 지정 합니다.

   또는 그룹 멤버십 및 역할에 관계 없이 모든 사용자가 컬렉션를 사용할 수 있도록 하려면 공개 컬렉션 ]**확인란을 선택**[!UICONTROL  하 여 공개 해야 합니다.

   >[!NOTE]
   >
   >그러나 관리자가 아닌 사용자는 공용 컬렉션 만들기를 제한할 수 있으므로 시스템 공간을 저장할 수 있도록 여러 개의 공개 컬렉션이 포함 되지 않습니다. 조직은 [관리 도구] 패널에서 사용 가능한 일반 ]**설정에서 [**[!UICONTROL  공용 컬렉션 만들기 ]**허용]**[!UICONTROL  구성을 비활성화할 수 있습니다.

   ![](assets/collection_sharingadduser.png)

   편집자는 공용 컬렉션를 비공용 컬렉션 **[!UICONTROL 으로 변경할 수 없으므로 컬렉션 설정]** 대화 상자에서 **[!UICONTROL 사용할 수 있는 공용 컬렉션]** 확인란은 없습니다.

   ![](assets/collection-setting-editor.png)

1. **[!UICONTROL 추가]** 버튼을 클릭 하 여 사용자 추가 하 고 저장 ]**을 클릭**[!UICONTROL  합니다. 컬렉션 사용자와 공유 됩니다.

   >[!NOTE]
   >
   >사용자의 역할는 컬렉션 내의 자산 및 폴더에 대 한 액세스를 제어 합니다. 사용자에게 에셋에 대한 액세스 권한이 없는 경우 빈 컬렉션이 사용자와 공유됩니다. 또한 사용자의 역할는 컬렉션에 사용할 수 있는 작업을 제어 합니다.

## 컬렉션 공유 해제 {#unshare-a-collection}

이전에 공유한 컬렉션에 대한 공유를 해제하려면 다음을 수행합니다.

1. **[!UICONTROL 컬렉션]** 콘솔에서 공유 안 함 컬렉션를 선택 합니다.

   맨 위의 도구 모음에서 설정 ]**을 클릭**[!UICONTROL  합니다.

   ![](assets/collection_settings.png)

1. **[!UICONTROL 컬렉션 설정]** 대화 상자의 **[!UICONTROL 구성원]** 섹션에서 사용자 옆에 있는 **[!UICONTROL x]** 기호를 클릭 하 여 컬렉션에 대 한 액세스 권한이 있는 사용자 목록에서 제거 합니다.

   ![](assets/unshare_collection.png)

1. 경고 메시지가 나타납니다. 확인 ]**을 클릭**[!UICONTROL  하 여 컬렉션를 공유 안 함 합니다.

1. 저장 ]**을 클릭**[!UICONTROL  하 여 변경 사항을 적용 합니다.

   공유 목록에서 사용자 제거 되 면 사용자의 **[!UICONTROL 컬렉션]** 콘솔에서 공유 되지 않은 컬렉션 제거 됩니다.

<!--
1. Click the overlay icon on the left, and choose **[!UICONTROL Navigation]**.

   ![](assets/contenttree-1.png)

1. From the siderail on the left, click **[!UICONTROL Collections]**.

   ![](assets/access_collections.png)

1. From the **[!UICONTROL Collections]** console, do one of the following:

    * Hover the pointer over the collection you want to share. From the quick action thumbnails available for the collection, click the **[!UICONTROL Settings]** icon.

   ![](assets/settings_thumbnail.png)

    * Select the collection you want to share. From the toolbar at the top, click **[!UICONTROL Settings]**.
    
   ![](assets/collection-sharing.png)

1. In the [!UICONTROL Collection Settings] dialog box, select the users or groups with whom you want to share the collection and select the role for a user or a group to match their global role. For example, assign the Editor role to a global editor, the Viewer role to a global viewer.

   Alternatively, to make the collection available to all users irrespective of their group membership and role, make it public by selecting the **[!UICONTROL Public Collection]** check-box.

   >[!NOTE]
   >
   >However, non-admin users can be restricted from creating public collections, to avoid having numerous public collections so that system space can be saved. Organizations can disable the **[!UICONTROL Allow public collections creation]** configuration from [!UICONTROL General] settings available in admin tools panel.

   ![](assets/collection_sharingadduser.png)

   Editors cannot change a public collection to a non-public collection and, therefore, do not have **[!UICONTROL Public Collection]** check-box available in **[!UICONTROL Collection Settings]** dialog.

   ![](assets/collection-setting-editor.png)

1. Select **[!UICONTROL Add]**, and then **[!UICONTROL Save]**. The collection is shared with the chosen users.

   >[!NOTE]
   >
   >A user's role governs access to the assets and folders inside a collection. If a user does not have access to assets, an empty collection is shared with the user. Also, a user's role governs the actions available for collections.

## Unshare a collection {#unshare-a-collection}

To unshare a previously shared collection, do the following:

1. From the **[!UICONTROL Collections]** console, select the collection you want to unshare.

   In the toolbar, click **[!UICONTROL Settings]**.

   ![](assets/collection_settings.png)

1. On the **[!UICONTROL Collection Settings]** dialog box, under **[!UICONTROL Members]**, click the **[!UICONTROL x]** symbol next to users or groups to remove them from the list of users you shared the collection with.

   ![](assets/unshare_collection.png)

1. In the warning message box, click **[!UICONTROL Confirm]** to confirm unshare.

   Click **[!UICONTROL Save]**.

1. Log in to Brand Portal with the credentials of the user you removed from the shared list. The collection is removed from the **[!UICONTROL Collections]** console.
-->
