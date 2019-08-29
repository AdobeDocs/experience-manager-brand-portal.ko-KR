---
title: 이미지 사전 설정 또는 동적 표현물 적용
seo-title: 이미지 사전 설정 또는 동적 표현물 적용
description: '매크로와 마찬가지로 이미지 사전 설정은 이름 아래에 저장된 사전 정의된 크기 및 서식 지정 명령의 사전 정의된 모음입니다. 이미지 사전 설정을 사용하면 AEM Assets 브랜드 포털에서 다양한 크기, 형식 및 속성의 이미지를 동적으로 전달할 수 있습니다. '
seo-description: '매크로와 마찬가지로 이미지 사전 설정은 이름 아래에 저장된 사전 정의된 크기 및 서식 지정 명령의 사전 정의된 모음입니다. 이미지 사전 설정을 사용하면 AEM Assets 브랜드 포털에서 다양한 크기, 형식 및 속성의 이미지를 동적으로 전달할 수 있습니다. '
uuid: A 3 C 8705 C -5 FBD -472 C -8 B 61-F 65 B 3 E 552 C 1 B
content-type: 참조
topic-tags: 관리
products: sg_ Experiencemanager/brand_ portal
discoiquuid: A 512 DFA 0-FEF 3-4 C 3 F-A 389-A 0 A 3 A 7415 BAC
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# 이미지 사전 설정 또는 동적 표현물 적용 {#apply-image-presets-or-dynamic-renditions}

매크로와 마찬가지로 이미지 사전 설정은 이름 아래에 저장된 사전 정의된 크기 및 서식 지정 명령의 사전 정의된 [!UICONTROL 모음입니다. ] 이미지 사전 설정을 사용하면 [!DNL AEM] 에셋을 통해 [!DNL Brand Portal] 다양한 크기, 포맷 및 속성의 이미지를 동적으로 전달할 수 있습니다.

이미지 사전 설정은 미리 보고 다운로드할 수 있는 이미지의 동적 표현물을 생성하는 데 사용됩니다. 이미지와 해당 변환을 미리 볼 때 관리자가 설정한 사양에 맞게 이미지의 서식을 변경할 사전 설정을 선택할 수 있습니다.

의 [!DNL Brand Portal]자산의 동적 표현물을 보려면 게시 위치에서 해당 PTIFF 변환이 [!DNL AEM] 작성자 인스턴스에 있는지 확인합니다 [!DNL Brand Portal]. 자산을 게시하면 해당 PTIFF 표현물도 [!DNL Brand Portal]게시됩니다. PTIFF 변환을 생성할 방법은 [!DNL Brand Portal]없습니다.

