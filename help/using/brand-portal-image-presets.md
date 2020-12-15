---
title: 이미지 사전 설정 또는 동적 변환 적용
seo-title: 이미지 사전 설정 또는 동적 변환 적용
description: '매크로와 마찬가지로 이미지 사전 설정은 이름 아래에 저장된 크기 및 서식 지정 명령의 사전 정의된 모음입니다. 이미지 사전 설정을 사용하면 AEM Assets Brand Portal에서 다양한 크기, 형식 및 속성의 이미지를 동적으로 제공할 수 있습니다. '
seo-description: '매크로와 마찬가지로 이미지 사전 설정은 이름 아래에 저장된 크기 및 서식 지정 명령의 사전 정의된 모음입니다. 이미지 사전 설정을 사용하면 AEM Assets Brand Portal에서 다양한 크기, 형식 및 속성의 이미지를 동적으로 제공할 수 있습니다. '
uuid: a3c8705c-5fbd-472c-8b61-f65b3e552c1b
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: a512dfa0-fef3-4c3f-a389-a0a3a7415bac
translation-type: tm+mt
source-git-commit: 2f6ec4ac56390b2243e1d1a2c2adb34eb9aad7b2
workflow-type: tm+mt
source-wordcount: '871'
ht-degree: 2%

---


# 이미지 사전 설정 또는 동적 변환 적용 {#apply-image-presets-or-dynamic-renditions}

매크로와 마찬가지로 이미지 사전 설정은 이름 아래에 저장된 크기 및 서식 지정 명령의 사전 정의된 모음입니다. 이미지 사전 설정을 사용하면 AEM Assets Brand Portal에서 다양한 크기, 형식 및 속성의 이미지를 동적으로 제공할 수 있습니다.

이미지 사전 설정은 미리 보고 다운로드할 수 있는 이미지의 동적 변환을 생성하는 데 사용됩니다. 이미지 및 해당 변환을 미리 볼 때, 관리자가 설정한 사양에 맞게 이미지 형식을 다시 지정할 사전 설정을 선택할 수 있습니다.

