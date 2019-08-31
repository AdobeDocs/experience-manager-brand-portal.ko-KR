---
title: 브랜드 포털에서 에셋 검색
seo-title: AEM 브랜드 포털에서 자산 검색 및 저장된 검색
description: 브랜드 포털 검색 기능을 사용하면 Omnisearch를 사용하여 관련 자산을 신속하게 검색하고 검색 필터를 사용하여 검색 범위를 좁힐 수 있습니다. 검색을 향후 고급 컬렉션으로 저장할 수 있습니다.
seo-description: 브랜드 포털 검색 기능을 사용하면 Omnisearch를 사용하여 관련 자산을 신속하게 검색하고 검색 필터를 사용하여 검색 범위를 좁힐 수 있습니다. 검색을 향후 고급 컬렉션으로 저장할 수 있습니다.
uuid: C 2955198-BDC 0-4853-A 13 A -661 E 6 A 9 EC 61 F
contentOwner: BDHAR
content-type: 참조
products: sg_ Experiencemanager/brand_ portal
topic-tags: searchandpromote
discoiquuid: dc 751 cd 7-f 663-46 d 2-84 c 4-5 bb 12 a 4 fe 1 ba
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 브랜드 포털에서 에셋 검색 {#search-assets-on-brand-portal}

브랜드 포털 검색 기능을 사용하면 Omnisearch를 사용하여 관련 자산을 신속하게 검색하고 필터를 사용하여 검색 범위를 좁히는 데 도움이 되는 검색을 할 수 있습니다. 또한 검색을 향후 고급 컬렉션으로 저장할 수도 있습니다.

## Omnisearch를 사용하여 에셋 검색 {#search-assets-using-omnisearch}

브랜드 포털에서 자산을 검색하려면 다음을 수행하십시오.

1. 도구 모음에서 **[!UICONTROL 검색]** 아이콘을 클릭하거나 "**[!UICONTROL /]**" 키를 눌러 Omnisearch를 실행합니다.

   ![](assets/omnisearchicon-1.png)

2. 검색 상자에 검색할 자산의 키워드를 입력합니다.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >Omnisearch에서 검색 제안이 표시되는 데 3 자 이상이 필요합니다.

3. 드롭다운 목록에 나타나는 관련 제안 중에서 선택하여 관련 자산에 빠르게 액세스할 수 있습니다.

   ![](assets/assets-search-result.png)

   *Omnisearch를 사용한 자산 검색*

## 필터 패널에서 패싯을 사용하여 검색 {#search-using-facets-in-filters-panel}

필터 패널에서 검색 패싯은 검색 경험에 세부기간을 추가하고 검색 기능을 효율적으로 만듭니다. 검색 패싯은 복잡한 검색을 수행할 수 있는 여러 차원 (예측) 를 사용합니다. 원하는 세부 수준으로 쉽게 드릴다운하여 보다 집중적인 검색을 수행할 수 있습니다.

예를 들어 이미지를 찾고 있는 경우 비트맵 또는 벡터 이미지를 표시할지 여부를 선택할 수 있습니다. 파일 유형 검색 패싯에서 이미지에 대한 MIME 유형을 지정하여 검색 범위를 더 줄일 수 있습니다. 마찬가지로 문서를 검색할 때 PDF 또는 MS Word 형식을 지정할 수 있습니다.

![브랜드 포털의 필터](assets/file-type-search.png "패널 브랜드 포털의 필터 패널")

[!UICONTROL 필터] 패널에는 [!UICONTROL 경로 브라우저], [!UICONTROL 파일 유형], [!UICONTROL 파일 크기], [!UICONTROL 상태]및 [!UICONTROL 방향과 같은 몇 가지 표준 패싯이 포함되어]있습니다. [하지만](../using/brand-portal-search-facets.md) 기본 검색 양식에서 예측을 추가하거나 제거하여 [!UICONTROL 필터] 패널에서 사용자 지정 검색 패싯을 추가하거나 특정 검색 패싯을 제거할 수 있습니다. 브랜드 포털에서 사용 가능하고 사용 가능한 [검색 키워드 목록을 참조하십시오](../using/brand-portal-search-facets.md#list-of-search-predicates).

사용 가능한 [검색 패싯을 사용하여 검색에 필터를 적용하려면](../using/brand-portal-search-facets.md)다음을 수행하십시오.

1. 오버레이 아이콘을 클릭하고 **[!UICONTROL 필터를 선택합니다]**.

   ![](assets/selectorrail.png)

2. 왼쪽의 **[!UICONTROL 필터]** 패널에서 관련 필터를 적용할 적절한 옵션을 선택합니다.
예를 들어 다음과 같은 표준 필터를 사용합니다.

   * **[!UICONTROL 경로 브라우저를]** 사용하여 특정 디렉토리에서 자산을 검색합니다. 경로 브라우저에 대한 안내서의 기본 검색 경로는 **[!UICONTROL /content/dam/mac/ &lt; 임차인 ID &gt;/이며]**&#x200B;기본 검색 양식을 편집하여 구성할 수 있습니다.
   >[!NOTE]
   >
   >관리자가 아닌 [!UICONTROL 사용자에게는] [!UICONTROL 필터] 패널의 경로 브라우저에 공유된 폴더 (및 해당 상위 폴더) 의 콘텐트 구조만 표시됩니다.\
   >관리 사용자에게 경로 브라우저를 사용하면 브랜드 포털에서 모든 폴더로 이동할 수 있습니다.

   * **[!UICONTROL 파일 유형을]** 참조하십시오. 또한 검색의 범위를 좁힐 수 있습니다. 예를 들어, 문서의 이미지 또는 형식 (PDF 또는 MS Word) 에 MIME 유형 (TIFF, 비트맵, GIMP 이미지) 를 지정할 수 있습니다.
   * **[!UICONTROL 파일 크기를]** 참조하십시오. 범위 범위에 대한 하한 및 상한을 지정하여 검색 범위를 좁히고 검색할 측정 단위를 지정할 수 있습니다.
   * **[!UICONTROL 승인 (]** 승인, 요청된 변경 사항, 거부됨, 보류 중) 및 만료와 같은 자산 상태에 따라 자산을 검색합니다.
   * **[!UICONTROL 자산의]** 등급을 기준으로 자산을 검색할 평균 등급.
   * **[!UICONTROL 자산의]** 방향 (수평, 수직, 정사각형) 를 기준으로 자산을 검색하는 방향입니다.
   * **[!UICONTROL 스타일을]** 사용하여 자산의 스타일 (컬러, 단색) 를 기반으로 자산을 검색합니다.
   * **[!UICONTROL 비디오 형식을]** 사용하여 형식 (DVI, Flash, MPEG 4, MPEG, OGG Theora, QuickTime, Windows Media, Webm) 를 기반으로 비디오 에셋을 검색할 수 있습니다.
   기본 검색 양식을 편집하여 필터 패널에서 [사용자 지정 검색 패싯을](../using/brand-portal-search-facets.md) 사용할 수 있습니다.

   * **[!UICONTROL 속성 설명]** 검색 양식에서 사용하는 경우, 설명이 매핑되는 메타데이터 속성과 일치하는 자산을 검색할 수 있습니다.\
      예를 들어 속성 설명이 매핑되는 경우 해당 제목을 [!UICONTROL `jcr:content /metadata/dc:title`]기준으로 자산을 검색할 수 있습니다.\
      [!UICONTROL 속성 설명에서는] 다음에 대한 텍스트 검색을 지원합니다.

      **부분 구문**
속성 조건부에서 부분 구문을 사용하여 자산 검색을 허용하도록 검색 양식에서 **[!UICONTROL 부분 검색]확인란을 활성화합니다.**\
      자산 메타데이터에 사용된 단어/구문을 정확히 지정하지 않더라도 원하는 자산을 검색할 수 있습니다.\
      다음을 수행할 수 있습니다.
* 필터 패널에서 패싯의 검색어에 나타나는 단어를 지정합니다. For example, if you search for the term **climb** (and Property Predicate is mapped to [!UICONTROL `dc:title`] property), then all the assets with the word **climb** in their title phrase are returned.
* 검색한 구문에서 발생하는 단어의 일부와 와일드카드 문자(*)를 지정하여 간격을 채웁니다.
예를 들어 다음을 검색할 수 있습니다.
      **CLIMB *** 는 제목 구문에서 문자가 "CLIMB" 로 시작하는 모든 자산을 반환합니다.
      *** climb는** 제목 구문에서 문자가 "climb" 문자로 끝나는 모든 자산을 반환합니다.
      *** CLIMB *** 는 제목 구문에서 문자가 "CLIMB" 인 모든 자산을 포함하는 모든 자산을 반환합니다.\
      **대소문자를 구분하지 않는 텍스트를**
속성 사기에서 대소문자를 구분하지 않는 검색을 허용하려면 검색 양식에서 대/소문자 **[!UICONTROL 무시]** 확인란을 활성화합니다. 기본적으로 속성 언어에서 텍스트 검색은 대/소문자를 구분합니다.
   >[!NOTE]
   >
   >**[!UICONTROL 부분 검색]** 확인란을 선택할 때 대/소문자를 [!UICONTROL 무시하면 기본적으로 선택됩니다] .

   ![](assets/wildcard-prop-1.png)

   검색 결과는 검색 결과 수와 함께 적용된 필터에 따라 표시됩니다.

   ![](assets/omnisearch-with-filters.png)

   검색 결과 카운트가 있는 자산 검색 결과

3. 검색 결과에서 항목으로 쉽게 이동할 수 있으며 검색 쿼리를 다시 실행하지 않고도 브라우저의 [뒤로] 단추를 사용하여 동일한 검색 결과로 돌아갈 수 있습니다.

## 검색을 스마트 컬렉션으로 저장 {#save-your-searches-as-smart-collection}

검색 설정을 스마트 컬렉션으로 저장하여 나중에 동일한 설정을 다시 실행하지 않고도 동일한 검색을 신속하게 반복할 수 있습니다.

검색 설정을 스마트 컬렉션으로 저장하려면 다음을 수행하십시오.

1. 스마트 컬렉션 **[!UICONTROL 저장을 탭/클릭하고]** 스마트 컬렉션의 이름을 입력합니다.

   스마트 컬렉션을 모든 사용자가 액세스할 수 있게 하려면 **[!UICONTROL [공개]**] 를 선택합니다. 스마트 컬렉션이 생성되어 저장된 검색 목록에 추가되었음을 확인하는 메시지가 나타납니다.

   >[!NOTE]
   >
   >관리자가 아닌 사용자는 조직의 브랜드 포털에서 관리자가 아닌 사용자가 만든 대량의 공개 스마트 컬렉션이 없도록 스마트 컬렉션을 공개하지 않도록 제한할 수 있습니다. 조직은 [관리 도구] 패널에서 **[!UICONTROL 사용할 수 있는]** **[!UICONTROL 일반]** 설정에서 공개 스마트 컬렉션 작성 구성을 비활성화할 수 있습니다.

   ![](assets/save_smartcollectionui.png)

2. 스마트 컬렉션을 다른 이름으로 저장하고 **[!UICONTROL 공개]** 확인란을 선택 또는 지우려면 [스마트 컬렉션 **[!UICONTROL 편집] 를 클릭합니다]**.

   ![](assets/edit_smartcollection.png)

3. 스마트 컬렉션 **[!UICONTROL 편집]** 대화 상자에서 **[!UICONTROL 다른 이름으로]** 저장을 선택하고 스마트 컬렉션의 이름을 입력합니다. **[!UICONTROL 저장을 클릭합니다]**.

   ![](assets/saveas_smartsearch.png)