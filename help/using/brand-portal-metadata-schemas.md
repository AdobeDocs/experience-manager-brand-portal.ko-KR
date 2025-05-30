---
title: 메타데이터 스키마 양식 사용
description: 메타데이터 스키마는 속성 페이지의 레이아웃과 특정 스키마를 사용하는 자산에 대해 표시되는 메타데이터 속성을 설명합니다. 에셋에 적용하는 스키마는 해당 속성 페이지에 나타나는 메타데이터 필드를 결정합니다.
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: administration
role: Admin
exl-id: fbedff90-a6cb-4175-8308-817cc9f5b450
source-git-commit: e01be07e7e791c6d406744148a77fd44d2479734
workflow-type: tm+mt
source-wordcount: '1603'
ht-degree: 5%

---

# 메타데이터 스키마 양식 사용 {#use-the-metadata-schema-form}

메타데이터 스키마는 속성 페이지의 레이아웃과 특정 스키마를 사용하는 자산에 대해 표시되는 메타데이터 속성을 설명합니다. 에셋에 적용하는 스키마는 해당 속성 페이지에 나타나는 메타데이터 필드를 결정합니다.

각 에셋에 대한 **[!UICONTROL 속성]** 페이지에는 에셋의 MIME 유형에 따라 기본 메타데이터 속성이 포함됩니다. 관리자는 메타데이터 스키마 편집기를 사용하여 기존 스키마를 수정하거나 사용자 지정 메타데이터 스키마를 추가할 수 있습니다. Experience Manager Assets Brand Portal은 다양한 MIME 유형의 자산에 대한 기본 양식을 제공합니다. 그러나 이러한 에셋에 대한 사용자 정의 양식을 추가할 수도 있습니다.

## 메타데이터 스키마 양식 추가 {#add-a-metadata-schema-form}

새 메타데이터 스키마 양식을 생성하려면 다음을 수행합니다.

1. 상단의 도구 모음에서 Experience Manager 로고를 클릭하여 관리 도구에 액세스합니다.

   ![](assets/aemlogo.png)

1. 관리 도구 패널에서 **[!UICONTROL 메타데이터 스키마]**&#x200B;를 클릭합니다.

   ![](assets/navigation-panel.png)

1. **[!UICONTROL 메타데이터 스키마 Forms]** 페이지에서 **[!UICONTROL 만들기]**&#x200B;를 클릭합니다.

   ![](assets/create-metadata-schema-form.png)

1. **[!UICONTROL 스키마 양식 만들기]** 대화 상자에서 스키마 양식의 제목을 지정한 다음 **[!UICONTROL 만들기]**&#x200B;를 클릭하여 양식 만들기 프로세스를 완료합니다.

   ![](assets/create-schema-form.png)

## 메타데이터 스키마 양식 편집 {#edit-a-metadata-schema-form}

추가되거나 기존 메타데이터 스키마 양식은 모두 편집할 수 있습니다. 메타데이터 스키마 양식에는 탭 및 탭 내의 양식 항목을 포함하여 상위 항목에서 파생된 콘텐츠가 포함되어 있습니다. 이러한 양식 항목을 메타데이터 노드 내의 필드에 매핑하거나 구성할 수 있습니다.

메타데이터 스키마 양식에 새 탭이나 양식 항목을 추가할 수 있습니다. 파생 탭과 양식 항목(상위 항목)이 잠긴 상태입니다. 하위 수준에서는 변경할 수 없습니다.

메타데이터 스키마 양식을 편집하려면 다음을 수행합니다.

1. 상단의 도구 모음에서 Experience Manager 로고를 클릭하여 관리 도구에 액세스합니다.

   ![](assets/aemlogo.png)

1. 관리 도구 패널에서 **[!UICONTROL 메타데이터 스키마]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 메타데이터 스키마 Forms]** 페이지에서 속성을 편집할 스키마 양식을 선택합니다(예: **[!UICONTROL collection]**).

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >편집되지 않은 템플릿에는 앞에 잠금 기호가 표시됩니다. 템플릿을 사용자 정의하는 경우 템플릿 앞에 있는 잠금 기호가 사라집니다.

1. 상단의 도구 모음에서 **[!UICONTROL 편집]**&#x200B;을 클릭합니다.

   **[!UICONTROL 메타데이터 스키마 편집기]** 페이지가 열리고 왼쪽에 **[!UICONTROL 기본]** 탭이 열립니다. 오른쪽에는 **[!UICONTROL 양식 작성]** 탭이 열립니다.

