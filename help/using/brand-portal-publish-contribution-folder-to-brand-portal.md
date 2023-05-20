---
title: Experience Manager Assets에서 Brand Portal으로 기여도 폴더 구성 및 게시
seo-title: Configure and publish contribution folder from Experience Manager Assets to Brand Portal
description: Experience Manager Assets에서 Brand Portal으로의 기여 폴더 구성 및 게시에 대한 통찰력을 얻으십시오.
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

공동 에셋 소싱의 경우 Experience Manager Assets 사용자(권한이 있는 관리자 및 관리자가 아닌 사용자)는 유형의 새 폴더를 만들 수 있습니다 **자산 기여**&#x200B;를 사용하여 생성된 새 폴더가 Brand Portal 사용자에 의해 에셋 제출에 열려 있는지 확인합니다.  그러면 두 개의 추가 하위 폴더(이라고 함)를 만드는 워크플로우가 자동으로 트리거됩니다. **공유됨** 및 **새로 만들기**, 새로 만든 항목 내 **기여도** 폴더를 삭제합니다.

그런 다음 Experience Manager Assets 사용자는 기여 폴더에 추가해야 하는 에셋 유형과 기준 에셋 세트에 대한 간단한 개요를 에셋에 업로드하여 에셋 요구 사항을 정의합니다 **공유됨** Brand Portal 사용자에게 필요한 정보가 있는지 확인하기 위한 폴더입니다. 그런 다음 관리자는 활성 Brand Portal 사용자에게 새로 만든 기여도 폴더를 Brand Portal에 게시하기 전에 기여도 폴더에 대한 액세스 권한을 부여할 수 있습니다.

다음 비디오에서는 Experience Manager Assets에서 기여 폴더를 구성하는 방법을 보여 줍니다.

