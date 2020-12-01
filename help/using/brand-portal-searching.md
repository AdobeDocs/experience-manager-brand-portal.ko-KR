---
title: Brand Portal에서 자산 검색
seo-title: AEM 브랜드 포털에서 자산 검색 및 검색 저장
description: 브랜드 포털 검색 기능을 사용하면 옴니서치를 사용하여 관련 자산을 신속하게 검색할 수 있고 검색 필터를 통해 검색 범위를 좁힐 수 있습니다. 나중에 스마트 컬렉션으로 검색을 저장할 수 있습니다.
seo-description: 브랜드 포털 검색 기능을 사용하면 옴니서치를 사용하여 관련 자산을 신속하게 검색할 수 있고 검색 필터를 통해 검색 범위를 좁힐 수 있습니다. 나중에 스마트 컬렉션으로 검색을 저장할 수 있습니다.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873
workflow-type: tm+mt
source-wordcount: '1163'
ht-degree: 7%

---


# Brand Portal에서 자산 검색 {#search-assets-on-brand-portal}

브랜드 포털 검색 기능을 사용하면 옴니쉬 및 필터를 사용하여 검색 범위를 좁히는 패싯 검색을 통해 관련 자산을 빠르게 검색할 수 있습니다. 나중에 스마트 컬렉션으로 검색을 저장할 수도 있습니다.

## Omnisearch {#search-assets-using-omnisearch}을 사용하여 자산 검색

브랜드 포털에서 자산을 검색하려면

1. 도구 모음에서 **[!UICONTROL 검색]** 아이콘을 클릭하거나 &quot;**[!UICONTROL /]**&quot; 키를 눌러 Omnisearch를 시작합니다.

   ![](assets/omnisearchicon-1.png)

1. 검색 상자에 검색할 자산에 대한 키워드를 입력합니다.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >검색 제안이 표시되려면 3자 이상이 필요합니다.

1. 관련 자산에 빠르게 액세스하려면 드롭다운 목록에 표시되는 관련 제안 중에서 선택하십시오.

   ![](assets/assets-search-result.png)

   *omnisearch를 사용한 자산 검색*

스마트 태그 자산의 검색 동작에 대해 알아보려면 [검색 결과 및 동작 이해](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-assets.html)를 참조하십시오.

## 필터 패널 {#search-using-facets-in-filters-panel}의 패싯을 사용하여 검색

필터 패널에서 검색 패싯을 사용하면 검색 경험에 세부기간을 추가하고 검색 기능을 효율적으로 사용할 수 있습니다. 검색 패싯은 복잡한 검색을 수행할 수 있도록 해주는 여러 차원(예측)을 사용합니다. 원하는 세부 수준으로 드릴다운하여 보다 집중적인 검색을 수행할 수 있습니다.

예를 들어, 이미지를 찾고 있는 경우 비트맵과 벡터 이미지 중 어떤 것을 원하는지 선택할 수 있습니다. 파일 유형 검색 패싯에서 이미지의 MIME 유형을 지정하여 검색 범위를 더 줄일 수 있습니다. 마찬가지로 문서를 검색할 때 형식(예: PDF 또는 MS Word 형식)을 지정할 수 있습니다.<br />

![브랜드 포털의 브랜드 ](assets/file-type-search.png "포털 필터 패널의 필터 패널")

**[!UICONTROL 필터]** 패널에는 - **[!UICONTROL 경로 브라우저]**, **[!UICONTROL 파일 유형]**, **[!UICONTROL 파일 크기]**, **[!UICONTROL 상태]** 및 **[!UICONTROL 방향]**&#x200B;과 같은 몇 가지 표준 패싯이 포함되어 있습니다.>. 그러나 기본 검색 양식에서 예측자를 추가하거나 제거하여 [사용자 지정 검색 패싯](../using/brand-portal-search-facets.md)을 추가하거나 **[!UICONTROL 필터]** 패널에서 특정 검색 패싯을 제거할 수 있습니다. 브랜드 포털[에서 사용 가능한 검색 조건들의 목록을 참조하십시오.](../using/brand-portal-search-facets.md#list-of-search-predicates)

