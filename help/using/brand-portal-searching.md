---
title: 브랜드 포털에서 자산 검색
seo-title: AEM 브랜드 포털에서 자산 검색 및 저장된 검색
description: 브랜드 포털 검색 기능을 사용하면 옴니서치를 사용하여 관련 자산을 신속하게 검색할 수 있으며 검색 필터를 통해 검색 범위를 좁힐 수 있습니다. 나중에 스마트 컬렉션으로 검색을 저장할 수 있습니다.
seo-description: 브랜드 포털 검색 기능을 사용하면 옴니서치를 사용하여 관련 자산을 신속하게 검색할 수 있으며 검색 필터를 통해 검색 범위를 좁힐 수 있습니다. 나중에 스마트 컬렉션으로 검색을 저장할 수 있습니다.
uuid: c295198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: 참조
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
translation-type: tm+mt
source-git-commit: 9763a57a83db22cd6686701dcbd8fcde16bcbb31

---


# 브랜드 포털에서 자산 검색 {#search-assets-on-brand-portal}

브랜드 포털 검색 기능을 사용하면 옴니셔와 필터를 사용하여 검색 범위를 좁히는 면처리된 검색을 통해 관련 자산을 신속하게 검색할 수 있습니다. 나중에 검색을 스마트 컬렉션으로 저장할 수도 있습니다.

## Omnisearch를 사용하여 자산 검색 {#search-assets-using-omnisearch}

To search for assets on Brand Portal:

1. 도구 모음에서 검색 **[!UICONTROL 아이콘을 클릭하거나]** "**[!UICONTROL /]**" 키를 눌러 Omnisearch를 시작합니다.

   ![](assets/omnisearchicon-1.png)

1. In the search box, type a keyword for the assets you want to search.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >At least 3 characters are required in omnisearch for search suggestions to appear.

1. Select from the related suggestions that appear in the drop-down list to quickly access relevant assets.

   ![](assets/assets-search-result.png)

   *Asset search using omnisearch*

To know about search behaviour with smart tagged assets, see understand search results and behavior.[](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-assets.html)

## Search using facets in Filters panel {#search-using-facets-in-filters-panel}

Search facets in the Filters panel add granularity to your search experience and make the search functionality efficient. Search facets use multiple dimensions (predicates) that enable you to perform intricate searches. You can easily drill down to the desired level of detail for a more focused search.

For example, if you are looking for an image, you can choose whether you want a bitmap or a vector image. You can reduce the scope of search further by specifying the MIME type for the image in the File Type search facet. Similarly, when searching for documents, you can specify the format, for example, PDF or MS Word format.<br />

![Filters panel in Brand PortalFilters panel in Brand Portal](assets/file-type-search.png "")

