---
title: 'Experience Manager Assets에서 Brand Portal으로 기여도 폴더 구성 및 게시 '
seo-title: Configure and publish contribution folder from Experience Manager Assets to Brand Portal
description: Experience Manager Assets에서 Brand Portal으로 기여도 폴더를 구성하고 게시하기 위한 통찰력을 얻을 수 있습니다.
seo-description: Get an insight into configuring and publishing a contribution folder from Experience Manager Assets to Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 9acad588-977a-45de-b544-f2cc8874ba12
source-git-commit: 3845d9fa17e75d59493383303ca0978349ca0401
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 0%

---

# Experience Manager Assets에서 기여 폴더 구성 {#configure-contribution-folder}

공동 작업 자산 소싱을 위해 Experience Manager Assets 사용자(권한이 있는 관리자 및 비관리 사용자)는 새 유형의 폴더를 만들 수 있습니다 **자산 기여**&#x200B;를 설정하는 경우, Brand Portal 사용자가 만든 새 폴더를 자산 제출로 열 수 있도록 합니다.  이렇게 하면 다음과 같은 두 개의 추가 하위 폴더를 만드는 워크플로우가 자동으로 트리거됩니다. **공유** 및 **신규**: 새로 만든 내의 **기여도** 폴더를 입력합니다.

그런 다음 Experience Manager Assets 사용자는 기여 폴더에 추가해야 하는 자산 유형과 기준 자산 세트에 대한 개요를 기준 자산에 업로드하여 자산 요구 사항을 정의합니다 **공유** 폴더를 사용하십시오. 그런 다음 관리자는 새로 만든 기여도 폴더를 Brand Portal에 게시하기 전에 활성 Brand Portal 사용자에게 기여도 폴더에 대한 액세스 권한을 부여할 수 있습니다.

다음 비디오에서는 Experience Manager Assets에서 기여도 폴더를 구성하는 방법을 보여 줍니다.