1. **[!UICONTROL 메타데이터 스키마 편집기]** 페이지에서 자산의 **[!UICONTROL 속성]** 페이지를 사용자 지정합니다. **[!UICONTROL 양식 작성]** 탭의 구성 요소 형식 목록에서 구성 요소를 하나 이상 끌어 놓기만 하면 됩니다. **[!UICONTROL 기본]** 탭으로 끌어 놓으십시오.

   ![](assets/metadata-schemaeditor-page.png)

1. 구성 요소를 구성하려면 구성 요소를 선택하고 **[!UICONTROL 설정]** 탭에서 속성을 수정하십시오.

### 양식 작성 탭의 구성 요소 {#components-in-the-build-form-tab}

**[!UICONTROL 양식 작성]** 탭에는 스키마 양식에 사용할 수 있는 항목이 나열됩니다. **[!UICONTROL 설정]** 탭은 **[!UICONTROL 양식 작성]** 탭에서 선택한 각 항목의 특성을 제공합니다. 다음 표에는 **[!UICONTROL 양식 작성]** 탭에서 사용할 수 있는 양식 항목이 나열되어 있습니다.

| 구성 요소 이름 | 설명 |
|----|----|
| **[!UICONTROL 섹션 머리글]** | 공통 구성 요소 목록의 섹션 머리글을 추가합니다. |
| **[!UICONTROL 한 줄 텍스트]** | 한 줄 텍스트 속성을 추가합니다. 문자열로 저장됩니다. |
| **[!UICONTROL 다중 값 텍스트]** | 다중 값 텍스트 속성을 추가합니다. 문자열 배열로 저장됩니다. |
| **[!UICONTROL 숫자]** | 숫자 구성 요소를 추가합니다. |
| **[!UICONTROL 날짜]** | 날짜 구성 요소를 추가합니다. |
| **[!UICONTROL 드롭다운]** | 드롭다운 목록을 추가합니다. |
| **[!UICONTROL 표준 태그]** | 태그를 추가합니다. 관리자는 경로 값을 변경해야 할 수 있습니다. 예를 들어, `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`이(가) Experience Manager Assets에서 메타데이터 스키마 양식을 게시하는 경우 경로에 테넌트 정보(예: `/etc/tags/<custom_tag_namespace>`)가 포함되어 있지 않습니다. |
| **[!UICONTROL 스마트 태그]** | Experience Manager Assets 스마트 태그 추가 기능을 구매하고 구성한 경우 태그가 자동으로 검색됩니다. |
| **[!UICONTROL 숨겨진 필드]** | 숨겨진 필드를 추가합니다. 자산이 저장될 때 POST 매개 변수로 전송됩니다. |
| **[!UICONTROL 자산 참조자]** | 이 구성 요소를 추가하여 에셋에서 참조한 에셋 목록을 확인하십시오. |
| **[!UICONTROL 자산 참조]** | 를 추가하여 에셋을 참조하는 에셋 목록을 표시합니다. |
| **[!UICONTROL 컨텍스트 메타데이터]** | 를 추가하여 자산의 속성 페이지에서 다른 메타데이터 탭의 표시를 제어합니다. |

<!--| **[!UICONTROL Asset Rating]** |  Average rating of an asset added from Experience Manager Assets before it is published to Brand Portal. |-->

>[!NOTE]
>
>작동하지 않으므로 **[!UICONTROL 제품 참조]**&#x200B;를 사용하지 마십시오.

#### 메타데이터 구성 요소 편집 {#edit-the-metadata-component}

양식의 메타데이터 구성 요소 속성을 편집하려면 구성 요소를 클릭하고 **[!UICONTROL 설정]** 탭에서 해당 속성을 편집하십시오.

* **[!UICONTROL 필드 레이블]**: 자산의 속성 페이지에 표시되는 메타데이터 속성의 이름입니다.

