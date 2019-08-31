---
title: 메타데이터 스키마 양식 사용
seo-title: 메타데이터 스키마 양식 사용
description: 메타데이터 스키마는 특정 스키마를 사용하는 자산에 대해 표시되는 속성 페이지 및 메타데이터 속성의 레이아웃에 대해 설명합니다. 자산에 적용하는 스키마는 속성 페이지에 표시되는 메타데이터 필드를 결정합니다.
seo-description: 메타데이터 스키마는 특정 스키마를 사용하는 자산에 대해 표시되는 속성 페이지 및 메타데이터 속성의 레이아웃에 대해 설명합니다. 자산에 적용하는 스키마는 속성 페이지에 표시되는 메타데이터 필드를 결정합니다.
uuid: 1 A 944 A 3 B -5152-425 F-B 1 EA-BFE 3331 DE 928
content-type: 참조
products: sg_ Experiencemanager/brand_ portal
topic-tags: 관리
discoiquuid: 500 b 46 da-ef 67-46 a 0-a 069-192 f 4 b 1 a 0 eca
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 메타데이터 스키마 양식 사용 {#use-the-metadata-schema-form}

메타데이터 스키마는 특정 스키마를 사용하는 자산에 대해 표시되는 속성 페이지 및 메타데이터 속성의 레이아웃에 대해 설명합니다. 자산에 적용하는 스키마는 속성 페이지에 표시되는 메타데이터 필드를 결정합니다.

각 자산의 **[!UICONTROL 속성]** 페이지에는 자산의 MIME 유형에 따라 기본 메타데이터 속성이 포함됩니다. 관리자는 메타데이터 스키마 편집기를 사용하여 기존 스키마를 수정하거나 사용자 정의 메타데이터 스키마를 추가할 수 있습니다. AEM Assets 브랜드 포털은 다양한 MIME 유형의 자산에 대한 기본 양식을 제공합니다. 그러나 이러한 자산에 대한 사용자 지정 양식을 추가할 수도 있습니다.

## 메타데이터 스키마 양식 추가 {#add-a-metadata-schema-form}

새 메타데이터 스키마 양식을 만들려면 다음을 수행하십시오.

1. 맨 위의 AEM 도구 모음에서 Adobe 로고를 클릭하여 관리 도구에 액세스합니다.

   ![](assets/aemlogo.png)

2. 관리 도구 패널에서 **[!UICONTROL 메타데이터 스키마를 클릭합니다]**.

   ![](assets/navigation-panel.png)

3. **[!UICONTROL 메타데이터 스키마 양식]** 페이지에서 **[!UICONTROL 만들기를]**&#x200B;클릭합니다.

   ![](assets/create-metadata-schema-form.png)

4. 스키마 양식 **[!UICONTROL 만들기]** 대화 상자에서 스키마 양식 제목을 지정한 다음 **[!UICONTROL 만들기를]** 클릭하여 양식 작성 프로세스를 완료합니다.

   ![](assets/create-schema-form.png)

## Edit a metadata schema form {#edit-a-metadata-schema-form}

새로 추가되거나 기존 메타데이터 스키마 양식을 편집할 수 있습니다. 메타데이터 스키마 양식에는 탭 내의 탭 및 양식 항목을 포함하여 상위에서 파생된 컨텐츠가 포함되어 있습니다. 이러한 양식 항목을 메타데이터 노드 내의 필드에 매핑하거나 구성할 수 있습니다.

메타데이터 스키마 양식에 새 탭 또는 양식 항목을 추가할 수 있습니다. 파생된 탭 및 양식 항목 (상위) 이 잠긴 상태에 있습니다. 하위 수준에서 변경할 수는 없습니다.

메타데이터 스키마 양식을 편집하려면 다음을 수행하십시오.

1. 맨 위의 AEM 도구 모음에서 Adobe 로고를 클릭하여 관리 도구에 액세스합니다.

   ![](assets/aemlogo.png)

2. 관리 도구 패널에서 **[!UICONTROL 메타데이터 스키마를 클릭합니다]**.
3. **[!UICONTROL 메타데이터 스키마 양식]** 페이지에서 컬렉션을 편집할 스키마 양식 (예: **[!UICONTROL 컬렉션]**) 를 선택합니다.

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >편집되지 않은 템플릿은 그 앞에 잠금 기호가 표시됩니다. 템플릿을 사용자 지정하는 경우 템플릿이 사라지기 전에 잠금 기호가 표시됩니다.

4. 상단에 있는 도구 모음에서 **[!UICONTROL 편집을]**&#x200B;클릭합니다.

   **[!UICONTROL 메타데이터 스키마 편집기]** 페이지가 열리고 **[!UICONTROL 기본]** 탭이 왼쪽에 열리고 양식 **[!UICONTROL 작성]** 탭이 오른쪽에 열립니다.

5. **[!UICONTROL 메타데이터 스키마 편집기]** 페이지에서 구성 **[!UICONTROL 요소]** **[!UICONTROL 유형 목록의 구성 요소 유형 목록에서 하나 이상의 구성 요소를]** **[!UICONTROL 기본]** 탭으로 드래그하여 자산의 속성 페이지를 사용자 지정합니다.

   ![](assets/metadata-schemaeditor-page.png)

6. 구성 요소를 구성하려면 **[!UICONTROL 설정]** 탭에서 구성 요소를 선택하고 속성을 수정합니다.

### 양식 작성 탭의 구성 요소 {#components-in-the-build-form-tab}

양식 **[!UICONTROL 작성]** 탭에는 스키마 양식에서 사용할 수 있는 항목이 나열됩니다. **[!UICONTROL 설정]** 탭은 양식 **[!UICONTROL 작성]** 탭에서 선택한 각 항목의 속성을 제공합니다. 다음 표에는 양식 **[!UICONTROL 작성]** 탭에서 사용할 수 있는 양식 항목이 나와 있습니다.

| 구성 요소 이름 | 설명 |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL 섹션 머리글] | 섹션 제목을 추가하여 공통 구성 요소 목록을 만듭니다. |
| [!UICONTROL 한 줄 텍스트] | 단일 행 텍스트 속성을 추가합니다. 문자열로 저장됩니다. |
| [!UICONTROL Multi valuetext] | 다중 값 텍스트 속성을 추가합니다. 문자열 배열로 저장됩니다. |
| [!UICONTROL 번호] | 숫자 구성 요소를 추가합니다. |
| [!UICONTROL 날짜] | 날짜 구성 요소를 추가합니다. |
| [!UICONTROL 드롭다운] | 드롭다운 목록을 추가합니다. |
| [!UICONTROL 표준 태그] | 태그 추가. **참고:** 관리자는 경로 값을 변경해야 할 수 있습니다. 예를 `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`들어, AEM에서 메타데이터 스키마 양식을 게시하면 경로에 임차인 정보가 포함되지 `/etc/tags/<custom_tag_namespace>`않습니다. |
| [!UICONTROL 스마트 태그] | AEM 스마트 태그 추가 기능을 구매 및 구성한 경우 자동으로 검색됩니다. |
| [!UICONTROL 숨김 필드] | 숨김 필드를 추가합니다. 자산이 저장될 때 post 매개 변수로 전송됩니다. |
| [!UICONTROL 자산 참조자] | 이 구성 요소를 추가하여 자산이 참조하는 자산의 목록을 봅니다. |
| [!UICONTROL 자산 참조] | 추가를 클릭하여 자산을 참조하는 자산 목록을 표시합니다. |
| [!UICONTROL 자산 등급] | 브랜드 포털에 게시되기 전에 AEM 자산에서 추가한 자산의 평균 등급. |
| [!UICONTROL 상황에 맞는 메타데이터] | Add to control the display of other metadata tabs of assets of assets. |

