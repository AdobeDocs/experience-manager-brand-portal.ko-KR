---
title: Brand Portal에서 자산 검색
seo-title: Asset searching and saved search on Experience Manager Assets Brand Portal
description: Brand Portal 검색 기능을 사용하면 omnisearch를 사용하여 관련 에셋을 빠르게 검색할 수 있으며, 검색 필터를 사용하면 검색 범위를 더욱 좁힐 수 있습니다. 나중에 스마트 컬렉션으로 검색을 저장합니다.
seo-description: Brand Portal search capability lets you quickly search for relevant assets using omnisearch, and search filters help you further narrow down your search. Save your searches as smart collections for future.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
exl-id: 7297bbe5-df8c-4d0b-8204-218a9fdc2292
source-git-commit: cbdd943b904882cc9a455bab24c3cf732d5966ca
workflow-type: tm+mt
source-wordcount: '1358'
ht-degree: 5%

---

# Brand Portal에서 자산 검색 {#search-assets-on-brand-portal}

Brand Portal 검색 기능을 사용하면 omnisearch 및 필터를 사용하여 검색 범위를 좁히는 데 도움이 되는 facet 검색을 사용하여 관련 에셋을 빠르게 검색할 수 있습니다. 파일 또는 폴더 수준에서 자산을 검색하고 검색 결과를 스마트 컬렉션으로 저장할 수 있습니다.

