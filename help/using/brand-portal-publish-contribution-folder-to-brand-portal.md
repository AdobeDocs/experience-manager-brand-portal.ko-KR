---
title: Experience Manager Assets에서 Brand Portal으로 기여도 폴더 구성 및 게시
description: Experience Manager Assets에서 Brand Portal으로의 기여 폴더 구성 및 게시에 대한 통찰력을 얻으십시오.
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
exl-id: 9acad588-977a-45de-b544-f2cc8874ba12
source-git-commit: 9e51048d21c5b4a34696e668309657d2091a8b04
workflow-type: tm+mt
source-wordcount: '1033'
ht-degree: 0%

---

# Experience Manager Assets에서 기여 폴더 구성 {#configure-contribution-folder}

공동 자산 소싱의 경우 Experience Manager Assets 사용자(권한이 있는 관리자 및 관리자가 아닌 사용자)는 **자산 기여** 유형의 폴더를 만들어 만든 폴더가 Brand Portal 사용자가 자산을 제출할 수 있도록 합니다.  이 메서드는 새로 만든 **기여도** 폴더 내에 **SHARED** 및 **NEW**&#x200B;이라는 두 개의 추가 하위 폴더를 만드는 워크플로를 자동으로 트리거합니다.

Experience Manager Assets 사용자는 기여 폴더에 추가해야 하는 에셋 유형에 대한 간단한 개요를 업로드하여 에셋 요구 사항을 정의합니다. 또한 기준선 에셋 세트를 SHARED 폴더에 업로드하여 Brand Portal 사용자가 필요한 정보를 갖도록 합니다. 그런 다음 관리자는 활성 Brand Portal 사용자에게 새로 만든 기여도 폴더를 Brand Portal에 게시하기 전에 기여도 폴더에 대한 액세스 권한을 부여할 수 있습니다.

다음 비디오는 Experience Manager Assets에서 기여 폴더를 구성하는 방법을 보여 줍니다.

