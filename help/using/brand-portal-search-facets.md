---
title: Use custom search facets
seo-title: Use custom search facets
description: Administrators can add search predicates to the Filters panel to customize search and make the search functionality versatile.
seo-description: Administrators can add search predicates to the Filters panel to customize search and make the search functionality versatile.
uuid: 986fba5a-fac5-4128-ac75-d04da5b52d45
content-type: 참조
topic-tags: 관리
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d

---


# Use custom search facets {#use-custom-search-facets}

Administrators can add search predicates to the Filters panel to customize search and make the search functionality versatile.

브랜드 포털은 승인된 브랜드 자산을 세부적으로 검색하는 [패싯된 검색을](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) 지원합니다. 이는 필터 패널로 인해 [**가능합니다**](../using/brand-portal-searching.md#search-using-facets-in-filters-panel). Search facets are made available on Filters panel through Search Form in the admin tools. **** 관리 도구의 검색 양식 페이지에 자산 관리 검색 레일이라고 하는 기본 검색 양식이 있습니다. However, Administrators can customize the default Filters panel by editing the default Search Form (Asset Admin Search Rail) by adding, modifying, or removing search predicates, thereby making the search functionality versatile.

You can use various search predicates to customize the Filters panel. **** For example, add the property predicate to search for assets that match a single property that you specify in this predicate. Add the options predicate to search for assets that match one or more values that you specify for a particular property. Add the date range predicate to search for assets created within a specified date range.

>[!NOTE]
>
>AEM에서는 조직에서 브랜드 포털에서 동일한 양식을 다시 만드는 대신 AEM [](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) 작성자의 맞춤형 검색 양식을 브랜드 포털에 게시할 수 있습니다.

## 검색 설명 추가 {#add-a-search-predicate}

필터 패널에 검색 조건자를 추가하려면 **[!UICONTROL 다음을]** 수행합니다.

1. 관리 도구에 액세스하려면 맨 위의 도구 모음에서 AEM 로고를 클릭합니다.

   ![](assets/aemlogo.png)

1. 관리 도구 패널에서 양식 **[!UICONTROL 검색을 클릭합니다]**.

   ![](assets/navigation-panel-1.png)

1. [ **[!UICONTROL 양식 검색]** ] 페이지에서 자산 **[!UICONTROL 관리 검색 레일을 선택합니다]**.

   ![](assets/search-forms-page.png)

1. 상단에 표시되는 도구 모음에서 편집을 클릭하여 **[!UICONTROL 검색]** 편집 양식을 엽니다.

   ![](assets/edit-search-form-1.png)

1. 검색 [!UICONTROL 양식 편집] 페이지에서 설명 선택 [!UICONTROL 탭에서] 기본 창으로 조건자를 드래그합니다. 예를 들어 속성 **[!UICONTROL 조건자를 드래그합니다]**.

   속성 **[!UICONTROL 필드가]** 기본 창에 나타나고 오른쪽의 설정 **[!UICONTROL 탭에]** 속성 예측이 표시됩니다.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >설정 탭의 헤더 레이블은 **[!UICONTROL 선택한]** 조건자의 유형을 식별합니다.

1. 설정 **[!UICONTROL 탭에서]** 속성 조건자에 대한 레이블, 자리 표시자 텍스트 및 설명을 입력합니다.

   * 지정된 **[!UICONTROL 속성]**&#x200B;값을 기반으로 자산의 부분 구문 검색(및 와일드카드 검색)을 허용하려면 부분 검색을 선택합니다. 기본적으로 술어는 전체 텍스트 검색을 지원합니다.
   * 속성 **[!UICONTROL 값을]**&#x200B;기반으로 하는 자산 검색을 대/소문자를 구분하지 않도록 하려면 [대/소문자 무시]를 선택합니다. 기본적으로 검색 필터에서 속성 값 검색은 대소문자를 구분합니다.
   >[!NOTE]
   >
   >부분 검색 **[!UICONTROL 확인란을 선택하면]** 기본적으로 [!UICONTROL 대소문자] 무시가 선택됩니다.

1. 속성 [!UICONTROL 이름] 필드에서 속성 선택기를 열고 검색이 수행되는 속성을 선택합니다. 또는 속성 이름을 입력합니다. 예를 들어, enter [!UICONTROL `  jcr :content/metadata/dc:title`] 또는 [!UICONTROL `./jcr:content/metadata/dc:title`]를 입력합니다.

   ![](assets/title-prop.png)

1. 완료를 **[!UICONTROL 클릭하여]** 설정을 저장합니다.
1. 자산 [!UICONTROL 사용자 인터페이스에서] 오버레이 아이콘을 클릭하고 필터를 선택하여 **[!UICONTROL 필터]** **[!UICONTROL 패널로]** 이동합니다. 속성 **[!UICONTROL 조건자가]** 패널에 추가됩니다.

   ![](assets/property-filter-panel.png)

1. 속성 텍스트 상자에 검색할 자산의 제목을 **[!UICONTROL 입력합니다]** . 예: "Adobe" 검색을 수행하면 제목이 "Adobe"와 일치하는 자산이 검색 결과에 표시됩니다.

## 검색 조건자 목록 {#list-of-search-predicates}

Similar to the way you add a Property predicate, you can add the following predicates to the Filters panel:********

| **설명 이름** | **설명** | **속성** |
|-------|-------|----------|
| [!UICONTROL 경로 브라우저] | Search predicate to search assets at a particular location. **** 참고: For a logged-in user, path browser on Filter shows only the content structure of the folders (and their ancestors) shared with the user.**  Admin users can search assets in any folder by navigating to that folder using Path Browser. <br> <br> Whereas, non-admin users can search assets in a folder (accessible to them) by navigating to that folder in Path Browser. | <ul><li>필드 레이블</li><li>경로</li><li>설명</li></ul> |
| [!UICONTROL 속성] | Search assets based on a particular metadata property. **** 참고: On selecting Partial Search, Ignore Case is selected by default.** | <ul><li>필드 레이블</li><li>자리 표시자</li><li>속성 이름</li><li>부분 검색</li><li>대소문자 구분 안 함</li><li> 설명</li></ul> |
| [!UICONTROL Multi-Value Property] | Similar to property predicate but allows multiple input values, separated by a delimiter (default is COMMA,) assets matching any of the input values are returned in results.[] | <ul><li>필드 레이블</li><li>자리 표시자</li><li>Property name</li><li>구분 기호 지원</li><li>대소문자 구분 안 함</li><li>설명</li></ul> |
| [!UICONTROL 태그] | Search predicate to search assets based on tags. You can configure the Path property to populate various tags in the Tags list. *Note: Administrators might need to change the path value, for example, , if they publish the search form from AEM, where the path does not include tenant information, for example, .[!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`][!UICONTROL `/etc/tags/<custom_tag_namespace>`] | <ul><li>필드 레이블</li><li>Property name</li><li>경로</li><li>설명</li></ul> |
| [!UICONTROL 경로] | Search predicate to search assets at a particular location. | <ul><li>필드 레이블</li><li>경로</li><li>설명</li></ul> |  |
| [!UICONTROL 상대적 날짜] | Search predicate to search assets based on the relative date of their creation. | <ul><li>필드 레이블</li><li>Property name</li><li>상대적 날짜</li></ul> |
| [!UICONTROL 범위] | 검색 조건자를 사용하여 지정된 속성 값 범위 내에 있는 자산을 검색합니다. In the Filters panel, you can specify minimum and maximum property values for the range. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| [!UICONTROL 날짜 범위] | 검색 조건자를 사용하여 날짜 속성에 대해 지정된 범위 내에서 생성된 자산을 검색합니다. 필터 패널에서 시작 날짜와 종료 날짜를 지정할 수 있습니다. | <ul><li>필드 레이블</li><li>자리 표시자</li><li>속성 이름</li><li>범위 텍스트(시작)</li><li>범위 텍스트(끝)</li><li>설명</li></ul> |
| [!UICONTROL 날짜] | 날짜 속성을 기반으로 한 슬라이더 기반의 자산 검색에 대한 검색 조건자입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| [!UICONTROL 파일 크기] | 검색 조건자를 사용하여 크기를 기반으로 자산을 검색합니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>경로</li><li>설명</li></ul> |
| [!UICONTROL 마지막으로 수정된 자산] | 검색 조건자를 사용하여 마지막으로 수정한 날짜를 기준으로 자산을 검색합니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| [!UICONTROL 승인 상태] | 검색 조건자를 사용하여 승인 메타데이터 속성을 기반으로 자산을 검색합니다. 기본 속성 이름은 **dam:status**&#x200B;입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| [!UICONTROL 체크아웃 상태] | 검색 조건자를 사용하여 AEM 자산에서 게시되었을 때 자산의 체크 아웃 상태를 기반으로 자산을 검색합니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| [!UICONTROL 체크아웃 기준] | 검색 조건자를 사용하여 자산을 체크 아웃한 사용자를 기반으로 자산을 검색합니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| [!UICONTROL 만료 상태] | 만료 상태를 기반으로 에셋을 검색하도록 조건자를 검색합니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| [!UICONTROL 컬렉션 구성원] | 검색 조건자를 사용하여 자산이 컬렉션의 일부인지 여부를 기반으로 자산을 검색합니다. | 설명 |
| [!UICONTROL 숨김] | 이 조건자는 최종 사용자에게 명시적으로 표시되지 않으며 일반적으로 검색 결과 유형을 **dam:Asset으로 제한하는 숨겨진 제약 조건에 사용됩니다**. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |

>[!NOTE]
>
>이러한 조건자가 브랜드 **[!UICONTROL 포털에서 작동하지]**&#x200B;않으므로 옵션 설명 **[!UICONTROL , 게시 상태 설명]**&#x200B;및 **[!UICONTROL 등급]** 조건자를 사용하지 마십시오.

## 검색 설명 삭제 {#delete-a-search-predicate}

검색 조건자를 삭제하려면 다음 단계를 수행합니다.

1. Adobe 로고를 클릭하여 관리 도구에 액세스합니다.

   ![](assets/aemlogo.png)

1. 관리 도구 패널에서 양식 **[!UICONTROL 검색을 클릭합니다]**.

   ![](assets/navigation-panel-2.png)

1. [ **[!UICONTROL 양식 검색]** ] 페이지에서 자산 **[!UICONTROL 관리 검색 레일을 선택합니다]**.

   ![](assets/search-forms-page.png)

1. 상단에 표시되는 도구 모음에서 편집을 클릭하여 **[!UICONTROL 검색]** 편집 양식을 엽니다.

   ![](assets/edit-search-form-2.png)

1. 검색 [!UICONTROL 양식 편집] 페이지의 기본 창에서 삭제할 조건자를 선택합니다. 예를 들어 속성 **[!UICONTROL 조건자를 선택합니다]**.

   오른쪽의 **[!UICONTROL 설정]** 탭에는 속성 설명 필드가 표시됩니다.

1. 속성 조건자를 삭제하려면 bin 아이콘을 클릭합니다. 필드 **[!UICONTROL 삭제]** 대화 상자에서 삭제를 클릭하여 **[!UICONTROL 삭제]** 작업을 확인합니다.

   속성 **[!UICONTROL 설명]** 필드는 주 창에서 제거되고 설정 **[!UICONTROL 탭이]** 비어 있게 됩니다.

   ![](assets/search-form-delete-predicate.png)

1. To save the changes, click Done in the toolbar.****
1. From the Assets user interface, click the overlay icon and choose Filter to navigate to the Filters panel. ************ The Property predicate is removed from the panel.****

   ![](assets/property-predicate-removed.png)
