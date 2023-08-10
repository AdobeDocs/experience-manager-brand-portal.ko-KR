---
title: 사용자 정의 검색 패싯 사용
seo-title: Use custom search facets
description: 관리자는 필터 패널에 검색 술어를 추가하여 검색을 사용자 정의하고 검색 기능을 다용도로 만들 수 있습니다.
seo-description: Administrators can add search predicates to the Filters panel to customize search and make the search functionality versatile.
uuid: 986fba5a-fac5-4128-ac75-d04da5b52d45
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
role: Admin
exl-id: c07e1268-2c83-40ba-8dcd-5dade3a10141
source-git-commit: 24e15fd8f609505a197d3615b113bef6318ee850
workflow-type: tm+mt
source-wordcount: '1312'
ht-degree: 10%

---

# 사용자 정의 검색 패싯 사용 {#use-custom-search-facets}

관리자는 검색 조건자에 [!UICONTROL 필터] 패널을 통해 검색을 사용자 정의하고 검색 기능을 다양하게 사용할 수 있습니다.

Brand Portal 지원 [패싯된 검색](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) 승인된 브랜드 자산의 세분화된 검색을 위해, 다음 이유로 인해 가능한: [**필터** 패널](../using/brand-portal-searching.md#search-using-facets-in-filters-panel). 검색 패싯은 다음을 통해 필터 패널에서 사용할 수 있습니다. **[!UICONTROL 검색 양식]** 을 참조하십시오. 자산 관리자 검색 레일이라는 기본 검색 양식이 관리 도구의 Forms 검색 페이지에 있습니다. 그러나 관리자는 검색 술어를 추가, 수정 또는 제거하여 기본 검색 양식(에셋 관리자 검색 레일)을 편집하여 기본 필터 패널을 사용자 정의하여 검색 기능을 다용화할 수 있습니다.

다양한 검색 술어를 사용하여 **[!UICONTROL 필터]** 패널. 예를 들어 속성 술어를 추가하여 이 술어에 지정하는 단일 속성과 일치하는 에셋을 검색합니다. 특정 속성에 대해 지정한 하나 이상의 값과 일치하는 에셋을 검색하려면 옵션 술어를 추가합니다. 지정된 날짜 범위 내에 생성된 에셋을 검색하려면 날짜 범위 술어를 추가합니다.

>[!NOTE]
>
>Experience Manager Assets을 통해 다음을 수행할 수 있습니다. [aem 작성자에서 사용자 지정된 검색 양식 게시](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) 동일한 양식을 Brand Portal에서 다시 만드는 대신 Brand Portal에서 사용할 수 있습니다.

## 검색 조건자 추가 {#add-a-search-predicate}

검색 조건자를 다음에 추가하려면 **[!UICONTROL 필터]** 패널:

1. 관리 도구에 액세스하려면 맨 위의 도구 모음에서 Experience Manager 로고를 클릭합니다.

   ![](assets/aemlogo.png)

1. 관리 도구 패널에서 **[!UICONTROL Forms 검색]**.

   ![](assets/navigation-panel-1.png)

1. 다음에서 **[!UICONTROL Forms 검색]** 페이지, 선택 **[!UICONTROL 에셋 관리자 검색 레일]**.

   ![](assets/search-forms-page.png)

1. 맨 위에 표시되는 도구 모음에서 **[!UICONTROL 편집]** 검색 양식 편집을 엽니다.

   ![](assets/edit-search-form-1.png)

1. 다음에서 [!UICONTROL 검색 양식 편집] 페이지에서 술어를 끌어서 놓습니다. [!UICONTROL 조건자 선택] 탭으로 이동하여 기본 창을 표시합니다. 예: 드래그 **[!UICONTROL 속성 조건자]**.

   다음 **[!UICONTROL 속성]** 필드가 기본 창에 나타나고 **[!UICONTROL 설정]** 오른쪽의 탭에는 속성 술어가 표시됩니다.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >의 헤더 레이블 **[!UICONTROL 설정]** 탭은 선택한 술어 유형을 식별합니다.

1. 다음에서 **[!UICONTROL 설정]** 탭에서 속성 조건자에 대한 레이블, 자리 표시자 텍스트 및 설명을 입력합니다.

   * 선택 **[!UICONTROL 부분 검색]**&#x200B;지정된 속성 값을 기반으로 자산의 부분 구문 검색(및 와일드카드 검색)을 허용하려는 경우. 기본적으로 조건자는 전체 텍스트 검색을 지원합니다.
   * 선택 **[!UICONTROL 대소문자 무시]**, 속성 값을 기반으로 하는 에셋 검색이 대/소문자를 구분하지 않도록 하려는 경우. 기본적으로 검색 필터의 속성 값 검색은 대/소문자를 구분합니다.

   >[!NOTE]
   >
   >선택 시 **[!UICONTROL 부분 검색]** 확인란, **[!UICONTROL 대소문자 무시]** 기본적으로 가 선택되어 있습니다.

1. 다음에서 **[!UICONTROL 속성 이름]** 필드에서 속성 선택기를 열고 검색이 수행되는 기준 속성을 선택합니다. 또는 속성의 이름을 입력합니다. For example, enter `jcr :content/metadata/dc:title` or `./jcr:content/metadata/dc:title`.

   >[!NOTE]
   >
   >Brand Portal에서 모든 문자열 속성(다음으로 시작하는 속성 제외) `xmp`) `jcrcontent/metadata` / `dam:asset` 기본적으로 색인화됩니다.
   >
   >속성 술어를 만드는 동안 인덱싱된 모든 속성을 사용할 수 있습니다. 인덱싱되지 않은 속성이 구성된 경우 인덱싱되지 않은 속성에 대한 검색 쿼리가 검색 결과를 제공하지 않을 수 있습니다.

   ![](assets/title-prop.png)