>[!VIDEO](https://video.tv.adobe.com/v/30547)

Experience Manager Assets 사용자는 기여 폴더를 구성하는 동안 다음 활동을 수행합니다.

* [기여도 폴더 만들기](#create-contribution-folder)
* [자산 요구 사항 업로드 및 기여자 할당](#configure-contribution-folder-properties)
* [기준 자산 업로드](#uplad-new-assets-to-contribution-folder)
* [Experience Manager Assets의 기여도 폴더를 Brand Portal에 게시](#publish-contribution-folder-to-brand-portal)

## 기여도 폴더 만들기 {#create-contribution-folder}


Experience Manager Assets 관리자와 관리자가 아닌 사용자가 새 폴더를 만들 권한이 있는 경우 Experience Manager Assets에서 기여 폴더를 만들 수 있습니다.
기여도 폴더를 만들려면, 자산 기여도 유형의 새 폴더를 만드십시오. 이렇게 하면 Brand Portal 사용자가 만든 새 폴더를 자산 제출로 열 수 있습니다.  이렇게 하면 기여도 폴더 내에서 SHARED 및 NEW라는 두 개의 추가 하위 폴더를 만드는 워크플로우를 자동으로 트리거합니다.


>[!NOTE]
>
>관리자는 폴더 내에 여러 자산 기여 폴더를 만들 수 있습니다.
>
>자산 기여 폴더에는 자산의 분배 및 기여 시 사용할 NEW 및 SHARED 폴더가 포함됩니다. 기여도 폴더 내에 자산, 폴더 또는 기여도 폴더를 만들지 마십시오.


기여도 폴더를 만드는 동안 기여도 폴더 속성을 별도로 구성할 수도 있습니다. 이 예에서는 속성을 별도로 구성합니다.

**기여 폴더를 만들려면:**

1. Experience Manager Assets 인스턴스에 로그인합니다.

1. 다음으로 이동 **[!UICONTROL 자산]** > **[!UICONTROL 파일]**. Experience Manager Assets 저장소의 모든 기존 폴더를 나열합니다.

1. 클릭 **[!UICONTROL 만들기]** 새 폴더를 만들려면 **[!UICONTROL 폴더 만들기]** 대화 상자가 열립니다.

1. Enter 키 **[!UICONTROL 제목]** 및 **[!UICONTROL 이름]** 폴더의 **[!UICONTROL 자산 기여]** 확인란을 선택합니다.
폴더 이름을 지정하려면 공백 없이 소문자를 사용하는 것이 좋습니다.

1. **[!UICONTROL 만들기]**&#x200B;를 클릭합니다. Experience Manager Assets 저장소에 나열된 기여도 폴더를 볼 수 있습니다.

   >[!NOTE]
   >
   >관리자가 아닌 사용자는 자산 기여 폴더를 만들고 공유할 수 있지만 수정하거나 삭제할 수 없습니다.


   ![](assets/create-contribution-folder.png)

1. 기여도 폴더를 열려면 클릭합니다. 두 개의 하위 폴더가 표시됩니다.**[!UICONTROL 공유]** 및 **[!UICONTROL 신규]** 기여도 폴더 내에 자동으로 만들어집니다.

   ![](assets/contribution-folder.png)


## 기여도 폴더 속성 구성 {#configure-contribution-folder-properties}

Experience Manager Assets 관리자는 기여 폴더의 속성을 구성하는 동안 다음 활동을 수행합니다.

* **설명 추가**: 기여 폴더에 대한 높은 수준의 설명을 제공합니다.
* **개요 업로드**: 자산 관련 정보가 포함된 자산 요구 사항 문서를 업로드합니다.
* **기여자 추가**: 기여도 폴더에 대한 액세스 권한을 부여할 Brand Portal 사용자를 추가합니다.

자산 요구 사항은 기여자(Brand Portal 사용자)가 기여도 폴더의 요구 사항과 요구 사항을 이해하는 데 도움이 되도록 관리자가 제공하는 세부 정보를 나타냅니다. 관리자가 기여도 폴더 및 자산 관련 정보(예: 목적, 이미지 유형, 최대 크기 등)에 추가해야 하는 자산 유형에 대한 간단한 설명이 포함된 자산 요구 사항 문서를 업로드합니다.

**기여도 폴더 속성을 구성하려면:**

1. Experience Manager Assets 인스턴스에 로그인합니다.

1. 다음으로 이동 **[!UICONTROL 자산 > 파일]** 기여도 폴더를 찾습니다.
1. 기여도 폴더를 선택하고 을(를) 클릭합니다 **[!UICONTROL 속성]** 폴더 속성 창을 열려면 다음을 수행하십시오.

   ![](assets/properties.png)

   ![](assets/contribution-folder-property1.png)

1. 다음으로 이동 **[!UICONTROL 자산 기여]** 탭.
1. 높은 수준 입력 **[!UICONTROL 설명]** 기여도 폴더에 배치합니다.
1. 클릭 **[!UICONTROL 개요 업로드]** 로컬 시스템에서 탐색하고 업로드하려면 **자산 요구 사항 문서**.

   ![](assets/upload.png)

1. 에서 **[!UICONTROL 사용자 추가]** 필드에서 기여도 폴더를 공유할 Brand Portal 사용자를 추가합니다. 이러한 사용자는 Brand Portal 인터페이스를 사용하여 기여도 폴더에 액세스하고 컨텐츠를 업로드할 수 있습니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   ![](assets/contribution-folder-property3.png)

>[!NOTE]
>
>검색 결과는 Experience Manager Assets에 구성된 Brand Portal 사용자 목록을 기반으로 합니다. 업데이트된 Brand Portal 사용자 목록이 있는지 확인합니다.

관리자는 `user.csv` 파일 위치 [!DNL Admin Console] Brand Portal 사용자를 추가하기 위한 기본 템플릿으로 사용합니다. 이동 [!UICONTROL 사용자] 을(를) 클릭하고 [!UICONTROL 사용자 목록을 csv로 내보내기] 옵션 다운로드 `users.csv` 파일. 다음 샘플 사용자는사용자를 추가하는 데 필요한 속성에 대해 자세히 설명합니다. 사용자 항목에 대한 유일한 필수 속성은 다음과 같습니다 `Email` 그리고 다른 모든 속성은 선택 사항입니다.

[파일 가져오기](assets/users.csv)

## 기여도 폴더에 자산 업로드 {#uplad-new-assets-to-contribution-folder}

Experience Manager Assets 사용자가 기준선 자산 세트를 로 업로드합니다 **공유** 폴더를 사용하십시오.

**기준 자산을 업로드하려면 다음을 수행하십시오.**

1. Experience Manager Assets 인스턴스에 로그인합니다.

1. 다음으로 이동 **[!UICONTROL 자산 > 파일]** 기여도 폴더를 찾습니다.

1. 기여도 폴더를 선택하고 을(를) 클릭하여 엽니다.

1. 을(를) 클릭합니다. **[!UICONTROL 신규]** 폴더를 입력합니다.

   ![](assets/upload-new-assets1.png)

1. 클릭 **[!UICONTROL 만들기]** > **[!UICONTROL 파일]** 여러 자산이 들어 있는 개별 파일 또는 폴더(.zip)를 업로드합니다.

   ![](assets/upload-new-assets2.png)

1. 자산(파일 또는 폴더)을 **[!UICONTROL 신규]** 폴더를 입력합니다.

   ![](assets/upload-asset4.png)

모든 자산 또는 폴더를 새 폴더에 업로드한 후 기여도 폴더를 Experience Manager Assets에 게시합니다.


## Brand Portal에 기여도 폴더 게시 {#publish-contribution-folder-to-brand-portal}

기여도 폴더가 구성되면 Experience Manager Assets 사용자(관리자/비관리 사용자)는 Experience Manager Assets에서 Brand Portal으로 기여도 폴더를 게시할 수 있습니다. 기여도 폴더에 액세스할 수 있는 권한이 있는 Brand Portal 사용자는 게시 작업이 완료되면 이메일/펄스 알림을 받게 됩니다.


**기여도 폴더를 게시하려면 다음을 수행하십시오.**

1. Experience Manager Assets 인스턴스에 로그인합니다.

1. 다음으로 이동 **[!UICONTROL 자산 > 파일]** Brand Portal에 게시할 기여도 폴더를 찾습니다.
1. 기여도 폴더를 선택하고 을(를) 클릭합니다 **[!UICONTROL 빠른 게시]** > **[!UICONTROL Brand Portal에 게시]**.

   ![](assets/publish-contribution-folder-to-bp.png)

   기여도 폴더가 Brand Portal에 게시되면 성공 메시지가 표시됩니다.

기여도 폴더에 지정된 Brand Portal 사용자에게 이메일/펄스 알림이 전송됩니다. Brand Portal 사용자는 기여도 폴더에 액세스하고 기여도를 시작할 수 있습니다. 참조, [자산을 기여도 폴더에 업로드하고 Experience Manager Assets에 게시](brand-portal-publish-contribution-folder-to-aem-assets.md).