[ [!UICONTROL 필터] ] 패널에는 [!UICONTROL 경로 브라우저], [!UICONTROL 경로 유형], [!UICONTROL 파일 크기], 파일 [!UICONTROL 방향,]위치, 상태 및 시간 초과, 시간 초과, However, you can add custom search facets or remove specific search facets from the Filters panel by adding or removing predicates in the underlying Search Form. [](../using/brand-portal-search-facets.md) 브랜드 포털에서 사용 가능한 [검색 예측 목록을 참조하십시오](../using/brand-portal-search-facets.md#list-of-search-predicates).

사용 가능한 [검색 패싯을](../using/brand-portal-search-facets.md)사용하여 검색에 필터를 적용하려면:

1. 오버레이 아이콘을 클릭하고 필터를 **[!UICONTROL 선택합니다]**.

   ![](assets/selectorrail.png)

2. 왼쪽의 **[!UICONTROL [필터]** ] 패널에서 적절한 옵션을 선택하여 관련 필터를 적용합니다.
예를 들어 다음 표준 필터를 사용합니다.

   * **[!UICONTROL 경로]** 브라우저를 사용하여 특정 디렉토리에서 자산을 검색합니다. 경로 브라우저에 대한 조건자의 기본 검색 경로는 **[!UICONTROL /content/dam/mac/&lt;tenant-id&gt;/]**&#x200B;이며 기본 검색 양식을 편집하여 구성할 수 있습니다.
   >[!NOTE]
   >
   >관리자가 아닌 사용자에게 필터 [!UICONTROL 패널의] 경로 브라우저는 [!UICONTROL 해당] 사용자와 공유된 폴더의 컨텐츠 구조만 표시합니다.\
   >사용자를 관리하기 위해 경로 브라우저를 사용하면 브랜드 포털의 모든 폴더로 이동할 수 있습니다.

   * **[!UICONTROL 파일]** 유형을 사용하여 원하는 에셋 파일의 유형(이미지, 문서, 멀티미디어, 아카이브)을 지정합니다. 또한 검색의 범위를 좁힐 수 있습니다. 예를 들어 문서의 이미지 또는 형식(PDF 또는 MS Word)에 대한 MIME 유형(Tiff, Bitmap, GIMP Images)을 지정할 수 있습니다.
   * **[!UICONTROL 파일]** 크기를 기준으로 자산을 검색할 수 있습니다. 크기 범위의 하한과 상한을 지정하여 검색 범위를 좁히고 검색할 측정 단위를 지정할 수 있습니다.
   * **[!UICONTROL 승인(승인됨, 변경사항 요청, 거부됨, 보류 중) 및 만료와 같은 자산 상태에 따라 자산을 검색하는 상태]** .
   * **[!UICONTROL 자산의]** 등급을 기준으로 자산을 검색하는 평균 등급.
   * **[!UICONTROL 자산의 방향]** (가로, 세로, 정사각형)을 기준으로 자산을 검색하는 방향입니다.
   * **[!UICONTROL 자산의 스타일(컬러, 단색)을 기반으로 자산을 검색하려면 스타일을]** 지정합니다.
   * **[!UICONTROL 비디오 형식을]** 기반으로 비디오 에셋을 검색할 수 있는 비디오 형식(DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM).
   기본 검색 양식을 편집하여 필터 패널에서 [사용자 정의 검색 패싯을](../using/brand-portal-search-facets.md) 사용할 수 있습니다.

   * **[!UICONTROL 속성]** 설명(검색 양식에서 사용되는 경우)을 사용하면 조건자가 매핑되는 메타데이터 속성과 일치하는 자산을 검색할 수 있습니다.\
      예를 들어 속성 조건자가 에 매핑된 경우 [!UICONTROL `jcr:content /metadata/dc:title`]해당 제목을 기준으로 자산을 검색할 수 있습니다.\
      속성 [!UICONTROL 조건자는] 다음에 대한 텍스트 검색을 지원합니다.

      **부분 구문**
속성 조건부에서 부분 구문을 사용하여 자산 검색을 허용하도록 검색 양식에서 **[!UICONTROL 부분 검색]확인란을 활성화합니다.**\
      자산 메타데이터에 사용된 단어/구문을 정확히 지정하지 않더라도 원하는 자산을 검색할 수 있습니다.\
      다음 작업을 수행할 수 있습니다.* [필터] 패널의 패싯에서 검색된 구문에서 발생하는 단어를 지정합니다. For example, if you search for the term **climb** (and Property Predicate is mapped to [!UICONTROL `dc:title`] property), then all the assets with the word **climb** in their title phrase are returned.
* 검색한 구문에서 발생하는 단어의 일부와 와일드카드 문자(*)를 지정하여 간격을 채웁니다.
예를 들어 다음을 검색할 수 있습니다.
      **climb*** 제목 구문에 "hide"로 시작하는 단어가 있는 모든 자산을 반환합니다.
      ***climb** 는 제목 구문에 "climb"로 끝나는 단어가 포함된 모든 자산을 반환합니다.
      ***climb*** 제목 구문에 "climb"로 구성된 단어가 포함된 모든 자산을 반환합니다.\
      **대/소문자를 구분하지 않는 텍스트**&#x200B;속성 조건자에서 대/소문자를 구분하지 않는 검색을 허용하려면 검색 양식에서 **[!UICONTROL 대]** 소문자 무시 확인란을 활성화합니다. 기본적으로 속성 조건자에 대한 텍스트 검색은 대소문자를 구분합니다.
   >[!NOTE]
   >
   >부분 검색 **[!UICONTROL 확인란을 선택하면]** 기본적으로 [!UICONTROL 대소문자] 무시가 선택됩니다.

   ![](assets/wildcard-prop-1.png)

   검색 결과는 적용된 필터에 따라 검색 결과 수와 함께 표시됩니다.

   ![](assets/omnisearch-with-filters.png)

   Asset search result with search result count

3. You can easily navigate to an item from the search result, and return to the same search result using the back button in your browser without having to re-run the search query.

## Save your searches as smart collection {#save-your-searches-as-smart-collection}

You can save the search settings as a smart collection to be able to quickly repeat the same search without having to redo the same settings later.

To save the search settings as a smart collection:

1. Tap/ click Save Smart Collection and provide a name for the smart collection.****

   To make the smart collection accessible to all users, select Public. **** 스마트 컬렉션이 만들어져서 저장된 검색 목록에 추가되었음을 확인하는 메시지가 표시됩니다.

   >[!NOTE]
   >
   >관리자가 아닌 사용자는 조직의 브랜드 포털에서 관리자가 아닌 사용자가 만든 많은 수의 공개 스마트 컬렉션을 공유하지 못하도록 할 수 있습니다. 조직은 관리 도구 패널에서 **[!UICONTROL 사용 가능한 일반]** 설정에서 공개 스마트 컬렉션 생성 **** 허용 구성을 비활성화할 수 있습니다.

   ![](assets/save_smartcollectionui.png)

2. 스마트 컬렉션을 다른 이름으로 저장하고 공개 확인란을 선택하거나 **[!UICONTROL 지우려면 스마트]** 컬렉션 **[!UICONTROL 편집을 클릭합니다]**.

   ![](assets/edit_smartcollection.png)

3. 스마트 **[!UICONTROL 컬렉션 편집]** 대화 상자에서 다른 **[!UICONTROL 이름으로]** 저장을 선택하고 스마트 컬렉션의 이름을 입력합니다. **[!UICONTROL 저장을 클릭합니다]**.

   ![](assets/saveas_smartsearch.png)