>[!NOTE]
>
>Brand Portal은 omnisearch를 사용한 컬렉션 검색을 지원하지 않습니다.
>
>그러나 다음을 사용할 수 있습니다. [검색 필터를 사용하여 관련 컬렉션 목록 가져오기](#search-collection).

## Omnisearch를 사용하여 에셋 검색 {#search-assets-using-omnisearch}

Brand Portal에서 자산을 검색하려면 다음을 수행하십시오.

1. 도구 모음에서 **[!UICONTROL 검색]** 아이콘을 클릭하거나 &quot;**[!UICONTROL /]**&quot; Omnisearch 시작 키.

   ![](assets/omnisearchicon-1.png)

1. 검색 상자에 검색할 에셋의 키워드를 입력합니다.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >* 검색 제안을 표시하려면 omnisearch에 최소 3자가 필요합니다.
   >* 다음을 검색할 때 `mountain biking`, omnisearch는 검색 결과에 두 항목이 모두 있는 모든 자산을 반환합니다. `mountain` 및 `biking` 메타데이터 필드에서 사용할 수 있습니다. 예를 들어, `mountain` 다음에서 `Title` 필드 및 `biking` 다음에서 `Description` 필드. 두 용어 모두 메타데이터 필드에서 사용할 수 있어야 검색 결과에 표시할 수 있습니다. 그러나 Omnisearch는 스마트 태그 메타데이터 필드에서 두 용어 중 하나만 사용할 수 있는 경우에도 검색 결과에 에셋을 반환합니다. 예를 들어 에셋에 `mountain` 는 스마트 태그 중 하나이며 를 포함하지 않습니다 `biking` 다른 메타데이터 필드에서 을 검색하고 `mountain biking`, omnisearch는 여전히 검색 결과에 에셋을 반환합니다.


1. 관련 에셋에 빠르게 액세스하려면 드롭다운 목록에 표시되는 관련 제안 중에서 선택합니다.

   ![](assets/assets-search-result.png)

   *omnisearch를 사용한 자산 검색*

스마트 태그가 지정된 에셋의 검색 동작에 대해 알아보려면 를 참조하십시오. [검색 결과 및 동작 이해](https://experienceleague.adobe.com/docs/experience-manager-65/assets/using/search-assets.html).

## 필터 패널에서 패싯을 사용하여 검색 {#search-using-facets-in-filters-panel}

필터 패널의 검색 패싯은 검색 경험에 세부 기간을 추가하고 검색 기능을 효율화합니다. 검색 패싯은 복잡한 검색을 수행할 수 있도록 해주는 여러 차원(술어)을 사용합니다. 원하는 세부 수준으로 쉽게 드릴다운하여 보다 집중적인 검색을 수행할 수 있습니다.

예를 들어 이미지를 찾는 경우 비트맵 이미지를 원하는지 벡터 이미지를 원하는지 선택할 수 있습니다. 파일 유형 검색 패싯에서 이미지에 대한 MIME 유형을 지정하여 검색 범위를 추가로 줄일 수 있습니다. 마찬가지로 문서를 검색할 때 PDF 또는 MS® Word 형식과 같은 형식을 지정할 수 있습니다.

![Brand Portal의 필터 패널](assets/file-type-search.png "Brand Portal의 필터 패널")

다음 **[!UICONTROL 필터]** 패널에는 다음과 같은 몇 가지 표준 패싯이 포함됩니다. **[!UICONTROL 경로 브라우저]**, **[!UICONTROL 파일 유형]**, **[!UICONTROL 파일 크기]**, **[!UICONTROL 상태]**, 및 **[!UICONTROL 방향]**. 그러나 다음을 수행할 수 있습니다. [사용자 정의 검색 패싯 추가](../using/brand-portal-search-facets.md) 또는 에서 특정 검색 패싯을 제거합니다. **[!UICONTROL 필터]** 패널: 기본 검색 양식에서 술어를 추가하거나 제거합니다. 사용 가능한 및 사용 가능한 목록 보기 [Brand Portal에서 술어 검색](../using/brand-portal-search-facets.md#list-of-search-predicates).

필터를 검색에 적용하려면 사용 가능한 [검색 패싯](../using/brand-portal-search-facets.md):

1. 오버레이 아이콘을 클릭하고 다음을 선택합니다. **[!UICONTROL 필터]**.

   ![](assets/selectorrail.png)

1. 다음에서 **[!UICONTROL 필터]** 왼쪽의 패널에서 적절한 옵션을 선택하여 관련 필터를 적용합니다.
예를 들어 다음 표준 필터를 사용합니다.

   * **[!UICONTROL 경로 브라우저]** 특정 디렉토리에서 에셋을 검색할 수 있습니다. 경로 브라우저에 대한 술어의 기본 검색 경로는 다음과 같습니다. `/content/dam/mac/<tenant-id>/`기본 검색 양식을 편집하여 구성할 수 있습니다.
   >[!NOTE]
   >
   >관리자가 아닌 사용자에게, [!UICONTROL 경로 브라우저] 위치: [!UICONTROL 필터] 패널에는 공유된 폴더(및 상위 폴더)의 콘텐츠 구조만 표시됩니다.\
   >관리 사용자를 위해 경로 브라우저를 사용하여 Brand Portal의 모든 폴더로 이동할 수 있습니다.

   * **[!UICONTROL 파일 유형]** 원하는 자산 파일의 유형(이미지, 문서, 멀티미디어, 아카이브)을 지정합니다. 또한 검색 범위를 좁힐 수 있습니다. 예를 들어 이미지에 대한 MIME 유형(Tiff, 비트맵, GIMP 이미지)이나 문서에 대한 형식(PDF 또는 MS® Word)을 지정할 수 있습니다.
   * **[!UICONTROL 파일 크기]** 를 클릭하여 크기를 기반으로 에셋을 검색할 수 있습니다. 크기 범위의 하한과 상한을 지정하여 검색 범위를 좁히고 검색할 측정 단위를 지정할 수 있습니다.
   * **[!UICONTROL 상태]** 승인(승인됨, 변경 요청, 거부됨, 보류 중) 및 만료와 같은 에셋 상태를 기준으로 에셋을 검색할 수 있습니다.
   * **[!UICONTROL 평균 등급]** 를 클릭하여 자산의 등급을 기반으로 자산을 검색합니다.
   * **[!UICONTROL 방향]** 에셋의 방향(가로, 세로, 사각형)을 기준으로 에셋을 검색할 수 있습니다.
   * **[!UICONTROL 스타일]** 에셋의 스타일(컬러, 모노크롬)을 기반으로 에셋을 검색할 수 있습니다.
   * **[!UICONTROL 비디오 형식]** 포맷을 기반으로 비디오 자산을 검색합니다(DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM).

   다음을 사용할 수 있습니다. [사용자 정의 검색 패싯](../using/brand-portal-search-facets.md) 필터 패널에서 기본 검색 양식을 편집하여

   * **[!UICONTROL 속성 조건자]** 검색 양식에서 를 사용하는 경우 조건자가 매핑된 메타데이터 속성과 일치하는 에셋을 검색할 수 있습니다.\
      예를 들어 속성 조건자가에 매핑되는 경우 [!UICONTROL `jcr:content /metadata/dc:title`], 제목을 기반으로 에셋을 검색할 수 있습니다.\
      다음 [!UICONTROL 속성 조건자] 은 다음에 대한 텍스트 검색을 지원합니다.

      **부분 구문**
속성 조건부에서 부분 구문을 사용하여 자산 검색을 허용하도록 검색 양식에서 **[!UICONTROL 부분 검색]** 확인란을 활성화합니다. 자산 메타데이터에 사용된 단어/구문을 정확히 지정하지 않더라도 원하는 자산을 검색할 수 있습니다.

      >[!NOTE]
      >
      > Brand Portal은 부분 검색에 대해 다음 필드를 지원합니다.
      >* jcr:content/metadata/dc:title
      >* jcr:content/jcr:title
      >* jcr:content/metadata/dam:search_promote
      >* jcr:content/metadata/dc:format


      다음과 같은 작업을 수행할 수 있습니다.
      * 필터 패널에서 패싯의 검색한 구문에서 발생하는 단어를 지정합니다. 예를 들어 검색어를 **상승** (속성 조건자가에 매핑됨) [!UICONTROL `dc:title`] 속성), 단어 포함 모든 에셋 **상승** 제목 구문이 반환됩니다.
      * 검색한 구문에서 발생하는 단어의 일부를 와일드카드 문자()와 함께 지정합니다.&#42;)을 클릭하여 간격을 채웁니다.
예를 들어 다음을 검색할 수 있습니다.
         * **상승&#42;** 제목 구문에 &quot;climb&quot; 문자로 시작하는 단어가 포함된 모든 자산을 반환합니다.
         * **&#42;상승** 제목 구문에 &quot;climb&quot; 문자로 끝나는 단어가 있는 모든 자산을 반환합니다.
         * **&#42;상승&#42;** 제목 구문에 &quot;climb&quot; 문자가 포함된 단어가 포함된 모든 자산을 반환합니다.

속성 조건자에서 대/소문자를 구분하지 않는 검색을 허용하려면       **대/소문자를 구분하지 않는 텍스트**
속성 조건자에서 대/소문자를 구분하지 않는 검색을 허용하려면 **[!UICONTROL 대소문자 무시]** 검색 양식에 있는 확인란입니다. 기본적으로 속성 조건자의 텍스트 검색은 대/소문자를 구분합니다.
   >[!NOTE]
   >
   >선택 시 **[!UICONTROL 부분 검색]** 확인란, **[!UICONTROL 대소문자 무시]** 기본적으로 가 선택되어 있습니다.

   ![](assets/wildcard-prop-1.png)

   검색 결과는 검색 결과 카운트와 함께 적용된 필터에 따라 표시됩니다.

   ![](assets/omnisearch-with-filters.png)

   검색 결과 카운트가 포함된 에셋 검색 결과.

1. 검색 쿼리를 다시 실행하지 않고도 검색 결과에서 항목을 쉽게 탐색하고 브라우저의 뒤로 단추를 사용하여 동일한 검색 결과로 돌아갈 수 있습니다.

## 검색을 스마트 컬렉션으로 저장 {#save-your-searches-as-smart-collection}

나중에 동일한 설정을 다시 실행하지 않고도 동일한 검색을 빠르게 반복할 수 있도록 검색 설정을 스마트 컬렉션으로 저장할 수 있습니다. 하지만 컬렉션에서는 검색 필터를 적용할 수 없습니다.

검색 설정을 스마트 컬렉션으로 저장하려면 다음을 수행합니다.

1. 탭/클릭 **[!UICONTROL 스마트 컬렉션 저장]** 스마트 컬렉션의 이름을 입력합니다.

   모든 사용자가 스마트 컬렉션을 액세스할 수 있도록 하려면 다음을 선택합니다. **[!UICONTROL 공용]**. 스마트 컬렉션이 생성되어 저장된 검색 목록에 추가되었음을 확인하는 메시지가 표시됩니다.

   >[!NOTE]
   >
   >조직의 Brand Portal에 관리자가 아닌 사용자가 만든 공용 스마트 컬렉션이 너무 많아 관리자가 아닌 사용자가 스마트 컬렉션을 공개하지 못하도록 제한할 수 있습니다. 조직에서 다음을 비활성화할 수 있습니다. **[!UICONTROL 공용 스마트 컬렉션 만들기 허용]** 다음에서 구성 **[!UICONTROL 일반]** 관리 도구 패널에서 사용할 수 있는 설정.

   ![](assets/save_smartcollectionui.png)

1. 스마트 컬렉션을 다른 이름으로 저장하려면 을 선택하거나 선택 취소합니다. **[!UICONTROL 공용]** 확인란, 클릭 **[!UICONTROL 스마트 컬렉션 편집]**.

   ![](assets/edit_smartcollection.png)

1. 다음에서 **[!UICONTROL 스마트 컬렉션 편집]** 대화 상자에서 **[!UICONTROL 다른 이름으로 저장]** 스마트 컬렉션의 이름을 입력합니다. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   ![](assets/saveas_smartsearch.png)


## 컬렉션 검색 {#search-collection}

컬렉션에 대해서는 Omnisearch가 지원되지 않습니다. 하지만 검색 필터를 적용하여 내에서 관련 컬렉션을 나열할 수 있습니다. [!UICONTROL 컬렉션] 인터페이스.

다음에서 [!UICONTROL 컬렉션] 인터페이스에서 오버레이 아이콘을 클릭하여 왼쪽 레일에서 필터 패널을 엽니다. 사용 가능한 필터에서 단일 또는 다중 검색 필터 적용(`modified date`, `access type`, 및 `tags`). 적용된 필터를 기반으로 가장 관련성이 높은 컬렉션 세트를 나열합니다.

![](assets/collection-search.png)
