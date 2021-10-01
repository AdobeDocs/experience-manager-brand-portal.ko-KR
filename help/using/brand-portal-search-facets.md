---
title: 사용자 정의 검색 패싯 사용
seo-title: Use custom search facets
description: 관리자는 필터 패널에 검색 설명을 추가하여 검색을 사용자 지정하고 검색 기능을 다양하게 만들 수 있습니다.
seo-description: Administrators can add search predicates to the Filters panel to customize search and make the search functionality versatile.
uuid: 986fba5a-fac5-4128-ac75-d04da5b52d45
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
role: Admin
exl-id: c07e1268-2c83-40ba-8dcd-5dade3a10141
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '1279'
ht-degree: 9%

---

# 사용자 정의 검색 패싯 사용 {#use-custom-search-facets}

관리자는 [!UICONTROL 필터] 패널에 검색 조건자를 추가하여 검색을 사용자 지정하고 검색 기능을 다양하게 만들 수 있습니다.

Brand Portal은 [**필터** 패널](../using/brand-portal-searching.md#search-using-facets-in-filters-panel)로 인해 가능한 승인된 브랜드 자산의 세부 검색에 대해 [면처리된 검색](../using/brand-portal-searching.md#search-using-facets-in-filters-panel)을 지원합니다. 검색 패싯은 관리 도구에서 **[!UICONTROL 검색 양식]**&#x200B;을 통해 필터 패널에서 사용할 수 있게 됩니다. Asset Admin 검색 레일이라고 하는 기본 검색 양식이 관리 도구의 Forms 검색 페이지에 있습니다. 그러나 관리자는 검색 조건자를 추가, 수정 또는 제거하여 기본 검색 양식(자산 관리 검색 레일)을 편집하여 기본 필터 패널을 사용자 지정함으로써 검색 기능을 다양한 용도로 사용할 수 있습니다.

다양한 검색 조건자를 사용하여 **[!UICONTROL 필터]** 패널을 사용자 지정할 수 있습니다. 예를 들어, 이 조건부에서 지정하는 단일 속성과 일치하는 자산을 검색하도록 속성 설명을 추가합니다. 옵션 설명을 추가하여 특정 속성에 대해 지정하는 하나 이상의 값과 일치하는 자산을 검색합니다. 지정된 날짜 범위 내에서 생성된 자산을 검색하려면 날짜 범위 설명을 추가합니다.

>[!NOTE]
>
>조직에서 Experience Manager 자산을 사용하면 Brand Portal에서 동일한 양식을 다시 만드는 대신 [AEM 작성자](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal)에서 Brand Portal으로 사용자 지정된 검색 양식을 게시할 수 있습니다.

## 검색 설명 추가 {#add-a-search-predicate}

**[!UICONTROL 필터]** 패널에 검색 설명을 추가하려면:

1. 관리 도구에 액세스하려면 맨 위의 도구 모음에서 Experience Manager 로고를 클릭합니다.

   ![](assets/aemlogo.png)

1. 관리 도구 패널에서 **[!UICONTROL Forms 검색]**&#x200B;을 클릭합니다.

   ![](assets/navigation-panel-1.png)

1. **[!UICONTROL Forms 검색]** 페이지에서 **[!UICONTROL 자산 관리 검색 레일]**&#x200B;을 선택합니다.

   ![](assets/search-forms-page.png)

1. 맨 위에 표시되는 도구 모음에서 **[!UICONTROL 편집]**&#x200B;을 클릭하여 편집 검색 양식을 엽니다.

   ![](assets/edit-search-form-1.png)

1. [!UICONTROL 검색 양식 편집] 페이지에서 [!UICONTROL 설명 선택] 탭의 설명을 기본 창으로 드래그합니다. 예를 들어 **[!UICONTROL 속성 조건자]**&#x200B;를 드래그합니다.

   **[!UICONTROL 속성]** 필드가 기본 창에 나타나고 오른쪽의 **[!UICONTROL 설정]** 탭에는 속성 설명이 표시됩니다.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >**[!UICONTROL 설정]** 탭의 헤더 레이블은 선택한 조건자의 유형을 식별합니다.

1. **[!UICONTROL 설정]** 탭에서 속성 조건자에 대한 레이블, 자리 표시자 텍스트 및 설명을 입력합니다.

   * 지정된 속성 값을 기준으로 자산의 부분 구문 검색(및 와일드카드 검색)을 허용하려면 **[!UICONTROL 부분 검색]**&#x200B;을 선택합니다. 기본적으로 조건부는 전체 텍스트 검색을 지원합니다.
   * 속성 값을 기반으로 하는 자산 검색을 대/소문자를 구분하지 않게 하려면 **[!UICONTROL 대/소문자 무시]**&#x200B;를 선택합니다. 기본적으로 검색 필터에서 속성 값을 검색하는 것은 대/소문자를 구분합니다.

   >[!NOTE]
   >
   >**[!UICONTROL 부분 검색]** 확인란을 선택하면 기본적으로 **[!UICONTROL 대/소문자 무시]**&#x200B;가 선택됩니다.

1. **[!UICONTROL 속성 이름]** 필드에서 속성 선택기를 열고 검색이 수행되는 속성을 선택합니다. 또는 속성의 이름을 입력합니다. 예를 들어 `  jcr :content/metadata/dc:title` 또는 `./jcr:content/metadata/dc:title`을 입력합니다.

   >[!NOTE]
   >
   >Brand Portal에서 `dam:asset`의 `jcrcontent/metadata`에 있는 모든 속성(`xmp`으로 시작하는 속성 제외)은 기본적으로 색인화됩니다.
   >
   >인덱싱된 속성은 속성 설명을 만드는 동안 사용할 수 있습니다. 인덱싱되지 않은 속성이 구성된 경우 인덱싱되지 않은 속성에 대한 검색 쿼리에 검색 결과가 표시되지 않을 수 있습니다.

   ![](assets/title-prop.png)

1. **[!UICONTROL 완료]** 를 클릭하여 설정을 저장합니다.
1. [!UICONTROL Assets] 사용자 인터페이스에서 오버레이 아이콘을 클릭하고 **[!UICONTROL 필터]**&#x200B;를 선택하여 **[!UICONTROL 필터]** 패널로 이동합니다. **[!UICONTROL 속성]** 설명이 패널에 추가됩니다.

   ![](assets/property-filter-panel.png)

1. **[!UICONTROL 속성]** 텍스트 상자에서 검색할 자산의 제목을 입력합니다. 예: &quot;Adobe&quot; 검색을 수행하면 제목이 &quot;Adobe&quot;과 일치하는 자산이 검색 결과에 표시됩니다.

## 검색 설명 목록 {#list-of-search-predicates}

**[!UICONTROL 속성]** 조건자를 추가하는 방법과 유사하게 **[!UICONTROL 필터]** 패널에 다음 조건자를 추가할 수 있습니다.

| **설명 이름** | **설명** | **속성** |
|-------|-------|----------|
| **[!UICONTROL 경로 브라우저]** | 특정 위치에서 자산을 검색하려면 검색 조건자를 사용하십시오. **참고:** *로그인한 사용자의 경우, 필터의 경로 브라우저에는 사용자와 공유되는 폴더(및 해당 상위 폴더)의 컨텐츠 구조만 표시됩니다.* <br> 관리자 사용자는 경로 브라우저를 사용하여 해당 폴더로 이동하여 임의의 폴더에서 자산을 검색할 수 있습니다. <br> 반면에, 관리자가 아닌 사용자는 경로 브라우저에서 해당 폴더로 이동하여 폴더의 자산을 검색할 수 있습니다(사용자가 액세스할 수 있음). | <ul><li>필드 레이블</li><li>경로</li><li>설명</li></ul> |
| **[!UICONTROL 속성]** | 특정 메타데이터 속성을 기반으로 자산을 검색합니다. **참고:** *부분 검색을 선택할 때 기본적으로 대소문자 무시 가 선택됩니다*. | <ul><li>필드 레이블</li><li>자리 표시자</li><li>속성 이름</li><li>부분 검색</li><li>대소문자 구분 안 함</li><li> 설명</li></ul> |
| **[!UICONTROL 다중 값 속성]** | 속성 조건자와 유사하지만, 구분 기호로 구분된 여러 개의 입력 값을 허용합니다(기본값은 COMMA[,]) 입력 값과 일치하는 자산이 결과에 반환됩니다. | <ul><li>필드 레이블</li><li>자리 표시자</li><li>속성 이름</li><li>구분 기호 지원</li><li>대소문자 구분 안 함</li><li>설명</li></ul> |
| **[!UICONTROL 태그]** | 검색 조건자를 사용하여 태그를 기반으로 자산을 검색합니다. 태그 목록에서 다양한 태그를 채우도록 경로 속성을 구성할 수 있습니다. *참고: 관리자는 경로 값(예: [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`])을 변경해야 할 수 있습니다. AEM에서 검색 양식을 게시하면 경로에 테넌트 정보가 포함되지 않습니다(예: [!UICONTROL `/etc/tags/<custom_tag_namespace>`]). | <ul><li>필드 레이블</li><li>속성 이름</li><li>경로</li><li>설명</li></ul> |
| **[!UICONTROL 경로]** | 특정 위치에서 자산을 검색하려면 검색 조건자를 사용하십시오. | <ul><li>필드 레이블</li><li>경로</li><li>설명</li></ul> |  |
| **[!UICONTROL 상대적 날짜]** | 검색 조건자를 사용하여 자산의 상대적 날짜에 따라 자산을 검색합니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>상대적 날짜</li></ul> |
| **[!UICONTROL 범위]** | 검색 조건자를 사용하여 지정된 속성 값 범위 내에 있는 자산을 검색합니다. [필터] 패널에서 범위에 대한 최소 및 최대 속성 값을 지정할 수 있습니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 날짜 범위]** | 검색 조건자를 사용하여 날짜 속성에 대해 지정된 범위 내에서 생성된 자산을 검색합니다. 필터 패널에서 시작 및 종료 날짜를 지정할 수 있습니다. | <ul><li>필드 레이블</li><li>자리 표시자</li><li>속성 이름</li><li>범위 텍스트(시작)</li><li>범위 텍스트(끝)</li><li>설명</li></ul> |
| **[!UICONTROL 날짜]** | 날짜 속성을 기반으로 자산의 슬라이더 기반 검색에 대한 검색 조건입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 파일 크기]** | 검색 조건자를 사용하여 크기를 기준으로 자산을 검색합니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>경로</li><li>설명</li></ul> |
| **[!UICONTROL 마지막으로 수정된 자산]** | 검색 조건자를 사용하여 마지막으로 수정된 날짜를 기준으로 자산을 검색합니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 승인 상태]** | 검색 조건자를 사용하여 승인 메타데이터 속성을 기반으로 자산을 검색합니다. 기본 속성 이름은 **dam:status**&#x200B;입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 체크아웃 상태]** | AEM Assets에서 게시되었을 때 자산의 체크아웃 상태에 따라 자산을 검색할 수 있도록 검색 조건입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 체크아웃 기준]** | 검색 조건자를 사용하여 자산을 체크 아웃한 사용자를 기반으로 자산을 검색합니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 만료 상태]** | 검색 조건자를 사용하여 만료 상태에 따라 자산을 검색합니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 컬렉션의 멤버]** | 검색 조건자를 사용하여 자산이 컬렉션의 일부인지 여부에 따라 자산을 검색합니다. | 설명 |
| **[!UICONTROL 숨김]** | 이 조건자는 최종 사용자가 명시적으로 볼 수 없으며 일반적으로 검색 결과 유형을 **dam:Asset**&#x200B;로 제한하는 숨겨진 제약 조건에 사용됩니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |

>[!NOTE]
>
>이러한 설명이 Brand Portal에서 작동하지 않으므로 **[!UICONTROL 옵션 설명]**, **[!UICONTROL 게시 상태 설명]** 및 **[!UICONTROL 등급 설명]**&#x200B;을 사용하지 마십시오.

## 검색 설명 삭제 {#delete-a-search-predicate}

검색 설명을 삭제하려면 다음 단계를 수행합니다.

1. 관리 도구에 액세스하려면 Adobe 로고를 클릭하십시오.

   ![](assets/aemlogo.png)

1. 관리 도구 패널에서 **[!UICONTROL Forms 검색]**&#x200B;을 클릭합니다.

   ![](assets/navigation-panel-2.png)

1. **[!UICONTROL Forms 검색]** 페이지에서 **[!UICONTROL 자산 관리 검색 레일]**&#x200B;을 선택합니다.

   ![](assets/search-forms-page.png)

1. 맨 위에 표시되는 도구 모음에서 **[!UICONTROL 편집]**&#x200B;을 클릭하여 편집 검색 양식을 엽니다.

   ![](assets/edit-search-form-2.png)

1. [!UICONTROL 검색 양식 편집] 페이지의 기본 창에서 삭제할 설명을 선택합니다. 예를 들어 **[!UICONTROL 속성 설명]**&#x200B;을 선택합니다.

   오른쪽의 **[!UICONTROL 설정]** 탭에는 속성 설명 필드가 표시됩니다.

1. 속성 설명을 삭제하려면 bin 아이콘을 클릭합니다. **[!UICONTROL 필드 삭제]** 대화 상자에서 **[!UICONTROL 삭제]**&#x200B;를 클릭하여 삭제 작업을 확인합니다.

   **[!UICONTROL 속성 설명]** 필드가 기본 창에서 제거되고 **[!UICONTROL 설정]** 탭이 비어 있습니다.

   ![](assets/search-form-delete-predicate.png)

1. 변경 사항을 저장하려면 도구 모음에서 **[!UICONTROL 완료]** 를 클릭합니다.
1. **[!UICONTROL Assets]** 사용자 인터페이스에서 오버레이 아이콘을 클릭하고 **[!UICONTROL 필터]**&#x200B;를 선택하여 **[!UICONTROL 필터]** 패널로 이동합니다. **[!UICONTROL 속성]** 조건부가 패널에서 제거됩니다.

   ![](assets/property-predicate-removed.png)
