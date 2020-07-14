---
title: 이미지 사전 설정 또는 동적 변환 적용
seo-title: 이미지 사전 설정 또는 동적 변환 적용
description: '매크로와 마찬가지로 이미지 사전 설정은 이름 아래에 저장된 크기 및 서식 지정 명령의 사전 정의된 모음입니다. AEM Assets 브랜드 포털은 이미지 사전 설정을 통해 다양한 크기, 형식 및 속성의 이미지를 동적으로 제공할 수 있습니다. '
seo-description: '매크로와 마찬가지로 이미지 사전 설정은 이름 아래에 저장된 크기 및 서식 지정 명령의 사전 정의된 모음입니다. AEM Assets 브랜드 포털은 이미지 사전 설정을 통해 다양한 크기, 형식 및 속성의 이미지를 동적으로 제공할 수 있습니다. '
uuid: a3c8705c-5fbd-472c-8b61-f65b3e552c1b
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: a512dfa0-fef3-4c3f-a389-a0a3a7415bac
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d
workflow-type: tm+mt
source-wordcount: '892'
ht-degree: 2%

---


# 이미지 사전 설정 또는 동적 변환 적용 {#apply-image-presets-or-dynamic-renditions}

매크로와 마찬가지로 이미지 사전 설정은 이름 아래에 저장된 크기 및 서식 지정 명령의 사전 정의된 모음입니다. AEM Assets 브랜드 포털은 이미지 사전 설정을 통해 다양한 크기, 형식 및 속성의 이미지를 동적으로 제공할 수 있습니다.

이미지 사전 설정은 미리 보고 다운로드할 수 있는 이미지의 동적 변환을 생성하는 데 사용됩니다. 이미지 및 해당 변환을 미리 볼 때, 관리자가 설정한 사양에 맞게 이미지의 서식을 재지정하는 사전 설정을 선택할 수 있습니다.

브랜드 포털에서 자산의 다이내믹한 표현물을 보려면 해당 피라미드형 tiff 표현물이 브랜드 포털에 게시하는 AEM 작성자 인스턴스에 있는지 확인하십시오. 자산을 게시하면 해당 PTIFF 표현도 브랜드 포털에 게시됩니다. 브랜드 포털에서 PTIFF 변환을 생성할 수 있는 방법은 없습니다.