(*AEM 작성자 인스턴스가&#x200B;**Dynamic Media Hybrid 모드***에서 실행 중인 경우) 브랜드 포털에서 자산의 다이내믹한 변환을 보려면 해당 Pyramid Tiff 변환이 브랜드 포털에 게시되는 AEM 작성자 인스턴스에 있는지 확인합니다. 자산을 게시하면 해당 PTIFF 표현도 브랜드 포털에 게시됩니다.

>[!NOTE]
>
>이미지 및 해당 변환을 다운로드할 때 기존 사전 설정 중에서 선택할 수 있는 옵션이 없습니다. 대신 사용자 정의 이미지 사전 설정의 속성을 지정할 수 있습니다. 자세한 내용은 이미지 다운로드 시 [이미지 사전 설정 적용을 참조하십시오](../using/brand-portal-image-presets.md#main-pars-text-1403412644).


이미지 사전 설정을 만드는 동안 필요한 매개 변수에 대한 자세한 내용은 [이미지 사전 설정 관리](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html)를 참조하십시오.

## 이미지 사전 설정 {#create-an-image-preset} 만들기

AEM 관리자는 자산 세부 사항 페이지에서 다이내믹 표현물로 나타나는 이미지 사전 설정을 만들 수 있습니다. 처음부터 이미지 사전 설정을 만들거나 새 이름으로 기존 사전 설정을 저장할 수 있습니다. 이미지 사전 설정을 만들 때 이미지 전달의 크기 및 서식 명령을 선택합니다. 이미지를 보기 위해 전달하면 선택한 명령에 따라 이미지가 최적화됩니다.

>[!NOTE]
>
>이미지의 동적 표현물은 해당 피라미드 TIFF를 사용하여 만들어집니다. 어떠한 자산에도 피라미드형 TIFF를 사용할 수 없는 경우 해당 자산에 대한 다이내믹 표현물을 브랜드 포털에서 가져올 수 없습니다.
>
>AEM 작성자 인스턴스가 **Dynamic Media 하이브리드 모드**&#x200B;에서 실행 중이면 이미지 에셋의 피라미드형 TIFF 변환이 만들어지고 AEM 저장소에 저장됩니다.
>
>반면에 AEM 작성자 인스턴스가 **Dynamic Media Scene 7 모드**&#x200B;에서 실행 중이면 이미지 자산의 피라미드형 TIFF 변환이 Scene 7 서버에 존재합니다.
>
>이러한 에셋이 브랜드 포털에 게시되면 이미지 사전 설정이 적용되고 동적 표현물이 표시됩니다.


1. 상단에 있는 AEM 도구 모음에서 Adobe 로고를 클릭하여 관리 도구에 액세스합니다.

1. 관리 도구 패널에서 **[!UICONTROL 이미지 사전 설정]**&#x200B;을 클릭합니다.

   ![](assets/admin-tools-panel-4.png)

1. 이미지 사전 설정 페이지에서 **[!UICONTROL 만들기]**&#x200B;를 클릭합니다.

   ![](assets/image_preset_homepage.png)

1. **[!UICONTROL 이미지 사전 설정 편집]** 페이지에서 이름을 포함하여 **[!UICONTROL 기본]** 및 **[!UICONTROL 고급]** 탭에 값을 적절히 입력합니다. 옵션은 [이미지 사전 설정 옵션](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options)에 요약되어 있습니다. 사전 설정은 왼쪽 창에 표시되며 다른 에셋과 함께 즉시 사용할 수 있습니다.

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >**[!UICONTROL 이미지 사전 설정 편집]** 페이지를 사용하여 기존 이미지 사전 설정의 속성을 편집할 수도 있습니다. 이미지 사전 설정을 편집하려면 이미지 사전 설정 페이지에서 해당 사전 설정을 선택하고 **[!UICONTROL 편집]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다. 이미지 사전 설정이 만들어지고 이미지 사전 설정 페이지에 표시됩니다.
1. 이미지 사전 설정을 삭제하려면 이미지 사전 설정 페이지에서 해당 사전 설정을 선택하고 **[!UICONTROL 삭제]**&#x200B;를 클릭합니다. 확인 페이지에서 **[!UICONTROL 삭제]**&#x200B;를 클릭하여 삭제를 확인합니다. 이미지 사전 설정이 이미지 사전 설정 페이지에서 제거됩니다.

## 이미지 미리 보기 시 이미지 사전 설정 적용 {#apply-image-presets-when-previewing-images}

이미지 및 해당 변환을 미리 볼 때, 기존 사전 설정에서 선택하여 관리자가 설정한 사양에 맞게 이미지를 다시 포맷하십시오.

1. 브랜드 포털 인터페이스에서 이미지를 클릭하여 엽니다.
1. 왼쪽의 오버레이 아이콘을 클릭하고 **[!UICONTROL 표현물]**&#x200B;을 선택합니다.

   ![](assets/image-preset-previewrenditions.png)

1. **[!UICONTROL 표현물]** 목록에서 적절한 동적 표현물을 선택합니다(예: **[!UICONTROL 축소판]**). 미리 보기 이미지는 선택한 변환에 따라 렌더링됩니다.

   ![](assets/image-preset-previewrenditionthumbnail.png)

## 이미지 {#apply-image-presets-when-downloading-images} 다운로드 시 이미지 사전 설정 적용

브랜드 포털에서 이미지 및 해당 표현물을 다운로드할 때 기존 이미지 사전 설정에서 선택할 수 없습니다. 그러나 이미지를 다시 포맷할 이미지를 기반으로 이미지 사전 설정 속성을 사용자 정의할 수 있습니다.

1. 브랜드 포털 인터페이스에서 다음 중 하나를 수행합니다.

   * 다운로드할 이미지 위로 포인터를 가져갑니다. 사용 가능한 빠른 작업 축소판에서 **[!UICONTROL 다운로드]** 아이콘을 클릭합니다.

   ![](assets/downloadsingleasset.png)

   * 다운로드할 이미지를 선택합니다. 맨 위의 도구 모음에서 **[!UICONTROL 다운로드]** 아이콘을 클릭합니다.

   ![](assets/downloadassets.png)

1. **[!UICONTROL 다운로드]** 대화 상자에서 해당 표현물이 있는 에셋을 다운로드할지 여부에 따라 필요한 옵션을 선택합니다.

   ![](assets/donload-assets-dialog.png)

1. 자산의 동적 변환을 다운로드하려면 **[!UICONTROL 동적 변환]** 옵션을 선택합니다.
1. 다운로드하는 동안 이미지 및 표현물의 서식을 동적으로 다시 지정할 이미지 사전 설정 속성을 사용자 정의합니다. 크기, 형식, 색상 공간, 해상도 및 이미지 수정자를 지정합니다.

   ![](assets/dynamicrenditions.png)

1. **[!UICONTROL 다운로드]**&#x200B;를 클릭합니다. 사용자 지정 동적 표현물은 다운로드하기로 선택한 이미지 및 표현물과 함께 ZIP 파일로 다운로드됩니다. 그러나 단일 에셋이 다운로드되면 압축 파일이 만들어지지 않으므로 다운로드 시간이 단축됩니다.