>[!NOTE]
>
>이미지와 해당 변환을 다운로드할 때 기존 사전 설정에서 선택할 수 있는 옵션은 없습니다. 대신 사용자 지정 이미지 사전 설정의 속성을 지정할 수 있습니다. 자세한 내용은 이미지 다운로드 시 이미지 사전 설정 [적용을](../using/brand-portal-image-presets.md#main-pars-text-1403412644)참조하십시오.

이미지 사전 설정을 만드는 동안 필요한 매개 변수에 대한 자세한 내용은 이미지 사전 설정 [관리](https://docs.adobe.com/docs/en//6-0/administer/integration/dynamic-media/image-presets.html)[!DNL AEM]를 참조하십시오.

## 이미지 사전 설정 만들기 {#create-an-image-preset}

관리자는 자산 세부 사항 페이지에서 다이내믹 표현물로 표시되는 이미지 사전 설정을 만들 수 있습니다. 처음부터 이미지 사전 설정을 만들거나 새 이름으로 기존 이미지 사전 설정을 저장할 수 있습니다. 이미지 사전 설정을 만들 때 이미지 전달 및 서식 지정 명령을 위한 크기를 선택합니다. 이미지를 볼 때 이미지를 제공하면 선택한 명령에 따라 해당 모양이 최적화됩니다.
관리자만에서 이미지 사전 설정을 만들 [!DNL Brand Portal]수 있습니다.

관리자만에서 이미지 사전 설정을 만들 [!DNL Brand Portal]수 있습니다.

>[!NOTE]
>
>PTIFF가 제공되는 자산에 대해 동적 표현물이 생성됩니다. 따라서 자산에 만들어 게시된 피라미드형 TIFF [!DNL AEM] 변환이 없는 [!DNL Brand Portal]경우 시스템 변환만 내보낼 수 있지만 동적 표현물은 옵션으로 제공됩니다.
에셋의 피라미드형 TIFF (PTIFF) 를 만들려면 Dynamic Media 하이브리드 모드를 (author) 에서 [!DNL AEM] 활성화해야 합니다. 이러한 자산이 게시되면 이미지 [!DNL Brand Portal]사전 설정이 적용되고 동적 표현물이 표시됩니다.

1. 상단에 [!DNL AEM] 있는 도구 모음에서 Adobe 로고를 클릭하여 관리 도구에 액세스합니다.

   !![](assets/[!DNL AEM]logo. png)

2. 관리 도구 패널에서 **이미지 사전 설정을**&#x200B;클릭합니다.

   ![](assets/admin-tools-panel-4.png)

3. 이미지 사전 설정 페이지에서 **만들기를**&#x200B;클릭합니다.

   ![](assets/image_preset_homepage.png)

4. 이미지 사전 설정 **편집** 페이지에서 이름을 포함하여 **기본** 및 **고급** 탭에 값을 입력합니다. 옵션은 [이미지 사전 설정 옵션](https://docs.adobe.com/docs/en//6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options)에[!DNL AEM]요약되어 있습니다. 사전 설정은 왼쪽 창에 나타나며 다른 자산과 함께 즉석에서 사용할 수 있습니다.

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >[이미지 사전 설정 **편집** ] 페이지를 사용하여 기존 이미지 사전 설정의 속성을 편집할 수도 있습니다. 이미지 사전 설정을 편집하려면 [이미지 사전 설정] 페이지에서 해당 사전 설정을 선택하고 [ **편집**] 를 클릭합니다.

5. **저장**&#x200B;을 클릭합니다. 이미지 사전 설정이 만들어지고 [이미지 사전 설정] 페이지에 표시됩니다.
6. 이미지 사전 설정을 삭제하려면 [이미지 사전 설정] 페이지에서 해당 사전 설정을 선택하고 [ **삭제**] 를 클릭합니다. 확인 페이지에서 **삭제를** 클릭하여 삭제를 확인합니다. 이미지 사전 설정이 이미지 사전 설정 페이지에서 제거됩니다.

## 이미지를 미리 볼 때 이미지 사전 설정 적용 {#apply-image-presets-when-previewing-images}

이미지와 해당 변환을 미리 볼 때 기존 사전 설정에서 선택하여 관리자가 설정한 사양에 맞게 이미지를 다시 포맷합니다.

1. [!DNL Brand Portal] 인터페이스에서 이미지를 클릭하여 엽니다.
2. 왼쪽에 있는 오버레이 아이콘을 클릭하고 **표현물을 선택합니다**.

   ![](assets/image-preset-previewrenditions.png)

3. **[변환** ] 목록에서 썸네일 (예: **썸네일**) 를 선택합니다. 미리 보기 이미지는 변환에 따라 렌더링됩니다.

   ![](assets/image-preset-previewrenditionthumbnail.png)

## 이미지 다운로드 시 이미지 사전 설정 적용 {#apply-image-presets-when-downloading-images}

이미지 및에서 [!DNL Brand Portal]해당 변환을 다운로드할 때는 기존 이미지 사전 설정에서 선택할 수 없습니다. 그러나 이미지 서식을 다시 지정할 이미지 사전 설정 속성을 사용자 지정할 수 있습니다.

1. [!DNL Brand Portal] 인터페이스에서 다음 중 하나를 수행합니다.

   * 다운로드할 이미지 위로 포인터를 가져갑니다. 빠른 작업 썸네일에서 **다운로드** 아이콘을 클릭합니다.
   ![](assets/downloadsingleasset.png)

   * 다운로드할 이미지를 선택합니다. 상단에 있는 도구 모음에서 **다운로드** 아이콘을 클릭합니다.
   ![](assets/downloadassets.png)

2. **다운로드** 대화 상자에서 표현물이 있거나 없는 자산을 다운로드할지 여부에 따라 필요한 옵션을 선택합니다.

   ![](assets/donload-assets-dialog.png)

3. 자산의 동적 표현물을 다운로드하려면 **Dynamic Rendition (s)** 옵션을 선택합니다.
4. 다운로드하는 동안 이미지 및 해당 표현물의 형식을 동적으로 다시 지정할 이미지 사전 설정 속성을 사용자 지정합니다. 크기, 형식, 색상 공간, 해상도 및 이미지 수정자를 지정합니다.

   ![](assets/dynamicrenditions.png)

5. ****&#x200B;다운로드를 클릭합니다. 사용자 지정 동적 표현물은 다운로드하도록 선택한 이미지 및 변환과 함께 ZIP 파일로 다운로드됩니다. 단, 단일 에셋이 다운로드되는 경우 ZIP 파일이 만들어지지 않으므로 빠른 다운로드가 보장됩니다.
