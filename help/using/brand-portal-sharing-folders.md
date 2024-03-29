---
title: 폴더 공유
seo-title: Share folders
description: Brand Portal은 에셋 수집을 지원하지 않으므로 사전 구성된 Experience Manager Assets 작성자 인스턴스에서 Brand Portal에 에셋을 게시해야 합니다. 게시된 에셋은 Experience Manager 인스턴스로 복제를 구성하는 동안 구성되지 않는 한 Brand Portal의 관리자가 아닌 사용자가 액세스할 수 없으며 사용자와 공유해야 합니다.
seo-description: Brand Portal does not support asset ingestion so assets must be published to Brand Portal from a pre-configured Experience Manager Assets Author instance. Published assets are not accessible to non-admin users of Brand Portal, unless configured while configuring replication with Experience Manager instance, and need to be shared with them.
uuid: 340d0a49-b708-4f0e-9fb8-99c824942f34
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 2332c16f-40be-4673-8cc6-2360d5b74116
exl-id: d28cf927-60e8-437e-9cba-92f7e19020e7
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 2%

---

# Brand Portal에서 폴더 공유 {#share-folders}

Brand Portal은 자산 수집을 지원하지 않으므로 사전 구성된 Experience Manager 작성자 인스턴스에서 Brand Portal에 자산을 게시해야 합니다.

## Brand Portal의 폴더 공유 워크플로 {#folder-sharing-workflow-in-brand-portal}

다음은 폴더 공유 워크플로 및 사용자 액세스에 대해 설명합니다.