>[!VIDEO](https://video.tv.adobe.com/v/30547)

Experience Manager Assets 사용자는 기여 폴더를 구성하는 동안 다음 활동을 수행합니다.

* [기여 폴더 만들기](#create-contribution-folder)
* [자산 요구 사항 업로드 및 참가자 할당](#configure-contribution-folder-properties)
* [기준선 에셋 업로드](#uplad-new-assets-to-contribution-folder)
* [Experience Manager Assets에서 Brand Portal으로의 Publish 기여 폴더](#publish-contribution-folder-to-brand-portal)

## 기여 폴더 만들기 {#create-contribution-folder}

새 폴더를 만들 수 있는 권한이 있는 Experience Manager Assets 관리자 및 관리자가 아닌 사용자는 Experience Manager Assets에서 기여 폴더를 만들 수 있습니다.
기여 폴더를 만들려면 자산 기여 유형의 폴더를 만들어 만든 폴더가 Brand Portal 사용자가 자산 제출에 열려 있도록 합니다. 이 메서드는 기여도 폴더 내에 SHARED 및 NEW라는 두 개의 추가 하위 폴더를 만드는 워크플로를 자동으로 트리거합니다.

>[!NOTE]
>
>관리자는 폴더 내에 여러 자산 기여 폴더를 만들 수 있습니다.
>
>에셋 기여 폴더에는 에셋의 분배와 기여를 위한 NEW 및 SHARED 폴더가 있습니다. 기여 폴더 내에 자산 폴더 또는 기여 폴더를 만들지 마십시오.


기여도 폴더를 만드는 동안뿐만 아니라 기여도 폴더 속성을 개별적으로 구성할 수도 있습니다. 이 예제에서 속성은 별도로 구성됩니다.

**기여 폴더를 만들려면:**

1. Experience Manager Assets 인스턴스에 로그인.

1. **[!UICONTROL Assets]** > **[!UICONTROL 파일]**(으)로 이동합니다. 이 목록에는 Experience Manager Assets 저장소의 모든 기존 폴더가 나열됩니다.

1. 새 폴더를 만들려면 **[!UICONTROL 만들기]**&#x200B;를 클릭하십시오. **[!UICONTROL 폴더 만들기]** 대화 상자가 열립니다.

1. 폴더의 **[!UICONTROL 제목]** 및 **[!UICONTROL 이름]**&#x200B;을 입력하고 **[!UICONTROL 자산 기여도]** 확인란을 선택하십시오.
Adobe은 공백 없이 소문자를 사용하여 폴더 이름을 지정할 것을 권장합니다.

1. **[!UICONTROL 만들기]**&#x200B;를 클릭합니다. Experience Manager Assets 저장소에 나열된 기여 폴더를 볼 수 있습니다.

   >[!NOTE]
   >
   >관리자가 아닌 사용자는 자산 기여 폴더를 만들고 공유할 수 있지만 수정하거나 삭제할 수는 없습니다.


   ![](assets/create-contribution-folder.png)

1. 기여 폴더를 엽니다. 기여도 폴더 내에 자동으로 만들어지는 두 개의 하위 폴더(**[!UICONTROL 공유]** 및 **[!UICONTROL 새로 만들기]**)를 볼 수 있습니다.

   ![](assets/contribution-folder.png)


## 기여 폴더 속성 구성 {#configure-contribution-folder-properties}

Experience Manager Assets 관리자는 기여 폴더의 속성을 구성하는 동안 다음 활동을 수행합니다.

* **설명 추가**: 기여도 폴더에 대한 높은 수준의 설명을 제공합니다.
* **개요 업로드**: 에셋 관련 정보가 포함된 에셋 요구 사항 문서를 업로드합니다.
* **기여자 추가**: 기여자 폴더에 대한 액세스 권한을 부여하려면 Brand Portal 사용자를 추가하십시오.

에셋 요구 사항은 기여자(Brand Portal 사용자)가 기여 폴더의 요구 사항 및 요구 사항을 이해할 수 있도록 관리자가 제공한 세부 정보를 나타냅니다. 관리자는 목적, 이미지 유형 및 최대 크기를 포함하여 기여 폴더에 대한 에셋 유형을 자세히 설명하는 에셋 요구 사항 문서를 업로드합니다.

**기여 폴더 속성을 구성하려면:**

1. Experience Manager Assets 인스턴스에 로그인.

1. **[!UICONTROL Assets > 파일]**(으)로 이동하여 기여도 폴더를 찾습니다.
1. 기여도 폴더를 선택하고 **[!UICONTROL 속성]**&#x200B;을 클릭하여 폴더 속성 창을 엽니다.

   ![](assets/properties.png)

   ![](assets/contribution-folder-property1.png)

1. **[!UICONTROL 자산 기여]** 탭으로 이동합니다.
1. 기여도 폴더의 높은 수준의 **[!UICONTROL 설명]**&#x200B;을 입력하십시오.
1. 로컬 컴퓨터에서 찾아보고 **자산 요구 사항 문서**&#x200B;를 업로드하려면 **[!UICONTROL 개요 업로드]**&#x200B;를 클릭하세요.

   ![](assets/upload.png)

1. **[!UICONTROL 사용자 추가]** 필드에서 기여도 폴더를 공유할 Brand Portal 사용자를 추가합니다. 이러한 사용자는 Brand Portal 인터페이스를 사용하여 기여 폴더에 컨텐츠를 액세스하고 업로드할 수 있습니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   ![](assets/contribution-folder-property3.png)

>[!NOTE]
>
>검색 결과는 Experience Manager Assets에 구성된 Brand Portal 사용자 목록을 기반으로 합니다. 업데이트된 Brand Portal 사용자 목록이 있는지 확인합니다.

관리자는 [!DNL Admin Console]에서 `user.csv` 파일을 다운로드하여 Brand Portal 사용자를 추가하기 위한 기본 템플릿으로 사용할 수 있습니다. [!UICONTROL 사용자] (으)로 이동하고 [!UICONTROL 사용자 목록을 csv로 내보내기] 옵션을 클릭하여 `users.csv` 파일을 다운로드합니다. 다음 샘플 사용자 목록에서는 사용자를 추가하는 데 필요한 속성을 자세히 설명합니다. 사용자 항목에 대한 유일한 필수 특성은 `Email`이며 다른 모든 특성은 선택 사항입니다.

[파일 가져오기](assets/users.csv)

## 기여 폴더에 자산 업로드 {#uplad-new-assets-to-contribution-folder}

Experience Manager Assets 사용자는 기본 자산 집합을 **SHARED** 폴더로 업로드하여 Brand Portal 사용자에게 필요한 정보가 있는지 확인합니다.

**기준 자산을 업로드하려면:**

1. Experience Manager Assets 인스턴스에 로그인.

1. **[!UICONTROL Assets > 파일]**(으)로 이동하여 기여도 폴더를 찾습니다.

1. 기여도 폴더를 선택하고 을(를) 클릭하여 엽니다.

1. **[!UICONTROL 새]** 폴더를 클릭합니다.

   ![](assets/upload-new-assets1.png)

1. **[!UICONTROL 만들기]** > **[!UICONTROL 파일]**&#x200B;을 클릭하여 여러 자산이 포함된 개별 파일 또는 폴더(.zip)를 업로드합니다.

   ![](assets/upload-new-assets2.png)

1. 에셋(파일 또는 폴더)을 찾아 **[!UICONTROL NEW]** 폴더에 업로드합니다.

   ![](assets/upload-asset4.png)

모든 에셋 또는 폴더를 NEW 폴더에 업로드한 후 기여도 폴더를 Experience Manager Assets에 게시합니다.


## Brand Portal에 대한 Publish 기여 폴더 {#publish-contribution-folder-to-brand-portal}

기여도 폴더가 구성되면 Experience Manager Assets 사용자(관리자/관리자가 아닌 사용자)는 기여도 폴더를 Experience Manager Assets에서 Brand Portal으로 게시할 수 있습니다. 기여 폴더에 액세스할 수 있는 권한이 있는 Brand Portal 사용자는 게시 작업이 완료되면 이메일 또는 펄스 알림을 받게 됩니다.


**기여 폴더를 게시하려면:**

1. Experience Manager Assets 인스턴스에 로그인.

1. **[!UICONTROL Assets > 파일]**(으)로 이동하여 Brand Portal에 게시할 기여 폴더를 찾습니다.
1. 기여 폴더를 선택하고 **[!UICONTROL 빠른 Publish]** > **[!UICONTROL Brand Portal으로 Publish]**&#x200B;을 클릭합니다.

   ![](assets/publish-contribution-folder-to-bp.png)

   기여 폴더가 Brand Portal에 게시되면 성공 메시지를 받습니다.

기여 폴더에 할당된 Brand Portal 사용자에게 이메일/펄스 알림이 전송됩니다. Brand Portal 사용자는 기여 폴더에 액세스하여 기여를 시작할 수 있습니다. [기여 폴더에 자산을 업로드하고 Experience Manager Assets에 게시](brand-portal-publish-contribution-folder-to-aem-assets.md)를 참조하세요.