>[!NOTE]
>
>이미지 및 해당 변환을 다운로드할 때 기존 사전 설정에서 선택할 수 있는 옵션이 없습니다. 대신 사용자 정의 이미지 사전 설정의 속성을 지정할 수 있습니다. 자세한 내용은 이미지를 다운로드할 [때 이미지 사전 설정 적용을 참조하십시오](../using/brand-portal-image-presets.md#main-pars-text-1403412644).

이미지 사전 설정을 만드는 동안 필요한 매개 변수에 대한 자세한 내용은 이미지 사전 [설정 관리를 참조하십시오](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html).

## 이미지 사전 설정 만들기 {#create-an-image-preset}

관리자는 자산 세부 사항 페이지에서 동적 표현물로 표시되는 이미지 사전 설정을 만들 수 있습니다. 처음부터 이미지 사전 설정을 만들거나 새 이름으로 기존 사전 설정을 저장할 수 있습니다. 이미지 사전 설정을 만들 때 이미지 전달의 크기와 서식 명령을 선택합니다. 이미지를 보기 위해 전달하면 선택한 명령에 따라 모양이 최적화됩니다.
관리자만 브랜드 포털에서 이미지 사전 설정을 만들 수 있습니다.

관리자만 브랜드 포털에서 이미지 사전 설정을 만들 수 있습니다.

>[!NOTE]
>
>이미지의 동적 표현물은 해당 Pyramid TIFF를 사용하여 만들어집니다. 어떤 자산에서도 Pyramid TIFF를 사용할 수 없는 경우 해당 자산에 대한 다이내믹 표현물은 브랜드 포털에서 가져올 수 없습니다.
AEM(작성자) 인스턴스가 **Dynamic Media 하이브리드 모드에서**&#x200B;실행 중인 경우 이미지 자산의 피라미드형 TIFF 변환이 AEM 저장소에 만들어지고 저장됩니다. 반면에 AEM(작성자) 인스턴스가 **Dynamic Media Scene 7 모드에서**실행 중인 경우 이미지 자산의 피라미드형 TIFF 변환이 Scene 7 서버에 존재합니다.
이러한 에셋이 브랜드 포털에 게시되면 이미지 사전 설정이 적용되고 동적 변환이 표시됩니다.

1. 상단에 있는 AEM 도구 모음에서 Adobe 로고를 클릭하여 관리 도구에 액세스합니다.

1. 관리 도구 패널에서 **[!UICONTROL 이미지 사전 설정을 클릭합니다]**.

   ![](assets/admin-tools-panel-4.png)

1. 이미지 사전 설정 페이지에서 만들기를 **[!UICONTROL 클릭합니다]**.

   ![](assets/image_preset_homepage.png)

1. 이미지 사전 설정 **[!UICONTROL 편집]** 페이지에서 **[!UICONTROL 기본]** 및 **[!UICONTROL 고급]** 탭에 이름을 포함하여 적절한 값을입력합니다. 이 옵션은 [이미지 사전 설정 옵션에 요약되어 있습니다](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options). 사전 설정은 왼쪽 창에 나타나며 다른 에셋과 동시에 사용할 수 있습니다.

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >이미지 사전 설정 **[!UICONTROL 편집]** 페이지를 사용하여 기존 이미지 사전 설정의 속성을 편집할 수도 있습니다. 이미지 사전 설정을 편집하려면 이미지 사전 설정 페이지에서 선택한 다음 **[!UICONTROL 편집을 클릭합니다]**.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다. 이미지 사전 설정이 만들어지고 이미지 사전 설정 페이지에 표시됩니다.
1. 이미지 사전 설정을 삭제하려면 이미지 사전 설정 페이지에서 해당 사전 설정을 선택하고 **[!UICONTROL 삭제를 클릭합니다]**. 확인 페이지에서 **[!UICONTROL 삭제를]** 클릭하여 삭제를 확인합니다. 이미지 사전 설정 페이지에서 이미지 사전 설정이 제거됩니다.

## 이미지 미리 보기 시 이미지 사전 설정 적용  {#apply-image-presets-when-previewing-images}

이미지 및 해당 표현물을 미리 볼 때, 기존 사전 설정 중에서 선택하여 관리자가 설정한 사양에 맞게 이미지를 다시 포맷하십시오.

1. 브랜드 포털 인터페이스에서 이미지를 클릭하여 엽니다.
1. 왼쪽의 오버레이 아이콘을 클릭하고 표현물을 **[!UICONTROL 선택합니다]**.

   ![](assets/image-preset-previewrenditions.png)

1. 표현물 **[!UICONTROL 목록]** 에서 적절한 동적 표현물(예: 축소판)을 **[!UICONTROL 선택합니다]**. 미리 보기 이미지는 선택한 변환에 따라 렌더링됩니다.

   ![](assets/image-preset-previewrenditionthumbnail.png)

## 이미지 다운로드 시 이미지 사전 설정 적용 {#apply-image-presets-when-downloading-images}

브랜드 포털에서 이미지 및 해당 표현물을 다운로드할 때 기존 이미지 사전 설정에서 선택할 수 없습니다. 그러나 이미지의 서식을 다시 지정할 이미지 사전 설정 속성을 사용자 정의할 수 있습니다.

1. 브랜드 포털 인터페이스에서 다음 중 하나를 수행합니다.

   * 다운로드할 이미지 위로 포인터를 가져갑니다. 사용 가능한 빠른 작업 축소판에서 **[!UICONTROL 다운로드]** 아이콘을 클릭합니다.

   ![](assets/downloadsingleasset.png)

   * 다운로드할 이미지를 선택합니다. 상단에 있는 도구 모음에서 **[!UICONTROL 다운로드]** 아이콘을 클릭합니다.

   ![](assets/downloadassets.png)

1. [ **[!UICONTROL 다운로드]** ] 대화 상자에서 해당 표현물과 함께 자산을 다운로드할지 또는 그렇지 않는지에 따라 필요한 옵션을 선택합니다.

   ![](assets/donload-assets-dialog.png)

1. 자산의 동적 표현물을 다운로드하려면 [ **[!UICONTROL 동적 표현물] 옵션을]** 선택합니다.
1. 다운로드하는 동안 이미지 및 표현물의 서식을 동적으로 다시 지정할 이미지 사전 설정 속성을 사용자 정의합니다. 크기, 형식, 색상 공간, 해상도 및 이미지 수정자를 지정합니다.

   ![](assets/dynamicrenditions.png)

1. 다운로드를 **[!UICONTROL 클릭합니다]**. 사용자 지정 동적 표현물은 다운로드하도록 선택한 이미지 및 표현물과 함께 ZIP 파일로 다운로드됩니다. 그러나 단일 자산을 다운로드하면 zip 파일이 만들어지지 않으므로 다운로드 시간이 빨라집니다.