검색에 필터를 적용하려면 사용 가능한 [검색 패싯](../using/brand-portal-search-facets.md)을 사용합니다.

1. 오버레이 아이콘을 클릭하고 **[!UICONTROL 필터]**&#x200B;를 선택합니다.

   ![](assets/selectorrail.png)

1. 왼쪽의 **[!UICONTROL 필터]** 패널에서 적절한 옵션을 선택하여 관련 필터를 적용합니다.
예를 들어 다음 표준 필터를 사용하십시오.

   * **[!UICONTROL 경로]** 탐색특정 디렉토리에서 자산을 검색합니다. 경로 브라우저에 대한 조건자의 기본 검색 경로는 `/content/dam/mac/<tenant-id>/`이며 기본 검색 양식을 편집하여 구성할 수 있습니다.
   >[!NOTE]
   >
   >관리자가 아닌 사용자에게, [!UICONTROL 필터] 패널의 [!UICONTROL 경로 브라우저]는 자신과 공유되는 폴더(및 상위 폴더)의 컨텐츠 구조만 표시합니다.\
   >관리 사용자를 위해 경로 브라우저는 브랜드 포털의 모든 폴더로 이동할 수 있도록 허용합니다.

   * **[!UICONTROL 파일]** 유형을 사용하여 원하는 에셋 파일의 유형(이미지, 문서, 멀티미디어, 아카이브)을 지정합니다. 또한 문서의 이미지 또는 형식(PDF 또는 MS Word)에 대한 MIME 유형(Tiff, Bitmap, GIMP Images)을 지정하여 검색 범위를 좁힐 수 있습니다.
   * **[!UICONTROL 파일]** 크기에셋을 크기에 따라 검색합니다. 크기 범위의 하한과 상한을 지정하여 검색 범위를 좁히고 검색할 측정 단위를 지정할 수 있습니다.
   * **[!UICONTROL 승인(승인됨, 변경요청, 거부됨, 보류 중) 및 만료와 같은 자산 상태에 따라 자산 검색을]** 시작합니다.
   * **[!UICONTROL 자산]** 등급을 기준으로 자산을 검색하는 평균 등급.
   * **[!UICONTROL 방향]** 은 자산의 방향(가로, 세로, 정사각형)을 기준으로 자산을 검색합니다.
   * **[!UICONTROL 스타일]** 을 사용하여 자산의 스타일(컬러, 모노크롬)을 기반으로 자산을 검색합니다.
   * **[!UICONTROL 비디오]** 형식을 기반으로 비디오 에셋을 검색하는 비디오 형식(DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM)

   기본 검색 양식을 편집하여 필터 패널에서 [사용자 정의 검색 패싯](../using/brand-portal-search-facets.md)을 사용할 수 있습니다.

   * **[!UICONTROL 속성]** 예측검색 양식에서 사용되는 경우 조건자가 매핑된 메타데이터 속성과 일치하는 자산을 검색할 수 있습니다.\
      예를 들어 속성 조건자가 [!UICONTROL `jcr:content /metadata/dc:title`]에 매핑된 경우 해당 제목을 기준으로 자산을 검색할 수 있습니다.\
      [!UICONTROL 속성 설명]은 다음 텍스트 검색을 지원합니다.

      **부분 구문**
속성 조건부에서 부분 구문을 사용하여 자산 검색을 허용하도록 검색 양식에서 **[!UICONTROL 부분 검색]** 확인란을 활성화합니다.\
      자산 메타데이터에 사용된 단어/구문을 정확히 지정하지 않더라도 원하는 자산을 검색할 수 있습니다.\
      다음을 작업을 수행할 수 있습니다.
      * 필터 패널의 패싯에서 검색된 구문에서 발생하는 단어를 지정합니다. 예를 들어 **breading**(및 속성 조건자가 [!UICONTROL `dc:title`] 속성에 매핑됨) 용어를 검색하는 경우 제목 구문에 **breading**&#x200B;이라는 단어가 있는 모든 자산이 반환됩니다.
      * 검색한 구문에서 발생하는 단어의 일부와 와일드카드 문자(*)를 지정하여 간격을 채웁니다.
