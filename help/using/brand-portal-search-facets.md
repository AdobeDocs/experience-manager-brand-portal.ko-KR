---
title: 사용자 지정 검색 패싯 사용
seo-title: 사용자 지정 검색 패싯 사용
description: 관리자는 검색 설명을 필터 패널에 추가하여 검색을 사용자 정의하고 검색 기능을 다용도로 만들 수 있습니다.
seo-description: 관리자는 검색 설명을 필터 패널에 추가하여 검색을 사용자 정의하고 검색 기능을 다용도로 만들 수 있습니다.
uuid: 986 fba 5 a-fac 5-4128-ac 75-d 04 da 5 b 52 d 45
content-type: 참조
topic-tags: 관리
products: sg_ Experiencemanager/brand_ portal
discoiquuid: 19 FAA 028-246 B -42 C 7-869 F -97 C 95 C 7 A 1349
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 사용자 지정 검색 패싯 사용 {#use-custom-search-facets}

관리자는 검색 설명을 [!UICONTROL 필터] 패널에 추가하여 검색을 사용자 정의하고 검색 기능을 다용도로 만들 수 있습니다.

브랜드 포털은 승인된 브랜드 에셋의 세부적인 검색에 [대한 패싯 검색을](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) 지원하므로 [**필터** 패널로 인해](../using/brand-portal-searching.md#search-using-facets-in-filters-panel)가능합니다. 검색 패싯은 관리 도구에서 **[!UICONTROL 검색 양식을]** 통해 필터 패널에 사용할 수 있습니다. 에셋 관리자 검색 레일이라는 기본 검색 양식이 관리 도구의 검색 양식 페이지에 있습니다. 하지만 관리자는 검색 설명을 추가, 수정 또는 제거하여 기본 검색 양식 (자산 관리자 검색 레일) 를 편집하여 기본 필터 패널을 사용자 지정할 수 있으므로 검색 기능을 다용도로 만들 수 있습니다.

다양한 검색 설명을 사용하여 **[!UICONTROL 필터]** 패널을 사용자 지정할 수 있습니다. 예를 들어, 이 설명서에서 지정하는 단일 속성과 일치하는 자산을 검색하려면 속성 설명을 추가합니다. 특정 속성에 대해 지정하는 하나 이상의 값과 일치하는 자산을 검색하려면 옵션 설명을 추가합니다. 지정된 날짜 범위 내에서 만든 자산을 검색하려면 날짜 범위 설명을 추가합니다.

>[!NOTE]
>
>AEM 에서는 조직에서 브랜드 [포털에서 동일한 양식을 다시 만들지 않고 AEM 작성자에서](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) 브랜드 포털에 사용자 지정된 검색 양식을 게시할 수 있습니다.

## 검색 설명 추가 {#add-a-search-predicate}

**[!UICONTROL 필터]** 패널에 검색 설명을 추가하려면:

1. 관리 도구에 액세스하려면 맨 위의 도구 모음에서 AEM 로고를 클릭합니다.

   ![](assets/aemlogo.png)

2. [관리 도구] 패널에서 [양식 **[!UICONTROL 검색] 를 클릭합니다]**.

   ![](assets/navigation-panel-1.png)

3. 양식 **[!UICONTROL 검색]** 페이지에서 **[!UICONTROL 자산 관리 검색 레일을 선택합니다]**.

   ![](assets/search-forms-page.png)

4. 상단에 표시되는 도구 모음에서 **[!UICONTROL 편집을]** 클릭하여 검색 편집 양식을 엽니다.

   ![](assets/edit-search-form-1.png)

5. 검색 양식 [!UICONTROL 편집] 페이지의 설명 [!UICONTROL 선택] 탭에서 기본 창으로 설명을 드래그합니다. 예를 들어 **[!UICONTROL 속성 설명을 드래그합니다]**.

   **[!UICONTROL 속성]** 필드는 기본 창에 나타나며 오른쪽의 **[!UICONTROL 설정]** 탭에는 속성 예측이 표시됩니다.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >**[!UICONTROL 설정]** 탭의 머리글 레이블은 선택하는 설명 유형을 식별합니다.

6. **[!UICONTROL [설정]** ] 탭에서 속성 설명 레이블, 자리 표시자 텍스트 및 설명을 입력합니다.

   * 지정된 속성 값을 기반으로 자산의 구문 검색 (및 와일드카드 검색) 를 허용하려면 **[!UICONTROL 부분 검색을]**&#x200B;선택합니다. 기본적으로, 설명자는 전체 텍스트 검색을 지원합니다.
   * 속성 값을 기반으로 자산 검색을 대/소문자를 구분하지 않으려면 대/소문자 ****&#x200B;무시를 선택합니다. 기본적으로 검색 필터에서 속성 값 검색은 대/소문자를 구분합니다.
   >[!NOTE]
   >
   >**[!UICONTROL 부분 검색]** 확인란을 선택할 때 대/소문자를 [!UICONTROL 무시하면 기본적으로 선택됩니다] .

7. [!UICONTROL 속성 이름] 필드에서 속성 선택기를 열고 수행되는 검색을 기반으로 속성을 선택합니다. 또는 속성의 이름을 입력합니다. [!UICONTROL `  jcr :content/metadata/dc:title`][!UICONTROL `./jcr:content/metadata/dc:title`]예를 들어 또는을 입력합니다.

   ![](assets/title-prop.png)

8. **[!UICONTROL 완료를]** 클릭하여 설정을 저장합니다.
9. [!UICONTROL 자산] 사용자 인터페이스에서 오버레이 아이콘을 클릭하고 **[!UICONTROL 필터를]** 선택하여 **[!UICONTROL 필터]** 패널로 이동합니다. **[!UICONTROL 속성]** 설명이 패널에 추가됩니다.

   ![](assets/property-filter-panel.png)

10. **[!UICONTROL 속성]** 텍스트 상자에서 검색할 자산의 제목을 입력합니다. 예: "adobe". 검색을 수행하면 검색 결과에 제목이 "adobe" 인 자산이 표시됩니다.

## 검색 설명 목록 {#list-of-search-predicates}

**[!UICONTROL 속성]** 설명을 추가하는 방식과 유사하게 **[!UICONTROL , 필터]** 패널에 다음 설명을 추가할 수 있습니다.

| **설명 이름** | **설명** | **속성** |
|-------|-------|----------|
| [!UICONTROL 경로 브라우저] | 검색 설명을 사용하여 특정 위치에서 자산을 검색합니다. **참고:***로그인한 사용자의 경우, 필터의 경로 브라우저에 사용자와 공유된 폴더 (및 해당 상위 항목) 의 컨텐츠 구조만 표시됩니다.*<br> 관리 사용자는 경로 브라우저를 사용하여 해당 폴더로 이동하여 모든 폴더에서 자산을 검색할 수 있습니다. <br> 반면에 관리자가 아닌 사용자는 경로 브라우저의 해당 폴더로 이동하여 폴더 (액세스 가능) 폴더에서 에셋을 검색할 수 있습니다. | <ul><li>필드 레이블</li><li>경로</li><li>설명</li></ul> |
| [!UICONTROL 속성] | 특정 메타데이터 속성을 기반으로 자산을 검색합니다. **참고:***부분 검색을 선택하면 대/소문자 무시가 기본적으로 선택됩니다*. | <ul><li>필드 레이블</li><li>자리 표시자</li><li>속성 이름</li><li>부분 검색</li><li>대소문자 구분 안 함</li><li> 설명</li></ul> |
| [!UICONTROL 다중 값 속성] | 속성 설명으로 유사하지만 여러 개의 입력 값을 구분 기호로 구분하고 (기본값은 쉼표 (기본값은 쉼표[,]) 입력 값 중 하나라도 일치하는 자산은 결과에 반환됩니다. | <ul><li>필드 레이블</li><li>자리 표시자</li><li>속성 이름</li><li>구분 기호 지원</li><li>대소문자 구분 안 함</li><li>설명</li></ul> |
| [!UICONTROL 태그] | 검색 설명을 사용하여 태그를 기반으로 자산을 검색합니다. 태그 목록에 다양한 태그를 채우도록 경로 속성을 구성할 수 있습니다. * 참고: 예를 들어, 관리자가 AEM에서 검색 양식을 [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`]게시하면, 경로에 임차인 정보가 포함되지 않는 등의 경로 값을 변경해야 할 수 [!UICONTROL `/etc/tags/<custom_tag_namespace>`]있습니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>경로</li><li>설명</li></ul> |
| [!UICONTROL 경로] | 검색 설명을 사용하여 특정 위치에서 자산을 검색합니다. | <ul><li>필드 레이블</li><li>경로</li><li>설명</li></ul> |  |
| [!UICONTROL 상대적 날짜] | 검색 설명을 사용하여 작성자의 상대적 날짜를 기준으로 자산을 검색합니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>상대적 날짜</li></ul> |
| [!UICONTROL 범위] | 검색 설명서에서는 지정된 속성 값 범위에 속하는 자산을 검색합니다. [필터] 패널에서 범위에 대한 최소 및 최대 속성 값을 지정할 수 있습니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| [!UICONTROL 날짜 범위] | 날짜 속성에 대해 지정된 범위 내에서 만든 자산을 검색하려면 검색 설명을 참조하십시오. 필터 패널에서 시작 날짜와 종료 날짜를 지정할 수 있습니다. | <ul><li>필드 레이블</li><li>자리 표시자</li><li>속성 이름</li><li>범위 텍스트 (위치)</li><li>범위 텍스트 (to)</li><li>설명</li></ul> |
| [!UICONTROL 날짜] | 날짜 속성을 기반으로 한 자산의 슬라이더 기반 검색을 위한 검색 조건자입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| [!UICONTROL 파일 크기] | 검색 설명서에서는 해당 크기에 따라 자산을 검색합니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>경로</li><li>설명</li></ul> |
| [!UICONTROL 마지막으로 수정된 자산] | 검색 설명을 사용하여 마지막으로 수정한 날짜를 기준으로 자산을 검색합니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| [!UICONTROL 승인 상태] | 승인 메타데이터 속성을 기반으로 자산을 검색하려면 검색 설명을 참조하십시오. 기본 속성 이름은 **DAM 입니다. 상태**. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| [!UICONTROL 체크아웃 상태] | AEM 자산에서 게시되었을 때 자산의 체크아웃 상태를 기반으로 자산을 검색하려면 검색 설명을 사용합니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| [!UICONTROL 체크아웃 기준] | 검색 설명서에서는 자산을 체크아웃한 사용자를 기반으로 자산을 검색합니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| [!UICONTROL 만료 상태] | 만료 상태를 기반으로 자산을 검색합니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| [!UICONTROL 컬렉션의 멤버] | 검색 설명서에서는 자산이 컬렉션의 일부인지 여부를 기반으로 자산을 검색합니다. | 설명 |
| [!UICONTROL 숨김] | 이 설명은 최종 사용자에게 명시적으로 표시되지 않으며, 일반적으로 DAM로 **검색 결과 유형을 제한하는 숨겨진 제한에 사용됩니다.**&#x200B;자산. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |

>[!NOTE]
>
>이러한 예측은 브랜드 포털에서 기능하지 않으므로 **[!UICONTROL 옵션 설명]**, **[!UICONTROL 게시 상태 설명]**&#x200B;및 **[!UICONTROL 등급 언급을]** 사용하지 마십시오.

## 검색 설명 삭제 {#delete-a-search-predicate}

검색 설명을 삭제하려면 다음 단계를 수행합니다.

1. Adobe 로고를 클릭하여 관리 도구에 액세스합니다.

   ![](assets/aemlogo.png)

2. [관리 도구] 패널에서 [양식 **[!UICONTROL 검색] 를 클릭합니다]**.

   ![](assets/navigation-panel-2.png)

3. 양식 **[!UICONTROL 검색]** 페이지에서 **[!UICONTROL 자산 관리 검색 레일을 선택합니다]**.

   ![](assets/search-forms-page.png)

4. 상단에 표시되는 도구 모음에서 **[!UICONTROL 편집을]** 클릭하여 검색 편집 양식을 엽니다.

   ![](assets/edit-search-form-2.png)

5. 검색 양식 [!UICONTROL 편집] 페이지의 주 창에서 삭제할 설명을 선택합니다. 예를 들어 **[!UICONTROL 속성 설명을 선택합니다]**.

   오른쪽의 **[!UICONTROL 설정]** 탭에는 속성 설명 필드가 표시됩니다.

6. 속성 설명을 삭제하려면 저장소 아이콘을 클릭합니다. 필드 **[!UICONTROL 삭제]** 대화 상자에서 **[!UICONTROL 삭제를]** 클릭하여 삭제 작업을 확인합니다.

   속성 **[!UICONTROL 설명]** 필드가 주 창에서 제거되고 **[!UICONTROL 설정]** 탭이 비어 있게 됩니다.

   ![](assets/search-form-delete-predicate.png)

7. 변경 내용을 저장하려면 도구 모음에서 **[!UICONTROL 완료를]** 클릭합니다.
8. **[!UICONTROL 자산]** 사용자 인터페이스에서 오버레이 아이콘을 클릭하고 **[!UICONTROL 필터를]** 선택하여 **[!UICONTROL 필터]** 패널로 이동합니다. **[!UICONTROL 속성]** 설명이 패널에서 제거됩니다.

   ![](assets/property-predicate-removed.png)