>[!NOTE]
>
>**[!UICONTROL 제품 참조는]**&#x200B;작동하지 않으므로 사용하지 마십시오.

#### 메타데이터 구성 요소 편집 {#edit-the-metadata-component}

양식에서 메타데이터 구성 요소의 속성을 편집하려면 구성 요소를 클릭하고 **[!UICONTROL 설정]** 탭에서 해당 속성을 편집합니다.

* **[!UICONTROL 필드 레이블]**: 자산의 속성 페이지에 표시되는 메타데이터 속성의 이름입니다.

* **[!UICONTROL 속성에 매핑]**: 이 속성의 값은 상대적 경로/이름을 CRX 저장소에서 저장할 자산 노드에 제공합니다. 다음으로 시작합니다&#x200B;**./**"경로가 자산의 노드 아래에 있음을 나타내기 때문입니다.

다음은 이 속성에 유효한 값입니다.

— [!UICONTROL `./jcr:content/metadata/dc:title`]: 자산의 메타데이터 노드에 값을 속성으로 [!UICONTROL `dc:title`]저장합니다.

— [!UICONTROL `./jcr:created`]: 자산의 노드에 jcr 속성을 표시합니다. 속성 보기에서 이러한 속성을 구성하는 경우 이러한 속성을 보호되어 있으므로 [편집 비활성화] 로 표시하는 것이 좋습니다. 그렇지 않으면 자산의 속성을 저장할 때 "에셋이 수정되지 못했습니다" 라는 오류가 발생합니다.

