---
title: Brand Portal에서 자산 검색
seo-title: Asset searching and saved search on Experience Manager Assets Brand Portal
description: Brand Portal 검색 기능을 사용하면 omnisearch를 사용하여 관련 자산을 빠르게 검색할 수 있고, 검색 필터를 통해 검색 범위를 좁힐 수 있습니다. 나중에 검색을 스마트 컬렉션으로 저장합니다.
seo-description: Brand Portal search capability lets you quickly search for relevant assets using omnisearch, and search filters help you further narrow down your search. Save your searches as smart collections for future.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
exl-id: 7297bbe5-df8c-4d0b-8204-218a9fdc2292
source-git-commit: dc425522f134781b4420eb8643ee6ee65d98b6cc
workflow-type: tm+mt
source-wordcount: '1151'
ht-degree: 7%

---

# Brand Portal에서 자산 검색 {#search-assets-on-brand-portal}

Brand Portal 검색 기능을 사용하면 omnisearch 및 필터를 사용하는 패싯 검색을 사용하여 관련 자산을 빠르게 검색할 수 있으므로 검색 범위를 더 좁힐 수 있습니다. 파일 또는 폴더 수준에서 자산을 검색하고 검색 결과를 스마트 컬렉션으로 저장할 수 있습니다. 그러나 omnisearch 또는 패싯 검색을 사용하여 컬렉션의 자산을 검색할 수 없습니다.

## Omnisearch를 사용하여 자산 검색 {#search-assets-using-omnisearch}

Brand Portal에서 자산을 검색하려면 다음을 수행하십시오.

1. 도구 모음에서 **[!UICONTROL 검색]** 아이콘을 클릭하거나 &quot;**[!UICONTROL /]**&quot; 키를 눌러 Omnisearch를 실행합니다.

   ![](assets/omnisearchicon-1.png)

1. 검색 상자에서 검색할 자산에 대한 키워드를 입력합니다.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >검색 제안이 표시되려면 omnisearch에 3자 이상이 필요합니다.

1. 드롭다운 목록에 나타나는 관련 제안 중에서 선택하여 관련 자산에 빠르게 액세스합니다.

   ![](assets/assets-search-result.png)

   *omnisearch를 사용한 자산 검색*