예를 들어 다음을 검색할 수 있습니다.
         * **scaling*** 은 제목 구문에서 &quot;hiking&quot;으로 시작하는 단어가 있는 모든 자산을 반환합니다.
         * ***** 등반은 단어(climb)로 끝나는 모든 자산을 제목처럼 힘들게 만든다.
         * ***climb*** 는 제목 구문에서 &quot;hiking&quot;을 구성하는 단어가 있는 모든 자산을 반환합니다.

속성 조건자에서 대/소문자를 구분하지 않는 검색을 허용하려면       **대/소문자를 구분하지 않는**
텍스트속성 조건자에서 대/소문자를 구분하지 않는 검색을 허용하려면 검색 양식에서  **[!UICONTROL 대소문자]** 무시 확인란을 활성화합니다. 기본적으로 속성 조건자에 대한 텍스트 검색은 대소문자를 구분합니다.
   >[!NOTE]
   >
   >**[!UICONTROL 부분 검색]** 확인란을 선택하면 기본적으로 **[!UICONTROL 대/소문자 무시]**&#x200B;가 선택됩니다.

   ![](assets/wildcard-prop-1.png)

   검색 결과는 적용된 필터와 검색 결과 수에 따라 표시됩니다.

   ![](assets/omnisearch-with-filters.png)

   검색 결과 카운트가 있는 자산 검색 결과.

1. 검색 결과에서 항목을 쉽게 탐색하고 검색 쿼리를 다시 실행하지 않고도 브라우저의 뒤로 단추를 사용하여 동일한 검색 결과로 돌아갈 수 있습니다.

## 검색을 스마트 컬렉션 {#save-your-searches-as-smart-collection}으로 저장

검색 설정을 스마트 컬렉션으로 저장하여 나중에 동일한 설정을 다시 실행하지 않고도 동일한 검색을 빠르게 반복할 수 있습니다.

검색 설정을 스마트 컬렉션으로 저장하려면

1. **[!UICONTROL 스마트 컬렉션 저장]**&#x200B;을 탭/클릭하고 스마트 컬렉션 이름을 입력합니다.

   모든 사용자가 스마트 컬렉션을 액세스할 수 있도록 하려면 **[!UICONTROL Public]**&#x200B;을 선택합니다. 스마트 컬렉션이 만들어지고 저장된 검색 목록에 추가되었음을 확인하는 메시지가 표시됩니다.

   >[!NOTE]
   >
   >관리자가 아닌 사용자는 조직의 브랜드 포털에서 관리자가 아닌 사용자가 만든 많은 수의 공개 스마트 컬렉션을 사용하지 않도록 스마트 컬렉션을 공개하는 것을 제한할 수 있습니다. 조직은 관리 도구 패널에서 **[!UICONTROL 일반]** 설정에서 **[!UICONTROL 공개 스마트 컬렉션 생성 허용]** 구성을 비활성화할 수 있습니다.

   ![](assets/save_smartcollectionui.png)

1. 스마트 컬렉션을 다른 이름으로 저장하고 **[!UICONTROL 공개]** 확인란을 선택하거나 해제하려면 **[!UICONTROL 스마트 컬렉션 편집]**&#x200B;을 클릭합니다.

   ![](assets/edit_smartcollection.png)

1. **[!UICONTROL 스마트 컬렉션 편집]** 대화 상자에서 **[!UICONTROL 다른 이름으로 저장]**&#x200B;을 선택하고 스마트 컬렉션의 이름을 입력합니다. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   ![](assets/saveas_smartsearch.png)
