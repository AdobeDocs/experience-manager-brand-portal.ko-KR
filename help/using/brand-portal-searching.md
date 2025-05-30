---
title: Brand Portal에서 자산 검색
description: Brand Portal 검색 기능을 사용하면 Omnisearch를 사용하여 관련 에셋을 빠르게 검색할 수 있으며, 검색 필터를 사용하면 검색 범위를 더욱 좁힐 수 있습니다. 나중에 스마트 컬렉션으로 검색을 저장합니다.
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
exl-id: 7297bbe5-df8c-4d0b-8204-218a9fdc2292
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '1343'
ht-degree: 0%

---

# Brand Portal에서 자산 검색 {#search-assets-on-brand-portal}

Brand Portal 검색 기능을 사용하면 Omnisearch 및 필터를 사용하여 검색 범위를 좁히는 데 도움이 되는 패싯 검색을 사용하여 관련 에셋을 빠르게 검색할 수 있습니다. 파일 또는 폴더 수준에서 자산을 검색하고 검색 결과를 스마트 컬렉션으로 저장할 수 있습니다.

>[!NOTE]
>
>Brand Portal은 Omnisearch를 사용한 컬렉션 검색을 지원하지 않습니다.
>
>그러나 [검색 필터를 사용하여 관련 컬렉션 목록을 가져올 수 있습니다](#search-collection).

## Omnisearch를 사용하여 에셋 검색 {#search-assets-using-omnisearch}

Brand Portal에서 자산을 검색하려면 다음을 수행하십시오.

1. 도구 모음에서 **[!UICONTROL 검색]** 아이콘을 클릭하거나 **[!UICONTROL /]**(슬래시) 키를 눌러 Omnisearch를 시작합니다.

   ![](assets/omnisearchicon-1.png)

1. 검색 상자에 검색할 에셋의 키워드를 입력합니다.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >* 검색 제안을 표시하려면 Omnisearch에 최소 3자가 필요합니다.
   >* `mountain biking`을(를) 검색하면 Omnisearch는 메타데이터 필드에서 `mountain`과(와) `biking`을(를) 모두 사용할 수 있는 모든 자산을 검색 결과에 반환합니다. 예를 들어 `Title` 필드의 `mountain` 및 `Description` 필드의 `biking`입니다. 두 용어 모두 메타데이터 필드에서 사용할 수 있어야 검색 결과에 표시할 수 있습니다. 그러나 Omnisearch는 스마트 태그 메타데이터 필드에서 두 용어 중 하나만 사용할 수 있는 경우에도 검색 결과에 에셋을 반환합니다. 예를 들어 에셋에 스마트 태그로서 `mountain`이(가) 있지만 다른 메타데이터 필드에는 `biking`이(가) 없다고 가정합니다. `mountain biking`을(를) 검색합니다. Omnisearch는 여전히 검색 결과에 에셋을 반환합니다. 이 워크플로우는 관련 태그가 있는 에셋이 누락되지 않도록 합니다.

1. 관련 에셋에 빠르게 액세스하려면 드롭다운 목록에 표시되는 관련 제안 중에서 선택합니다.

   ![](assets/assets-search-result.png)

   *Omnisearch를 사용한 자산 검색*

스마트 태그가 지정된 자산을 사용한 검색 동작에 대해 자세히 알아보려면 [검색 결과 및 동작 이해](https://experienceleague.adobe.com/ko/docs/experience-manager-65/content/assets/using/search-assets)(으)로 이동하십시오.

## 필터 패널에서 패싯을 사용하여 검색 {#search-using-facets-in-filters-panel}

필터 패널의 검색 패싯은 검색 경험에 세부 기간을 추가하고 검색 기능을 보다 효율적으로 만듭니다. 검색 패싯은 복잡한 검색을 수행할 수 있도록 해주는 여러 차원(술어)을 사용합니다. 원하는 세부 수준으로 쉽게 드릴다운하여 보다 집중적인 검색을 수행할 수 있습니다.

예를 들어 이미지를 찾는 경우 비트맵 이미지를 원하는지 벡터 이미지를 원하는지 선택할 수 있습니다. 파일 유형 검색 패싯에서 이미지의 MIME 유형을 지정하여 검색 범위를 더 좁힐 수 있습니다. 마찬가지로 문서를 검색할 때 PDF 또는 MS® Word 형식과 같은 형식을 지정할 수 있습니다.

![Brand Portal의 필터 패널](assets/file-type-search.png "Brand Portal의 필터 패널")

**[!UICONTROL 필터]** 패널에는 **[!UICONTROL 경로 브라우저]**, **[!UICONTROL 파일 형식]**, **[!UICONTROL 파일 크기]**, **[!UICONTROL 상태]** 및 **[!UICONTROL 방향]**&#x200B;과 같은 몇 가지 표준 패싯이 포함되어 있습니다.
그러나 [사용자 지정 검색 패싯을 추가](../using/brand-portal-search-facets.md)하거나 **[!UICONTROL 필터]** 패널에서 특정 검색 패싯을 제거할 수 있습니다. 기본 검색 양식에서 술어를 편집하기만 하면 됩니다. 사용 가능하고 사용 가능한 [Brand Portal의 검색 조건자](../using/brand-portal-search-facets.md#list-of-search-predicates) 목록을 확인하십시오.

사용 가능한 [검색 패싯](../using/brand-portal-search-facets.md)을 사용하여 검색에 필터를 적용하려면:

1. 오버레이 아이콘을 클릭하고 **[!UICONTROL 필터]**&#x200B;를 선택합니다.

   ![](assets/selectorrail.png)

1. 왼쪽의 **[!UICONTROL 필터]** 패널에서 적절한 옵션을 선택하여 관련 필터를 적용합니다.
예를 들어 다음 표준 필터를 사용합니다.

   * 특정 디렉터리에서 자산을 검색할 **[!UICONTROL 경로 브라우저]**. 경로 브라우저에 대한 조건자의 기본 검색 경로는 `/content/dam/mac/<tenant-id>/`이며, 기본 검색 양식을 편집하여 구성할 수 있습니다.

   >[!NOTE]
   >
   >관리자가 아닌 사용자는 [!UICONTROL 필터] 패널의 [!UICONTROL 경로 브라우저]에 공유된 폴더(및 상위 폴더)의 콘텐츠 구조만 표시됩니다.\
   >관리 사용자를 위해 경로 브라우저를 사용하여 Brand Portal의 모든 폴더로 이동할 수 있습니다.

   * **[!UICONTROL 파일 형식]**: 원하는 자산 파일의 형식(이미지, 문서, 멀티미디어, 보관)을 지정합니다. 또한 검색 범위를 좁힐 수 있습니다. 예를 들어 이미지에 대한 MIME 유형(Tiff, 비트맵, GIMP 이미지)이나 문서에 대한 형식(PDF 또는 MS® Word)을 지정할 수 있습니다.
   * 크기를 기준으로 자산을 검색하려면 **[!UICONTROL 파일 크기]**. 크기 범위의 하한과 상한을 지정하여 검색 범위를 좁히고 검색할 측정 단위를 지정할 수 있습니다.
   * 승인(승인됨, 변경 요청, 거부됨, 보류 중) 및 만료와 같은 에셋 상태를 기준으로 에셋을 검색하려면 **[!UICONTROL 상태]**.
   * 에셋의 등급을 기준으로 에셋을 검색할 **[!UICONTROL 평균 등급]**.
   * **[!UICONTROL 방향]** - 자산의 방향(가로, 세로, 사각형)을 기준으로 자산을 검색합니다.
   * **[!UICONTROL 스타일]** - 에셋의 스타일(컬러, 단색)을 기준으로 에셋을 검색합니다.
   * **[!UICONTROL 비디오 형식]** - 해당 형식(DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM)을 기준으로 비디오 자산을 검색합니다.

   기본 검색 양식을 편집하여 필터 패널에서 [사용자 지정 검색 패싯](../using/brand-portal-search-facets.md)을 사용할 수 있습니다.

   * **[!UICONTROL 속성 조건자]** 검색 양식에서 사용하는 경우 조건자가 매핑된 메타데이터 속성과 일치하는 에셋을 검색할 수 있습니다.\
     예를 들어 속성 조건자가 `jcr:content/metadata/dc:title`에 매핑되어 있으면 제목을 기반으로 에셋을 검색할 수 있습니다.\
     [!UICONTROL 속성 조건자]는 다음에 대한 텍스트 검색을 지원합니다.

     **부분 구문**
속성 조건부에서 부분 구문을 사용하여 자산 검색을 허용하려면 검색 양식에서 **[!UICONTROL 부분 검색]** 확인란을 활성화하십시오. 이 방법을 사용하면 에셋 메타데이터에 사용된 단어 또는 구문을 정확히 지정하지 않더라도 원하는 에셋을 검색할 수 있습니다.

     >[!NOTE]
     >
     > Brand Portal은 부분 검색에 대해 다음 필드를 지원합니다.
     >
     >* `jcr:content/metadata/dc:title`
     >* `jcr:content/jcr:title`
     >* `jcr:content/metadata/dc:format`

     다음과 같은 작업을 수행할 수 있습니다.
      * 필터 패널에서 패싯의 검색한 구문에서 발생하는 단어를 지정합니다. 예를 들어 용어 **climb**&#x200B;을 검색하는 경우(그리고 속성 조건부가 `dc:title` 속성에 매핑됨) 제목 구문에 **climb**&#x200B;이라는 단어가 포함된 모든 자산이 반환됩니다.
      * 검색한 구문에서 발생하는 단어의 일부와 와일드카드 문자(&#42;)를 지정하여 간격을 채웁니다.
예를 들어 다음을 검색할 수 있습니다.
         * **climb&#42;**&#x200B;은(는) 제목 구문에 &quot;climb&quot; 문자로 시작하는 단어가 포함된 모든 자산을 반환합니다.
         * **&#42;climb**&#x200B;은(는) 제목 구문에 &quot;climb&quot; 문자로 끝나는 단어가 있는 모든 자산을 반환합니다.
         * **&#42;climb&#42;**&#x200B;은(는) 제목 구문에 &quot;climb&quot; 문자가 포함된 단어가 있는 모든 자산을 반환합니다.

     **대/소문자를 구분하지 않는 텍스트**
속성 조건자에서 대소문자를 구분하지 않는 검색을 허용할 수 있습니다. 검색 양식에서 **[!UICONTROL 대소문자 구분 안 함]** 확인란을 활성화하기만 하면 됩니다. 기본적으로 속성 조건자의 텍스트 검색은 대/소문자를 구분합니다.

   >[!NOTE]
   >
   >**[!UICONTROL 부분 검색]** 확인란을 선택하면 기본적으로 **[!UICONTROL 대/소문자 구분 안 함]**&#x200B;이 선택됩니다.

   ![](assets/wildcard-prop-1.png)

   검색 결과는 검색 결과 카운트와 함께 적용된 필터에 따라 표시됩니다.

   ![](assets/omnisearch-with-filters.png)

   검색 결과 카운트가 포함된 에셋 검색 결과.

1. 검색 쿼리를 다시 실행하지 않고도 검색 결과에서 항목을 쉽게 탐색하고 브라우저의 뒤로 단추를 사용하여 동일한 검색 결과로 돌아갈 수 있습니다.

## 검색을 스마트 컬렉션으로 저장 {#save-your-searches-as-smart-collection}

나중에 동일한 설정을 다시 실행하지 않고도 동일한 검색을 빠르게 반복할 수 있도록 검색 설정을 스마트 컬렉션으로 저장할 수 있습니다. 하지만 컬렉션에서는 검색 필터를 적용할 수 없습니다.

검색 설정을 스마트 컬렉션으로 저장하려면 다음을 수행합니다.

1. **[!UICONTROL 스마트 컬렉션 저장]**&#x200B;을 클릭하고 스마트 컬렉션의 이름을 제공합니다.

   모든 사용자가 스마트 컬렉션에 액세스할 수 있도록 하려면 **[!UICONTROL 공개]**&#x200B;를 선택하세요. 스마트 컬렉션이 생성되어 저장된 검색 목록에 추가되었음을 확인하는 메시지가 표시됩니다.

   >[!NOTE]
   >
   >조직의 Brand Portal에 관리자가 아닌 사용자가 만든 공용 스마트 컬렉션이 너무 많이 생성되지 않도록 관리자가 아닌 사용자가 스마트 컬렉션을 공개하지 못하도록 제한할 수 있습니다. 조직은 관리 도구 패널에서 사용할 수 있는 **[!UICONTROL 일반]** 설정에서 **[!UICONTROL 공용 스마트 컬렉션 만들기 허용]** 구성을 비활성화할 수 있습니다.

   ![](assets/save_smartcollectionui.png)

1. 스마트 컬렉션을 다른 이름으로 저장하고 **[!UICONTROL 공개]** 확인란을 선택하거나 선택을 취소하려면 **[!UICONTROL 스마트 컬렉션 편집]**&#x200B;을 클릭합니다.

   ![](assets/edit_smartcollection.png)

1. **[!UICONTROL 스마트 컬렉션 편집]** 대화 상자에서 **[!UICONTROL 다른 이름으로 저장]**&#x200B;을 선택하고 스마트 컬렉션의 이름을 입력합니다. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   ![](assets/saveas_smartsearch.png)


## 컬렉션 검색 {#search-collection}

컬렉션에 대해서는 Omnisearch가 지원되지 않습니다. 그러나 검색 필터를 적용하여 [!UICONTROL 컬렉션] 인터페이스 내에서 관련 컬렉션을 나열할 수 있습니다.

[!UICONTROL 컬렉션] 인터페이스에서 오버레이 아이콘을 클릭하여 왼쪽 레일에서 필터 패널을 엽니다. 사용 가능한 필터(`modified date`, `access type` 및 `tags`)에서 단일 또는 여러 검색 필터를 적용합니다. 적용된 필터를 기반으로 가장 관련성이 높은 컬렉션 세트를 나열합니다.

![](assets/collection-search.png)