스마트 태그가 지정된 자산의 검색 동작에 대해 알아보려면 [검색 결과 및 동작 이해](https://experienceleague.adobe.com/docs/experience-manager-65/assets/using/search-assets.html).

## 필터 패널에서 패싯을 사용하여 검색 {#search-using-facets-in-filters-panel}

필터 패널의 검색 패싯을 사용하면 검색 환경에 세부 사항을 추가하여 검색 기능을 효율적으로 수행할 수 있습니다. 검색 패싯에서는 복잡한 검색을 수행할 수 있는 여러 차원(설명)을 사용합니다. 보다 집중된 검색을 위해 원하는 세부 정보로 쉽게 드릴다운할 수 있습니다.

예를 들어, 이미지를 찾는 경우 비트맵과 벡터 이미지 중 어느 것을 선택할지 선택할 수 있습니다. 파일 유형 검색 패싯에서 이미지에 대한 MIME 유형을 지정하여 검색 범위를 더 줄일 수 있습니다. 마찬가지로 문서를 검색할 때 형식(예: PDF 또는 MS Word 형식)을 지정할 수 있습니다.

![Brand Portal의 필터 패널](assets/file-type-search.png "Brand Portal의 필터 패널")

다음 **[!UICONTROL 필터]** 패널에는 다음과 같은 몇 가지 표준 패싯이 포함되어 있습니다. **[!UICONTROL 경로 브라우저]**, **[!UICONTROL 파일 유형]**, **[!UICONTROL 파일 크기]**, **[!UICONTROL 상태]**, 및 **[!UICONTROL 방향]**. 그러나 다음을 수행할 수 있습니다 [사용자 정의 검색 패싯 추가](../using/brand-portal-search-facets.md) 또는 특정 검색 패싯을 **[!UICONTROL 필터]** 기본 검색 양식에서 조건자를 추가하거나 제거하여 패널. 사용 가능하고 사용 가능한 목록 을 참조하십시오 [Brand Portal에서 검색 설명](../using/brand-portal-search-facets.md#list-of-search-predicates).

검색에 필터를 적용하려면 사용 가능한 [검색 패싯](../using/brand-portal-search-facets.md):

1. 오버레이 아이콘을 클릭하고 을 선택합니다 **[!UICONTROL 필터]**.

   ![](assets/selectorrail.png)

1. 에서 **[!UICONTROL 필터]** 왼쪽의 패널에서 적절한 옵션을 선택하여 관련 필터를 적용합니다.
예를 들어, 다음 표준 필터를 사용하십시오.

   * **[!UICONTROL 경로 브라우저]** 을 눌러 특정 디렉토리에서 자산을 검색합니다. 경로 브라우저에 대한 조건부의 기본 검색 경로는 다음과 같습니다 `/content/dam/mac/<tenant-id>/`기본 검색 양식을 편집하여 구성할 수 있습니다.
   >[!NOTE]
   >
   >관리자가 아닌 사용자에게 [!UICONTROL 경로 브라우저] in [!UICONTROL 필터] 패널에는 공유된 폴더(및 상위 폴더)의 컨텐츠 구조만 표시됩니다.\
   >관리자 사용자에게 경로 브라우저를 사용하면 Brand Portal의 모든 폴더로 이동할 수 있습니다.

   * **[!UICONTROL 파일 유형]** 찾고 있는 자산 파일의 유형(이미지, 문서, 멀티미디어, 아카이브)을 지정하려면 또한 검색 범위를 좁힐 수 있습니다. 예를 들어 문서의 이미지 또는 형식(PDF 또는 MS Word)에 대한 MIME 유형(Tiff, Bitmap, GIMP 이미지)을 지정할 수 있습니다.
   * **[!UICONTROL 파일 크기]** 크기를 기준으로 자산을 검색합니다. 검색 범위를 좁힐 수 있도록 크기 범위의 하한과 상한을 지정하고 검색할 측정 단위를 지정할 수 있습니다.
   * **[!UICONTROL 상태]** 승인(승인됨, 변경요청됨, 거부됨, 보류 중) 및 만료와 같은 자산 상태를 기반으로 자산을 검색하려면
   * **[!UICONTROL 평균 등급]** 자산의 등급을 기준으로 자산을 검색합니다.
   * **[!UICONTROL 방향]** 자산의 방향(가로, 세로, 사각형)을 기반으로 자산을 검색하려면 다음을 수행하십시오.
   * **[!UICONTROL 스타일]** 자산의 스타일(컬러, 모노크롬)을 기반으로 자산을 검색하려면 다음을 수행하십시오.
   * **[!UICONTROL 비디오 형식]** 해당 형식을 기반으로 비디오 자산을 검색하려면(DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM).

   다음을 사용할 수 있습니다 [사용자 지정 검색 패싯](../using/brand-portal-search-facets.md) 기본 검색 양식을 편집하여 [필터] 패널에서

   * **[!UICONTROL 속성 설명]** 검색 양식에서 사용하는 경우 조건부가 매핑되는 메타데이터 속성과 일치하는 자산을 검색할 수 있습니다.\
      예를 들어 속성 조건부가 [!UICONTROL `jcr:content /metadata/dc:title`], 해당 제목을 기준으로 자산을 검색할 수 있습니다.\
      다음 [!UICONTROL 속성 설명] 에서는 텍스트 검색을 지원합니다.

      **부분 구문**
속성 조건부에서 부분 구문을 사용하여 자산 검색을 허용하도록 검색 양식에서 **[!UICONTROL 부분 검색]** 확인란을 활성화합니다.\
      자산 메타데이터에 사용된 단어/구문을 정확히 지정하지 않더라도 원하는 자산을 검색할 수 있습니다.\
      다음을 작업을 수행할 수 있습니다.
      * 필터 패널에서 패싯의 검색한 구문에서 발생하는 단어를 지정합니다. 예를 들어 **등벽** (그리고 속성 조건부가 [!UICONTROL `dc:title`] property) 를 반환하고, **등벽** 제목 구문에서 해당 구문이 반환됩니다.
      * 검색한 구문에서 발생하는 단어의 일부와 와일드카드 문자(*)를 지정하여 간격을 채웁니다.
예를 들어 다음을 검색할 수 있습니다.
         * **등산하기** 제목 구문에 &quot;climb&quot; 문자로 시작하는 단어가 있는 모든 자산을 반환합니다.
         * ***등반** 제목 구문에 &quot;climb&quot;으로 끝나는 단어가 포함된 모든 자산을 반환합니다.
         * ***등반*** 제목 구문에 &quot;climb&quot; 문자가 포함된 단어가 있는 모든 자산을 반환합니다.

속성 조건부에서 대소문자를 구분하지 않는 검색을 허용하려면       **대/소문자를 구분하지 않는 텍스트**
속성 조건부에서 대소문자를 구분하지 않는 검색을 허용하려면 **[!UICONTROL 대/소문자 무시]** 검색 양식의 확인란. 기본적으로 속성 조건부의 텍스트 검색은 대소문자를 구분합니다.
   >[!NOTE]
   >
   >선택 시 **[!UICONTROL 부분 검색]** 확인란, **[!UICONTROL 대/소문자 무시]** 기본적으로 선택되어 있습니다.

   ![](assets/wildcard-prop-1.png)

   검색 결과는 검색 결과 수와 함께 적용된 필터에 따라 표시됩니다.

   ![](assets/omnisearch-with-filters.png)

   검색 결과 카운트가 있는 자산 검색 결과.

1. 검색 결과에서 항목을 쉽게 탐색하고 검색 쿼리를 다시 실행하지 않고 브라우저의 뒤로 단추를 사용하여 동일한 검색 결과로 돌아갈 수 있습니다.

## 검색을 스마트 컬렉션으로 저장 {#save-your-searches-as-smart-collection}

검색 설정을 스마트 컬렉션으로 저장하여 나중에 동일한 설정을 다시 실행하지 않고도 동일한 검색을 빠르게 반복할 수 있습니다. 그러나 컬렉션에는 검색 필터를 적용할 수 없습니다.

검색 설정을 스마트 컬렉션으로 저장하려면 다음을 수행합니다.

1. 탭/클릭 **[!UICONTROL 스마트 컬렉션 저장]** 및 은(는) 스마트 컬렉션의 이름을 제공합니다.

   모든 사용자가 스마트 컬렉션에 액세스할 수 있도록 하려면 **[!UICONTROL 공용]**. 스마트 컬렉션이 생성되어 저장된 검색 목록에 추가되었음을 확인하는 메시지가 표시됩니다.

   >[!NOTE]
   >
   >관리자가 아닌 사용자는 조직의 Brand Portal에서 관리자가 아닌 사용자가 만든 많은 수의 공개 스마트 컬렉션을 방지하기 위해 스마트 컬렉션을 공개하도록 제한할 수 있습니다. 조직에서 **[!UICONTROL 공용 스마트 컬렉션 만들기 허용]** 구성 **[!UICONTROL 일반]** 관리 도구 패널에서 사용할 수 있는 설정입니다.

   ![](assets/save_smartcollectionui.png)

1. 스마트 컬렉션을 다른 이름으로 저장하려면 **[!UICONTROL 공용]** 확인란 **[!UICONTROL 스마트 컬렉션 편집]**.

   ![](assets/edit_smartcollection.png)

1. 설정 **[!UICONTROL 스마트 컬렉션 편집]** 대화 상자, 선택 **[!UICONTROL 다른 이름으로 저장]** 스마트 컬렉션 이름을 입력합니다. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   ![](assets/saveas_smartsearch.png)