>[!VIDEO](https://video.tv.adobe.com/v/30547)

Experience Manager Assets 사용자는 기여 폴더를 구성하는 동안 다음 활동을 수행합니다.

* [기여 폴더 만들기](#create-contribution-folder)
* [자산 요구 사항 업로드 및 참가자 할당](#configure-contribution-folder-properties)
* [기준선 에셋 업로드](#uplad-new-assets-to-contribution-folder)
* [Experience Manager Assets에서 Brand Portal으로 기여 폴더 게시](#publish-contribution-folder-to-brand-portal)

## 기여 폴더 만들기 {#create-contribution-folder}


새 폴더를 만들 수 있는 권한이 있는 Experience Manager Assets 관리자 및 관리자가 아닌 사용자는 Experience Manager Assets에서 기여 폴더를 만들 수 있습니다.
기여 폴더를 만들려면 자산 기여 유형의 새 폴더를 만들어 만든 새 폴더가 Brand Portal 사용자에 의해 자산 제출에 열려 있도록 합니다.  이렇게 하면 기여도 폴더 내에 SHARED 및 NEW라는 두 개의 추가 하위 폴더를 만드는 워크플로우가 자동으로 트리거됩니다.


>[!NOTE]
>
>관리자는 폴더 내에 여러 자산 기여 폴더를 만들 수 있습니다.
>
>에셋 기여 폴더에는 에셋의 분배와 기여를 위한 NEW 및 SHARED 폴더가 있습니다. 기여 폴더 내에 에셋, 폴더 또는 기여 폴더를 만들지 마십시오.


기여도 폴더를 만드는 동안뿐만 아니라 기여도 폴더 속성을 개별적으로 구성할 수도 있습니다. 이 예제에서는 속성을 별도로 구성합니다.

**기여 폴더를 만들려면 다음 작업을 수행하십시오.**

1. Experience Manager Assets 인스턴스에 로그인.

1. 다음으로 이동 **[!UICONTROL 에셋]** > **[!UICONTROL 파일]**. 이 목록에는 Experience Manager Assets 저장소의 모든 기존 폴더가 나열됩니다.

1. 클릭 **[!UICONTROL 만들기]** 새 폴더를 만듭니다. **[!UICONTROL 폴더 만들기]** 대화 상자가 열립니다.

1. 입력 **[!UICONTROL 제목]** 및 **[!UICONTROL 이름]** 폴더의 을(를) 선택한 다음 **[!UICONTROL 자산 기여]** 확인란.
폴더 이름을 지정하려면 공백 없이 소문자를 사용하는 것이 좋습니다.

1. **[!UICONTROL 만들기]**&#x200B;를 클릭합니다. Experience Manager Assets 저장소에 나열된 기여 폴더를 볼 수 있습니다.

   >[!NOTE]
   >
   >관리자가 아닌 사용자는 자산 기여 폴더를 만들고 공유할 수 있지만 수정하거나 삭제할 수는 없습니다.


   ![](assets/create-contribution-folder.png)

1. 기여도 폴더를 열려면 클릭하면 두 개의 하위 폴더가 표시됩니다.**[!UICONTROL 공유됨]** 및 **[!UICONTROL 새로 만들기]** 기여도 폴더 내에 자동으로 만들어집니다.

   ![](assets/contribution-folder.png)


## 기여 폴더 속성 구성 {#configure-contribution-folder-properties}

Experience Manager Assets 관리자는 기여 폴더의 속성을 구성하는 동안 다음 활동을 수행합니다.

* **설명 추가**: 기여도 폴더에 대한 높은 수준의 설명을 제공합니다.
* **개요 업로드**: 에셋 관련 정보가 포함된 에셋 요구 사항 문서를 업로드합니다.
* **기여자 추가**: Brand Portal 사용자를 추가하여 기여 폴더에 대한 액세스 권한을 부여합니다.

에셋 요구 사항은 기여자(Brand Portal 사용자)가 기여 폴더의 요구 사항 및 요구 사항을 이해할 수 있도록 관리자가 제공한 세부 정보를 나타냅니다. 관리자가 기여 폴더에 추가해야 하는 에셋 유형 및 에셋 관련 정보(예: 목적, 이미지 유형, 최대 크기 등)에 대한 간단한 정보가 포함된 에셋 요구 사항 문서를 업로드합니다.

**기여 폴더 속성을 구성하려면 다음을 수행합니다.**

1. Experience Manager Assets 인스턴스에 로그인.

1. 다음으로 이동 **[!UICONTROL 에셋 > 파일]** 기여도 폴더를 찾습니다.
1. 기여도 폴더를 선택하고 **[!UICONTROL 속성]** 폴더 속성 창을 엽니다.

   ![](assets/properties.png)

   ![](assets/contribution-folder-property1.png)

1. 다음으로 이동 **[!UICONTROL 자산 기여]** 탭.
1. 높은 수준으로 입력 **[!UICONTROL 설명]** 기여도 폴더 내.
1. 클릭 **[!UICONTROL 개요 업로드]** 로컬 컴퓨터에서 찾아보고 **자산 요구 사항 문서**.

   ![](assets/upload.png)

1. 다음에서 **[!UICONTROL 사용자 추가]** 기여도 폴더를 공유할 Brand Portal 사용자를 필드에 추가합니다. 이러한 사용자는 Brand Portal 인터페이스를 사용하여 기여 폴더에 컨텐츠를 액세스하고 업로드할 수 있습니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   ![](assets/contribution-folder-property3.png)

>[!NOTE]
>
>검색 결과는 Experience Manager Assets에 구성된 Brand Portal 사용자 목록을 기반으로 합니다. 업데이트된 Brand Portal 사용자 목록이 있는지 확인합니다.

관리자는 `user.csv` 파일 출처: [!DNL Admin Console] Brand Portal 사용자를 추가하기 위한 기본 템플릿으로 사용합니다. 다음으로 이동 [!UICONTROL 사용자] 을(를) 클릭하고 [!UICONTROL 사용자 목록을 csv로 내보내기] 다운로드 옵션 `users.csv` 파일. 다음 샘플 사용자 목록에서는 사용자를 추가하는 데 필요한 속성을 자세히 설명합니다. 사용자 항목에 대한 유일한 필수 속성은 다음과 같습니다. `Email` 다른 속성은 모두 선택 사항입니다.

[파일 가져오기](assets/users.csv)

## 기여 폴더에 자산 업로드 {#uplad-new-assets-to-contribution-folder}

Experience Manager Assets 사용자가 기준선 에셋 세트를 **공유됨** Brand Portal 사용자에게 필요한 정보가 있는지 확인하기 위한 폴더입니다.

**기준 자산을 업로드하려면 다음을 수행합니다.**

1. Experience Manager Assets 인스턴스에 로그인.

1. 다음으로 이동 **[!UICONTROL 에셋 > 파일]** 기여도 폴더를 찾습니다.

1. 기여도 폴더를 선택하고 을(를) 클릭하여 엽니다.

1. 을(를) 클릭합니다 **[!UICONTROL 새로 만들기]** 폴더를 삭제합니다.

   ![](assets/upload-new-assets1.png)

1. 클릭 **[!UICONTROL 만들기]** > **[!UICONTROL 파일]** 여러 에셋이 들어 있는 개별 파일 또는 폴더(.zip)를 업로드합니다.

   ![](assets/upload-new-assets2.png)

1. 에셋(파일 또는 폴더)을에 검색 및 업로드 **[!UICONTROL 새로 만들기]** 폴더를 삭제합니다.

   ![](assets/upload-asset4.png)

모든 에셋 또는 폴더를 NEW 폴더에 업로드한 후 기여도 폴더를 Experience Manager Assets에 게시합니다.


## 기여 폴더를 Brand Portal에 게시 {#publish-contribution-folder-to-brand-portal}

기여도 폴더가 구성되면 Experience Manager Assets 사용자(관리자/관리자가 아닌 사용자)는 기여도 폴더를 Experience Manager Assets에서 Brand Portal으로 게시할 수 있습니다. 기여 폴더에 액세스할 권한이 있는 Brand Portal 사용자는 게시 작업이 완료되면 이메일/펄스 알림을 받게 됩니다.


**기여 폴더를 게시하려면 다음을 수행하십시오.**

1. Experience Manager Assets 인스턴스에 로그인.

1. 다음으로 이동 **[!UICONTROL 에셋 > 파일]** Brand Portal에 게시할 기여 폴더를 찾습니다.
1. 기여도 폴더를 선택하고 **[!UICONTROL 빠른 게시]** > **[!UICONTROL Brand Portal에 게시]**.

   ![](assets/publish-contribution-folder-to-bp.png)

   기여도 폴더가 Brand Portal에 게시되면 성공 메시지를 받게 됩니다.

기여 폴더에 할당된 Brand Portal 사용자에게 이메일/펄스 알림이 전송됩니다. Brand Portal 사용자는 기여 폴더에 액세스하여 기여를 시작할 수 있습니다. 다음을 참조하십시오. [기여 폴더에 에셋을 업로드하고 Experience Manager Assets에 게시](brand-portal-publish-contribution-folder-to-aem-assets.md).