* 기본적으로 Experience Manager Assets에서 Brand Portal으로 게시된 모든 폴더는 복제를 구성하는 동안 [공개]로 표시되지 않는 한 Brand Portal 관리자만 볼 수 있습니다.
* 관리자는 **[!UICONTROL 폴더 속성]** 콘솔을 사용하여 선택적 사용자 또는 그룹과 폴더를 공유합니다. 폴더가 공유되는 사용자 또는 그룹만 Brand Portal에 로그인한 후 폴더를 볼 수 있습니다. 폴더가 다른 사용자에게 표시되지 않습니다.
* 관리자는 폴더 속성 ]**콘솔에서**[!UICONTROL  공용 폴더 ]**확인란을 통해**[!UICONTROL  폴더를 공개 하도록 선택할 수도 있습니다. 공용 폴더는 모든 사용자가 볼 수 있습니다.

* 사용자 역할 및 권한과 관계없이 사용자가 Brand Portal에 로그인하면 모든 공용 폴더 및 해당 폴더와 직접 공유되거나 해당 폴더가 속한 그룹과 공유되는 폴더가 표시됩니다. 비공개 폴더 또는 다른 사용자와 공유된 폴더가 모든 사용자에게 표시되지 않습니다.

### Brand Portal에서 사용자 그룹과 폴더 공유 {#sharing-folders-with-user-groups-on-brand-portal}

폴더 에셋에 대한 액세스 권한은 하위 폴더의 설정에 관계없이 상위 폴더의 액세스 권한에 따라 다릅니다. 이 동작은 이 제어합니다. [ACL](https://experienceleague.adobe.com/docs/experience-manager-65/administering/security/security.html) AEM에서 하위 폴더는 상위 폴더에서 ACL을 상속합니다. 예를 들어 폴더 A에 폴더 C가 포함 된 폴더 B가 들어 있는 경우 폴더 A에 대 한 액세스 권한이 있는 사용자 그룹 (또는 사용자)는 폴더 B와 폴더 C에 대 한 동일한 액세스 권한을 갖습니다. 폴더 B는 해당 Acl을 상속 하는 하위 폴더 이며, B의 하위 폴더가 있는 폴더 C는 해당 Acl을 상속 합니다.

마찬가지로 폴더 B에 대 한 액세스 권한이 있는 사용자 그룹 (또는 사용자)은 폴더 A의 폴더 C에 대해 동일한 액세스 권한을 갖습니다. 따라서 조직은 가장 노출 된 자산이 하위 폴더에 배치 되 고 하위 항목에서 루트 폴더에 대 한 액세스를 제한할 수 있도록 컨텐츠 정렬 하는 것이 좋습니다.

### 공용 폴더 게시 {#public-folder-publish}

Brand Portal 복제를 구성 하는 동안 공용 폴더 Publish ]**옵션을 선택 하지 않으면 관리자가 아닌 사용자 (편집자 및 뷰어)가 AEM Assets에서 Brand Portal에 게시 된**[!UICONTROL  자산에 액세스할 수 없습니다.

![](assets/assetbpreplication.png)

**[!UICONTROL 공개 폴더 Publish]** 옵션이 비활성화 된 경우 관리자는 공유 기능을 사용 하 여 관리자가 아닌 사용자와 이러한 자산을 특별히 공유 해야 합니다.

>[!NOTE]
>
>공용 폴더 Publish ]**활성화**[!UICONTROL  하는 옵션은 AEM 6.3.2.1에서 사용할 수 있습니다.

## 공유 폴더 액세스 {#access-to-shared-folders}

다음 매트릭스에서는 다양한 사용자 역할에 대한 에셋 공유/공유 해제에 대한 액세스 권한 및 권한에 대해 설명합니다.

|  | AEM Assets에서 Brand Portal으로 게시된 모든 폴더에 대한 액세스 | 공유 폴더에 대 한 액세스 권한 | 폴더 권한 공유/공유 안 함 |
|---------------|-----------|-----------|------------|
| 관리자 | 예 | 예 | 예 |
| 편집기 | 아니요* | 예, 공유 하거나 자신이 속한 그룹 함께 공유 하는 경우에만 | 예, 해당 폴더 또는 이들이 속한 그룹 함께 공유 된 폴더만 |
| 뷰어 | 아니요* | 예, 해당 사용자와 공유되거나 해당 사용자가 속한 그룹과 공유되는 경우에만 | 아니요 |
| 게스트 사용자 | 아니요* | 예, 공유 하거나 자신이 속한 그룹 함께 공유 하는 경우에만 | 아니요 |

>[!NOTE]
>
>기본적으로 AEM 작성자를 사용 하 여 Brand Portal 복제를 **[!UICONTROL 구성 하는 동안에는 공용 폴더 Publish]** 옵션이 비활성화 됩니다. 이 옵션이 활성화되면 기본적으로 모든 사용자(관리자가 아닌 사용자도 Brand Portal에 게시된 폴더에 액세스할 수 있습니다.

### 관리자가 아닌 사용자 공유 폴더에 대 한 액세스 권한 {#non-admin-user-access-to-shared-folders}

관리자가 아닌 사용자는 Brand Portal에서 공유 되는 폴더에만 액세스할 수 있습니다. 그러나 로그인 할 때 portal에 이러한 폴더가 표시 되는 방법은 폴더 계층 구조 ]**구성 활성화 설정**[!UICONTROL  에 따라 다릅니다.

**구성을 사용할 수 없는 경우**

관리자가 아닌 사용자는 Brand Portal에 로깅의 랜딩 페이지에서 공유 되는 모든 폴더를 볼 수 있습니다.

![](assets/disabled-folder-hierarchy1-1.png)

**구성이 활성화된 경우**

관리자가 아닌 사용자는 Brand Portal에 로그인하면 폴더 트리(루트 폴더에서 시작)와 각 상위 폴더 내에 배치된 공유 폴더를 볼 수 있습니다.

이러한 상위 폴더는 가상 폴더이며 가상 폴더에서 작업을 수행할 수 없습니다. 잠금 아이콘으로 이러한 가상 폴더를 인식할 수 있습니다.

마우스로 가리키거나 선택할 때 작업 작업이 표시되지 않음 **[!UICONTROL 카드 보기]**&#x200B;공유 폴더와 다릅니다. **[!UICONTROL 개요]** 에서 가상 폴더를 선택하면 버튼이 표시됩니다. **[!UICONTROL 열 보기]** 및 **[!UICONTROL 목록 보기]**.

>[!NOTE]
>
>가상 폴더의 기본 썸네일은 첫 번째 공유 폴더의 썸네일 이미지입니다.

![](assets/enabled-hierarchy1-1.png) ![](assets/hierarchy1-nonadmin-1.png) ![](assets/hierarchy-nonadmin-1.png) ![](assets/hierarchy2-nonadmin-1.png)

## 폴더 공유 {#how-to-share-folders}

Brand Portal에서 사용자와 폴더를 공유 하려면 다음 단계를 팔로우 하십시오.

1. 왼쪽에서 [오버레이 아이콘]을 클릭 하 고 [탐색 ]**]을 선택**[!UICONTROL  합니다.

   ![](assets/selectorrail.png)

1. 왼쪽의 siderail에서 파일 ]**를 선택**[!UICONTROL  합니다.

   ![](assets/access_files.png)

1. Brand Portal 인터페이스에서 공유 하려는 폴더를 선택 합니다.

   ![](assets/share-folders.png)

1. 상단의 도구 모음에서 를 선택합니다. **[!UICONTROL 공유]**.

   ![](assets/share_icon.png)

   다음 [!UICONTROL 폴더 속성] 콘솔이 나타납니다.

   ![](assets/folder_properties.png)

1. 다음에서 **[!UICONTROL 폴더 속성]** 콘솔에서 폴더 제목을 **[!UICONTROL 폴더 제목]** 기본 이름을 사용자에게 표시하지 않으려는 경우 필드입니다.
1. 다음에서 **[!UICONTROL 사용자 추가]** 폴더를 공유할 사용자 또는 그룹을 나열하고 **[!UICONTROL 추가]**.
다른 사용자가 없는 게스트 사용자와만 폴더를 공유하려면 **[!UICONTROL 익명 사용자]** 다음에서 **[!UICONTROL 구성원]** 드롭다운입니다.

   ![](assets/only-anonymous.png)

   >[!NOTE]
   >
   >모든 사용자가 폴더를 그룹 멤버십 및 역할에 관계 없이 사용할 수 있게 하려면 공용 폴더 ]**확인란을 선택**[!UICONTROL  합니다.

1. 필요한 경우 **[!UICONTROL 썸네일 변경]** 폴더의 썸네일 이미지를 수정합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

1. 공유 폴더에 액세스하려면 폴더를 공유한 사용자의 자격 증명으로 Brand Portal에 로그인합니다. 인터페이스에서 공유 폴더를 검토합니다.

## 폴더 공유 안 함 {#unshare-the-folders}

이전에 공유한 폴더의 공유를 해제하려면 다음 단계를 수행하십시오.

1. Brand Portal 인터페이스에서 공유 안 함 폴더를 선택 합니다.

   ![](assets/share-folders-1.png)

1. 맨 위에 있는 도구 모음에서 를 클릭합니다. **[!UICONTROL 공유]**.
1. 다음에서 **[!UICONTROL 폴더 속성]** 콘솔, 아래 **[!UICONTROL 구성원]**&#x200B;를 클릭하고 **[!UICONTROL x]** 폴더를 공유한 사용자 목록에서 제거할 사용자 옆의 기호입니다.

   ![](assets/folder_propertiesunshare.png)

1. 경고 메시지 상자에서 **[!UICONTROL 확인]** 공유 취소를 확인합니다.
**[!UICONTROL 저장]**&#x200B;을 클릭합니다.

1. 공유 목록에서 제거한 사용자의 자격 증명으로 Brand Portal에 로그인합니다. 해당 폴더는 사용자의 Brand Portal 인터페이스에서 더 이상 사용할 수 없습니다.