* **[!UICONTROL 자리 표시자]**: 이 속성을 사용하여 사용자에게 메타데이터 속성과 관련된 모든 정보를 제공합니다.
* ****&#x200B;필수: 속성 페이지에서 메타데이터 속성을 필수로 표시하려면 이 속성을 사용합니다.
* **[!UICONTROL 편집 비활성화]**: 속성 페이지에서 메타데이터 속성을 편집할 수 없게 하려면 이 속성을 사용합니다.
* **[!UICONTROL 읽기 전용 필드는 읽기 전용으로 표시]**: 값이 없는 경우에도 속성 페이지에 메타데이터 속성을 표시하려면 이 속성을 표시합니다. 기본적으로 메타데이터 속성에 값이 없으면 속성 페이지에 나열되지 않습니다.
* **[!UICONTROL 설명]**: 메타데이터 구성 요소에 대한 간단한 설명을 추가하려면 이 속성을 사용합니다.
* **[!UICONTROL 삭제 아이콘]**: 스키마 양식에서 구성 요소를 삭제하려면 이 아이콘을 클릭합니다.

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>모든 메타데이터 필드는 자산의 메타데이터 편집기 양식에서 읽기 전용입니다. 자산의 메타데이터는 브랜드 포털에 게시되기 전에 AEM 자산에서 편집해야 하므로

#### 스키마 양식에서 탭 추가 또는 삭제 {#add-or-delete-a-tab-in-the-schema-form}

기본 스키마 양식에는 **[!UICONTROL 기본]** 및 **[!UICONTROL 고급]** 탭이 포함됩니다. 스키마 편집기를 사용하여 탭을 추가하거나 삭제할 수 있습니다.

![](assets/add_delete_tabs_metadataschemaform.png)

* 스키마 양식에 새 탭을 추가하려면 **[!UICONTROL +]**&#x200B;를 클릭합니다. 기본적으로 새 탭의 이름은 "이름 없는 -1" 입니다. **[!UICONTROL 설정]** 탭에서 이름을 수정할 수 있습니다.

![](assets/add-tab-metadata-form.png)

* 탭을 삭제하려면 **[!UICONTROL X]**&#x200B;를 클릭합니다. Click **[!UICONTROL Save]** to save the changes.

## 폴더에 메타데이터 스키마 적용 {#apply-a-metadata-schema-to-a-folder}

브랜드 포털에서 자산의 [!UICONTROL 속성] 페이지에 표시하기 위해 선택한 정보만 표시하도록 메타데이터 스키마를 사용자 정의하고 제어할 수 있습니다. [!UICONTROL 속성] 페이지에 표시되는 메타데이터를 제어하려면 메타데이터 스키마 양식에서 필요한 메타데이터를 제거하고 해당 폴더에 적용합니다.

폴더에 메타데이터 스키마 양식을 적용하려면 다음을 수행하십시오.

1. 맨 위의 AEM 도구 모음에서 Adobe 로고를 클릭하여 관리 도구에 액세스합니다.

   ![](assets/aemlogo.png)

2. 관리 도구 패널에서 **[!UICONTROL 메타데이터 스키마를 클릭합니다]**.

3. **[!UICONTROL 메타데이터 스키마 양식]** 페이지에서 [!UICONTROL 옷 (예]: 옷) 에 적용할 스키마 양식을 선택합니다.

   ![](assets/apply-metadata-schema-form-to-folder.png)

4. 맨 위의 도구 모음에서 폴더에 **[!UICONTROL 적용을 클릭합니다]**.

5. 폴더 **[!UICONTROL 선택]** 페이지에서 **[!UICONTROL 의류]** 메타데이터 스키마를 적용할 폴더 (예: **[!UICONTROL 장갑]**) 로 이동합니다.

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

6. **[!UICONTROL 적용을]** 클릭하여 메타데이터 스키마 양식을 폴더에 적용합니다.

   **[!UICONTROL 의류]** 메타데이터 스키마 양식에서 사용할 수 있는 메타데이터는 **[!UICONTROL 장갑]** 폴더에 적용되며 폴더의 **[!UICONTROL 속성]** 페이지에 표시됩니다.

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>비디오 파일이 들어 있는 폴더에 중첩된 스키마가 포함된 스키마를 적용하는 경우 비디오 파일의 메타데이터 속성이 제대로 렌더링되지 않을 수 있습니다. 메타데이터 속성이 올바로 렌더링되도록 하려면 중첩 스키마를 제거하고 상위 스키마만 폴더에 적용합니다.