* **[!UICONTROL 속성에 매핑]**: 이 속성의 값은 CRX 저장소에 저장된 에셋 노드에 대한 상대 경로/이름을 제공합니다. &quot;**&quot;(으)로 시작합니다.경로가 자산의 노드 아래에 있음을 나타내므로 /**&quot;.

다음은 이 속성에 유효한 값입니다.

— `./jcr:content/metadata/dc:title`: 자산의 메타데이터 노드에 있는 값을 속성 `dc:title`(으)로 저장합니다.

— `./jcr:created`: 자산의 노드에 jcr 속성을 표시합니다. 보기 속성에 대해 이러한 속성을 구성한 경우 Adobe에서는 속성이 보호되므로 이를 편집 비활성화로 표시하는 것이 좋습니다. 그렇지 않으면 자산의 속성을 저장할 때 &quot;Assets이 수정되지 않음&quot; 오류가 발생합니다.

* **[!UICONTROL 자리 표시자]**: 이 속성을 사용하여 메타데이터 속성과 관련된 모든 관련 정보를 사용자에게 제공합니다.
* **[!UICONTROL 필수]**: 이 속성을 사용하여 메타데이터 속성을 속성 페이지에서 필수로 표시합니다.
* **[!UICONTROL 편집 사용 안 함]**: 이 속성을 사용하여 속성 페이지에서 메타데이터 속성을 편집할 수 없게 만듭니다.
* **[!UICONTROL 읽기 전용에 빈 필드 표시]**: 값이 없는 경우에도 속성 페이지에 메타데이터 속성을 표시하려면 이 속성을 표시하십시오. 기본적으로 메타데이터 속성에 값이 없으면 속성 페이지에 나열되지 않습니다.
* **[!UICONTROL 설명]**: 메타데이터 구성 요소에 대한 간단한 설명을 추가하려면 이 속성을 사용합니다.
* **[!UICONTROL 삭제 아이콘]**: 스키마 양식에서 구성 요소를 삭제하려면 이 아이콘을 클릭하십시오.

  ![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>에셋의 메타데이터 편집기 양식에서 모든 메타데이터 필드는 읽기 전용입니다. 에셋이 Brand Portal에 게시되기 전에 Experience Manager Assets에서 에셋의 메타데이터를 편집해야 하기 때문입니다.

#### 스키마 양식에서 탭 추가 또는 삭제 {#add-or-delete-a-tab-in-the-schema-form}

기본 스키마 양식에는 **[!UICONTROL 기본]** 및 **[!UICONTROL 고급]** 탭이 있습니다. 스키마 편집기를 사용하여 탭을 추가하거나 삭제할 수 있습니다.

![](assets/add_delete_tabs_metadataschemaform.png)

* 스키마 양식에 새 탭을 추가하려면 **[!UICONTROL +]**&#x200B;을(를) 클릭합니다. 기본적으로 새 탭의 이름은 &quot;Unnamed-1&quot;입니다. **[!UICONTROL 설정]** 탭에서 이름을 수정할 수 있습니다.

  ![](assets/add-tab-metadata-form.png)

* 탭을 삭제하려면 **[!UICONTROL x]**&#x200B;을(를) 클릭합니다. **[!UICONTROL 저장]**&#x200B;을 클릭하여 변경 내용을 저장합니다.

## 폴더에 메타데이터 스키마 적용 {#apply-a-metadata-schema-to-a-folder}

Brand Portal을 사용하면 에셋의 **[!UICONTROL 속성]** 페이지에 표시할 특정 정보만 표시되도록 메타데이터 스키마를 사용자 지정하고 제어할 수 있습니다. **[!UICONTROL 속성]** 페이지에 표시되는 메타데이터를 제어하려면 메타데이터 스키마 양식에서 필요한 메타데이터를 제거하고 특정 폴더에 적용합니다.

폴더에 메타데이터 스키마 양식을 적용하려면 다음을 수행합니다.

1. 상단의 도구 모음에서 Experience Manager 로고를 클릭하여 관리 도구에 액세스합니다.

   ![](assets/aemlogo.png)

1. 관리 도구 패널에서 **[!UICONTROL 메타데이터 스키마]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 메타데이터 스키마 Forms]** 페이지에서 에셋에 적용할 스키마 양식(예: **[!UICONTROL 의류]**)을 선택합니다.

   ![](assets/apply-metadata-schema-form-to-folder.png)

1. 상단의 도구 모음에서 **[!UICONTROL 폴더에 적용]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 폴더 선택]** 페이지에서 **[!UICONTROL 의류]** 메타데이터 스키마를 적용할 폴더로 이동합니다(예: **[!UICONTROL 장갑]**).

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

1. 폴더에 메타데이터 스키마 양식을 적용하려면 **[!UICONTROL 적용]**&#x200B;을 클릭하십시오.

   **[!UICONTROL 의류]** 메타데이터 스키마 양식에서 사용할 수 있는 메타데이터는 **[!UICONTROL 장갑]** 폴더에 적용되며 폴더의 **[!UICONTROL 속성]** 페이지에 표시됩니다.

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>중첩된 스키마가 포함된 스키마를 비디오 파일이 포함된 폴더에 적용하면 비디오 파일에 대한 메타데이터 속성이 제대로 렌더링되지 않을 수 있습니다. 메타데이터 속성이 올바르게 렌더링되도록 하려면 중첩된 스키마를 제거하고 상위 스키마만 폴더에 적용합니다.

## 메타데이터 스키마 양식 삭제 {#delete-a-metadata-schema-form}

Brand Portal을 사용하면 사용자 정의 스키마 양식만 삭제할 수 있습니다. 기본 스키마 양식/템플릿을 삭제할 수는 없습니다. 그러나 이러한 양식에서 사용자 정의 변경 사항을 삭제할 수 있습니다.

양식을 삭제하려면 양식을 선택하고 **[!UICONTROL 삭제]** 아이콘을 클릭합니다.

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>기본 양식에 대한 사용자 지정 변경 내용을 삭제한 후 메타데이터 스키마 인터페이스에서 양식 이름 앞에 **[!UICONTROL Lock]** 기호가 다시 표시되어 양식이 기본 상태로 되돌아갔음을 나타냅니다.

## MIME 유형에 대한 스키마 양식 {#schema-forms-for-mime-types}

### MIME 유형에 대한 새 양식 추가 {#adding-new-forms-for-mime-types}

기본 양식 외에도 다양한 MIME 유형의 자산에 대한 사용자 정의 양식을 추가하거나 적절한 양식 유형에서 새 양식을 만들 수 있습니다. For example, to add a new template for the **[!UICONTROL image/png]** subtype, create the form under the &quot;image&quot; forms. The title for the schema form is the subtype name. 이 경우 제목은 &quot;png&quot;입니다.

#### 다양한 MIME 유형에 기존 스키마 템플릿 사용 {#using-an-existing-schema-template-for-various-mime-types}

다른 MIME 유형에 기존 템플릿을 사용할 수 있습니다. 예를 들어 MIME 유형 **image/png**&#x200B;의 자산에 대해 **image/jpeg** 양식을 사용하십시오.

이 경우 CRX 저장소의 [!UICONTROL `/etc/dam/metadataeditor/mimetypemappings`]에 새 노드를 만듭니다. 노드 이름을 지정하고 다음 속성을 정의합니다.

| **이름** | **유형** | **값** |
|---|---|---|
| exposedmimetype | 문자열 | image/jpeg |
| mime 유형 | 문자열[] | image/png |

* **exposedmimetype**: 매핑할 기존 양식의 이름
* **mime 형식**: **exposedmimetype** 특성에 정의된 양식을 사용하는 MIME 형식 목록입니다

Brand Portal은 다음 MIME 유형 및 스키마 양식을 매핑합니다.

| **스키마 양식** | **MIME 유형** |
|---|---|
| image/jpeg | image/pjpeg |
| image/tiff | image/x-tiff |
| application/pdf | application/postscript |
| application/x-ImageSet | Multipart/Related; type=application/x-ImageSet |
| application/x-SpinSet | Multipart/Related; type=application/x-SpinSet |
| application/x-MixedMediaSet | Multipart/Related; type=application/x-MixedMediaSet |
| video/quicktime | video/x-quicktime |
| video/mpeg4 | video/mp4 |
| video/avi | video/avi, video/msvideo, video/x-msvideo |
| video/wmv | `video/x-ms-wmv` |
| video/flv | video/x-flv |

다음은 기본 메타데이터 속성 목록입니다.

* `jcr:content/metadata/cq:tags`
* `jcr:content/metadata/dc:format`
* `jcr:content/metadata/dam:status`
* `jcr:content/metadata/videoCodec`
* `jcr:content/metadata/audioCodec`
* `jcr:content/metadata/dc:title`
* `jcr:content/metadata/dc:description`
* `jcr:content/metadata/xmpMM:InstanceID`
* `jcr:content/metadata/xmpMM:DocumentID`
* `jcr:content/metadata/dam:sha1`
* `jcr:content/metadata/dam:solutionContext`
* `jcr:content/metadata/videoBitrate`
* `jcr:content/metadata/audioBitrate`
* `jcr:content/usages/usedBy`
* `jcr:content/jcr:lastModified`
* `jcr:content/metadata/prism:expirationDate`
* `jcr:content/onTime`
* `jcr:content/offTime`
* `jcr:content/metadata/dam:size`
* `jcr:content/metadata/tiff:ImageWidth`
* `jcr:content/metadata/tiff:ImageLength`