1. 클릭 **[!UICONTROL 완료]** 설정을 저장합니다.
1. 다음에서 [!UICONTROL 에셋] 사용자 인터페이스에서 오버레이 아이콘을 클릭하고 **[!UICONTROL 필터]** 을 클릭하여 다음 위치로 이동합니다. **[!UICONTROL 필터]** 패널. The **[!UICONTROL Property]** predicate is added to the panel.

   ![](assets/property-filter-panel.png)

1. 검색할 자산의 제목을 입력합니다. **[!UICONTROL 속성]** 텍스트 상자입니다. 예: &quot;Adobe&quot;. 검색을 수행하면 제목이 &quot;Adobe&quot;와 일치하는 에셋이 검색 결과에 표시됩니다.

## 검색 조건자 목록 {#list-of-search-predicates}

를 추가하는 방식과 유사 **[!UICONTROL 속성]** 조건자에 다음 조건자를 추가할 수 있습니다 **[!UICONTROL 필터]** 패널:

| **술어 이름** | **설명** | **속성** |
|-------|-------|----------|
| **[!UICONTROL 경로 브라우저]** | 특정 위치에서 에셋을 검색하는 검색 조건자입니다. **참고:** *로그인한 사용자의 경우 필터의 경로 브라우저에 사용자와 공유된 폴더(및 상위 항목)의 콘텐츠 구조만 표시됩니다.* <br> 관리자 사용자는 경로 브라우저를 사용하여 해당 폴더로 이동하여 모든 폴더에서 에셋을 검색할 수 있습니다. <br> 반면 관리자가 아닌 사용자는 경로 브라우저에서 해당 폴더로 이동하여 폴더에서 에셋을 검색할 수 있습니다(액세스 가능). | <ul><li>필드 레이블</li><li>경로</li><li>설명</li></ul> |
| **[!UICONTROL 속성]** | 특정 메타데이터 속성을 기반으로 에셋을 검색합니다. **참고:** *부분 검색 선택 시 기본적으로 대/소문자 무시 가 선택됩니다*. | <ul><li>필드 레이블</li><li>자리 표시자</li><li>속성 이름</li><li>부분 검색</li><li>대소문자 구분 안 함</li><li> 설명</li></ul> |
| **[!UICONTROL 다중 값 속성]** | 속성 조건자와 유사하지만 구분 기호로 구분된 여러 입력 값을 허용합니다(기본값: COMMA).[,]) 입력 값 중 하나와 일치하는 에셋이 결과로 반환됩니다. | <ul><li>필드 레이블</li><li>자리 표시자</li><li>속성 이름</li><li>구분 기호 지원</li><li>대소문자 구분 안 함</li><li>설명</li></ul> |
| **[!UICONTROL 태그]** | 태그를 기반으로 에셋을 검색하는 검색 조건자입니다. 태그 목록의 다양한 태그를 채우도록 경로 속성을 구성할 수 있습니다. *참고: 예를 들어 관리자는 경로 값을 변경해야 할 수 있습니다. [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`], AEM에서 검색 양식을 게시하는 경우 여기서 경로에는 테넌트 정보가 포함되지 않습니다. 예: [!UICONTROL `/etc/tags/<custom_tag_namespace>`]. | <ul><li>필드 레이블</li><li>속성 이름</li><li>경로</li><li>설명</li></ul> |
| **[!UICONTROL 경로]** | 특정 위치에서 에셋을 검색하는 검색 조건자입니다. | <ul><li>필드 레이블</li><li>경로</li><li>설명</li></ul> |                                                     |
| **[!UICONTROL 상대적 날짜]** | 만든 상대적 날짜를 기준으로 자산을 검색하는 검색 조건자입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>상대적 날짜</li></ul> |
| **[!UICONTROL 범위]** | 지정된 속성 값 범위 내에 있는 에셋을 검색하는 검색 조건자입니다. [필터] 패널에서 범위에 대한 최소 및 최대 속성 값을 지정할 수 있습니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 날짜 범위]** | 날짜 속성에 대해 지정된 범위 내에 생성된 에셋을 검색하는 검색 조건자입니다. 필터 패널에서 시작 및 종료 날짜를 지정할 수 있습니다. | <ul><li>필드 레이블</li><li>자리 표시자</li><li>속성 이름</li><li>범위 텍스트(시작)</li><li>범위 텍스트(종료)</li><li>설명</li></ul> |
| **[!UICONTROL 날짜]** | 날짜 속성을 기반으로 하는 에셋의 슬라이더 기반 검색에 대한 검색 조건자입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 파일 크기]** | 크기 기준으로 에셋을 검색하는 검색 조건자입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>경로</li><li>설명</li></ul> |
| **[!UICONTROL 마지막으로 수정된 자산]** | 마지막으로 수정한 날짜를 기준으로 에셋을 검색하는 검색 조건자입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 승인 상태]** | 승인 메타데이터 속성을 기반으로 에셋을 검색하는 검색 조건자입니다. 기본 속성 이름은 입니다. **dam:status**. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 체크아웃 상태]** | AEM Assets에서 게시한 에셋의 체크아웃 상태를 기반으로 에셋을 검색하는 검색 조건자입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 체크아웃 기준]** | 에셋을 체크아웃한 사용자를 기준으로 에셋을 검색하는 검색 조건자입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 만료 상태]** | 만료 상태를 기반으로 에셋을 검색하는 검색 조건자입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 컬렉션 구성원]** | 자산이 컬렉션의 일부인지 여부를 기준으로 자산을 검색하는 검색 조건자입니다. | 설명 |
| **[!UICONTROL 숨김]** | 이 조건자는 최종 사용자에게 명시적으로 표시되지 않으며 일반적으로 검색 결과 유형을 제한하는 데 사용되는 숨겨진 제한에 사용됩니다. **dam:Asset**. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |

>[!NOTE]
>
>* 사용하지 않음 **[!UICONTROL 옵션 조건자]**, **[!UICONTROL 게시 상태 조건자]**, 및 **[!UICONTROL 등급 조건자]** 따라서 이 술어는 Brand Portal에서 작동하지 않습니다.
>* 폴더 유형 조건자 `(nt:folder type)` 는 Brand Portal에서 지원되지 않으며 성능 문제가 발생할 수 있습니다. 게시된 사용자 정의 검색 양식에 있는 경우 검색 양식을 편집하여 삭제할 수 있습니다.

## 검색 조건자 삭제 {#delete-a-search-predicate}

검색 조건자를 삭제하려면 다음 단계를 수행합니다.

1. 관리 도구에 액세스하려면 Adobe 로고를 클릭하십시오.

   ![](assets/aemlogo.png)

1. 관리 도구 패널에서 **[!UICONTROL Forms 검색]**.

   ![](assets/navigation-panel-2.png)

1. 다음에서 **[!UICONTROL Forms 검색]** 페이지, 선택 **[!UICONTROL 에셋 관리자 검색 레일]**.

   ![](assets/search-forms-page.png)

1. 맨 위에 표시되는 도구 모음에서 **[!UICONTROL 편집]** 검색 양식 편집을 엽니다.

   ![](assets/edit-search-form-2.png)

1. 다음에서 [!UICONTROL 검색 양식 편집] 메인 창에서 삭제할 술어를 선택합니다. 예를 들어 을 선택합니다. **[!UICONTROL 속성 조건자]**.

   다음 **[!UICONTROL 설정]** 오른쪽의 탭에는 속성 설명 필드가 표시됩니다.

1. 속성 설명을 삭제하려면 bin 아이콘을 클릭합니다. 다음에서 **[!UICONTROL 필드 삭제]** 대화 상자에서 **[!UICONTROL 삭제]** 삭제 작업을 확인합니다.

   다음 **[!UICONTROL 속성 조건자]** 필드가 기본 창에서 제거되고 **[!UICONTROL 설정]** 탭이 비어 있습니다.

   ![](assets/search-form-delete-predicate.png)

1. 변경 사항을 저장하려면 를 클릭합니다. **[!UICONTROL 완료]** 을 클릭합니다.
1. 다음에서 **[!UICONTROL 에셋]** 사용자 인터페이스에서 오버레이 아이콘을 클릭하고 **[!UICONTROL 필터]** 을 클릭하여 다음 위치로 이동합니다. **[!UICONTROL 필터]** 패널. 다음 **[!UICONTROL 속성]** 조건자가 패널에서 제거됩니다.

   ![](assets/property-predicate-removed.png)