## Delete a metadata schema form {#delete-a-metadata-schema-form}

브랜드 포털에서 사용자 지정 스키마 양식만 삭제할 수 있습니다. 기본 스키마 양식/템플릿은 삭제할 수 없습니다. 그러나 이러한 양식에서 사용자 정의 변경 사항을 삭제할 수는 있습니다.

양식을 삭제하려면 양식을 선택하고 **[!UICONTROL 삭제]** 아이콘을 클릭합니다.

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>기본 양식의 사용자 지정 변경 내용을 삭제하면 메타데이터 스키마 인터페이스의 양식 이름 앞에 **[!UICONTROL 잠금]** 기호가 다시 나타나 양식이 기본 상태로 되돌려진다는 것을 나타냅니다.

## MIME 유형을 위한 스키마 양식 {#schema-forms-for-mime-types}

### MIME 유형에 대한 새 양식 추가 {#adding-new-forms-for-mime-types}

기본 양식 외에도, 다양한 MIME 유형의 자산에 대한 사용자 지정 양식을 추가하거나, 적절한 양식 유형 아래에 새 양식을 만들 수 있습니다. 예를 들어 **[!UICONTROL , 이미지/PNG]** 하위 유형에 대한 새 템플릿을 추가하려면 "이미지" 양식에 양식을 만듭니다. 스키마 양식의 제목은 하위 유형 이름입니다. 이 경우 제목은 "png" 입니다.

#### 다양한 MIME 유형에 기존 스키마 템플릿 사용 {#using-an-existing-schema-template-for-various-mime-types}

다른 MIME 유형에 기존 템플릿을 사용할 수 있습니다. 예를 들어 **이미지/JPEG** 형식을 MIME 유형의 **이미지/PNG에 사용합니다**.

이 경우 CRX 저장소에서 새 [!UICONTROL `/etc/dam/metadataeditor/mimetypemappings`] 노드를 만듭니다. 노드의 이름을 지정하고 다음 속성을 정의합니다.

| **이름** | **유형** | **값** |
|---|---|---|
| Exposedmimetype | 문자열 | image/jpeg |
| Mimetypes | String[] | image/png |

* **Exposedmimetype**: 매핑할 기존 양식의 이름
* **Mimetypes**: **Exposedmimetype** 속성에 정의된 양식을 사용하는 MIME 유형 목록

브랜드 포털은 다음 MIME 유형과 스키마 양식을 매핑합니다.

| **스키마 양식** | **MIME 유형** |
|---|---|
| image/jpeg | image/pjpeg |
| image/tiff | image/x-tiff |
| application/pdf | application/postscript |
| application/x-imageset | Multipart/Related; type=application/x-ImageSet |
| application/x-spinset | Multipart/Related; type=application/x-SpinSet |
| application/x-mixedmediaset | Multipart/Related; type=application/x-MixedMediaSet |
| video/quicktime | video/x-quicktime |
| Video/MPEG 4 | video/mp4 |
| 비디오/AVI | 비디오/avi, 비디오/msvideo, 비디오/x-msvideo |
| video/wmv | video/x-ms-wmv |
| 비디오/FLV | video/x-flv |

다음은 기본 메타데이터 속성 목록입니다.

* jcr:content/metadata/cq:tags
* jcr:content/metadata/dc:format
* jcr:content/metadata/dam:status
* JCR: 컨텐츠/메타데이터/Videocodec
* JCR: 컨텐츠/메타데이터/Audiocodec
* JCR: 컨텐츠/메타데이터/DC: title
* JCR: 컨텐츠/메타데이터/DC: description
* JCR: content/metadata/xmpmm: Instanceid
* JCR: content/metadata/xmpmm: Documentid
* JCR: 컨텐츠/메타데이터/DAM: SHA 1
* JCR: 컨텐츠/메타데이터/DAM: Solutioncontext
* JCR: content/metadata/videobitrate
* JCR: content/metadata/audiobitrate
* JCR: 컨텐츠/사용/Usedby
* jcr:content/jcr:lastModified
* jcr:content/metadata/prism:expirationDate
* JCR: 컨텐츠/Ontime
* JCR: 컨텐츠/해제 시간
* jcr:content/metadata/dam:size
* JCR: content/metadata/tiff: Imagewidth
* JCR: content/metadata/tiff: Imagelength
