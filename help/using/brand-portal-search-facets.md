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
source-git-commit: c5c16d2aa1b488efac90dbc77023bba9897ae929
workflow-type: tm+mt
source-wordcount: '1325'
ht-degree: 7%

---

# 사용자 정의 검색 패싯 사용 {#use-custom-search-facets}

관리자는 [!UICONTROL 필터] 패널에 검색 술어를 추가하여 검색을 사용자 정의하고 검색 기능을 다양하게 만들 수 있습니다.

Brand Portal은 승인된 브랜드 에셋의 세분화된 검색에 대해 [패싯된 검색](../using/brand-portal-searching.md#search-using-facets-in-filters-panel)을 지원합니다. 이는 [**필터** 패널](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) 때문에 가능합니다. 검색 패싯은 관리자 도구의 **[!UICONTROL 검색 양식]**&#x200B;을 통해 필터 패널에서 사용할 수 있습니다. 자산 관리자 검색 레일이라는 기본 검색 양식이 관리 도구의 Forms 검색 페이지에 있습니다. 그러나 관리자는 검색 술어를 추가, 수정 또는 제거하여 기본 검색 양식(에셋 관리자 검색 레일)을 편집하여 기본 필터 패널을 사용자 정의하여 검색 기능을 다용화할 수 있습니다.

다양한 검색 조건자를 사용하여 **[!UICONTROL 필터]** 패널을 사용자 지정할 수 있습니다. 예를 들어 속성 술어를 추가하여 이 술어에 지정하는 단일 속성과 일치하는 에셋을 검색합니다. 특정 속성에 대해 지정한 하나 이상의 값과 일치하는 에셋을 검색하려면 옵션 술어를 추가합니다. 지정된 날짜 범위 내에서 생성된 에셋을 검색하려면 날짜 범위 술어를 추가합니다.

>[!NOTE]
>
>Experience Manager Assets을 사용하면 조직에서 Brand Portal에서 동일한 양식을 다시 만드는 대신 [AEM 작성자](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal)의 사용자 지정된 검색 양식을 Brand Portal에 게시할 수 있습니다.

## 검색 조건자 추가 {#add-a-search-predicate}

**[!UICONTROL 필터]** 패널에 검색 조건자를 추가하려면:

1. 관리 도구에 액세스하려면 맨 위의 도구 모음에서 Experience Manager 로고를 클릭합니다.

   ![](assets/aemlogo.png)

1. 관리 도구 패널에서 **[!UICONTROL Forms 검색]**&#x200B;을 클릭합니다.

   ![](assets/navigation-panel-1.png)

1. **[!UICONTROL Forms 검색]** 페이지에서 **[!UICONTROL Assets 관리자 검색 레일]**&#x200B;을 선택합니다.

   ![](assets/search-forms-page.png)

1. 맨 위에 표시되는 도구 모음에서 **[!UICONTROL 편집]**&#x200B;을 클릭하여 검색 양식 편집을 엽니다.

   ![](assets/edit-search-form-1.png)

1. [!UICONTROL 검색 양식 편집] 페이지에서 [!UICONTROL 조건자 선택] 탭의 조건자를 기본 창으로 끕니다. 예를 들어 **[!UICONTROL 속성 조건자]**&#x200B;를 드래그합니다.

   **[!UICONTROL Property]** 필드가 기본 창에 나타나고 오른쪽의 **[!UICONTROL 설정]** 탭에 속성 술어가 표시됩니다.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >**[!UICONTROL 설정]** 탭의 머리글 레이블은 선택한 술어 유형을 식별합니다.

1. **[!UICONTROL 설정]** 탭에서 속성 조건자에 대한 레이블, 자리 표시자 텍스트 및 설명을 입력합니다.

   * 지정된 속성 값을 기반으로 자산의 부분 구문 검색(및 와일드카드 검색)을 허용하려면 **[!UICONTROL 부분 검색]**&#x200B;을 선택하십시오. 기본적으로 조건자는 전체 텍스트 검색을 지원합니다.
   * 속성 값을 기반으로 하는 자산 검색을 대/소문자를 구분하지 않게 하려면 **[!UICONTROL 대/소문자 무시]**&#x200B;를 선택합니다. 기본적으로 검색 필터의 속성 값 검색은 대/소문자를 구분합니다.

   >[!NOTE]
   >
   >**[!UICONTROL 부분 검색]** 확인란을 선택하면 기본적으로 **[!UICONTROL 대소문자 구분 안 함]**&#x200B;이 선택됩니다.

1. **[!UICONTROL 속성 이름]** 필드에서 속성 선택기를 열고 검색을 수행할 속성을 선택합니다. 또는 속성의 이름을 입력합니다. For example, enter `jcr :content/metadata/dc:title` or `./jcr:content/metadata/dc:title`.

   >[!NOTE]
   >
   >Brand Portal에서 `dam:asset`의 `jcrcontent/metadata`에 있는 모든 String 속성(`xmp`(으)로 시작하는 속성 제외)은 기본적으로 인덱싱됩니다. 모든 유형의 나머지 다른 모든 사용자 지정 속성은 기본적으로 인덱싱되지 않습니다.
   >
   >속성 술어를 만드는 동안 인덱싱된 모든 속성을 사용할 수 있습니다. 인덱싱되지 않은 속성이 구성된 경우 인덱싱되지 않은 속성에 대한 검색 쿼리가 검색 결과를 제공하지 않을 수 있습니다.

   ![](assets/title-prop.png)

1. 설정을 저장하려면 **[!UICONTROL 완료]**&#x200B;를 클릭하세요.
1. [!UICONTROL Assets] 사용자 인터페이스에서 오버레이 아이콘을 클릭하고 **[!UICONTROL 필터]**&#x200B;를 선택하여 **[!UICONTROL 필터]** 패널로 이동합니다. **[!UICONTROL 속성]** 조건자가 패널에 추가됩니다.

   ![](assets/property-filter-panel.png)

1. **[!UICONTROL 속성]** 텍스트 상자에 검색할 에셋의 제목을 입력합니다. 예: &quot;Adobe&quot;. 검색을 수행하면 제목이 &quot;Adobe&quot;와 일치하는 에셋이 검색 결과에 표시됩니다.

## 검색 조건자 목록 {#list-of-search-predicates}

**[!UICONTROL 속성]** 술어를 추가하는 방법과 유사하게 **[!UICONTROL 필터]** 패널에 다음 술어를 추가할 수 있습니다.

| **조건자 이름** | **설명** | **속성** |
|-------|-------|----------|
| **[!UICONTROL 경로 브라우저]** | 특정 위치에서 에셋을 검색하는 검색 조건자입니다. **참고:** *로그인한 사용자의 경우 필터의 경로 브라우저에 사용자와 공유된 폴더(및 상위 항목)의 콘텐츠 구조만 표시됩니다.* <br> 관리자 사용자는 경로 브라우저를 사용하여 해당 폴더로 이동하여 모든 폴더에서 에셋을 검색할 수 있습니다. <br> 반면 관리자가 아닌 사용자는 경로 브라우저에서 해당 폴더로 이동하여 폴더의 자산을 검색할 수 있습니다. | <ul><li>필드 레이블</li><li>경로</li><li>설명</li></ul> |
| **[!UICONTROL 속성]** | 특정 메타데이터 속성을 기반으로 에셋을 검색합니다. **참고:** *부분 검색을 선택하면 대소문자 구분이 기본적으로 선택됩니다*. | <ul><li>필드 레이블</li><li>플레이스홀더</li><li>속성 이름</li><li>부분 검색</li><li>대소문자 구분 안 함</li><li> 설명</li></ul> |
| **[!UICONTROL 다중 값 속성]** | 속성 조건자와 비슷하지만 구분 기호로 구분된 여러 개의 입력 값을 허용합니다(기본값은 COMMA[,]). 입력 값 중 하나와 일치하는 자산이 결과로 반환됩니다. | <ul><li>필드 레이블</li><li>플레이스홀더</li><li>속성 이름</li><li>구분 기호 지원</li><li>대소문자 구분 안 함</li><li>설명</li></ul> |
| **[!UICONTROL 태그]** | 태그를 기반으로 에셋을 검색하는 검색 조건자입니다. 태그 목록의 다양한 태그를 채우도록 경로 속성을 구성할 수 있습니다. *참고: 관리자가 AEM에서 검색 양식을 게시하는 경우 경로 값(예: [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`])을 변경해야 할 수 있습니다. 여기서 경로에는 테넌트 정보(예: [!UICONTROL `/etc/tags/<custom_tag_namespace>`])가 포함되지 않습니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>경로</li><li>설명</li></ul> |
| **[!UICONTROL 경로]** | 특정 위치에서 에셋을 검색하는 검색 조건자입니다. | <ul><li>필드 레이블</li><li>경로</li><li>설명</li></ul> |                                                     |
| **[!UICONTROL 상대적 날짜]** | 만든 상대적 날짜를 기준으로 자산을 검색하는 검색 조건자입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>상대적 날짜</li></ul> |
| **[!UICONTROL 범위]** | 지정된 속성 값 범위 내에 있는 에셋을 검색하는 검색 조건자입니다. [필터] 패널에서 범위에 대한 최소 및 최대 속성 값을 지정할 수 있습니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 날짜 범위]** | 날짜 속성에 대해 지정된 범위 내에 생성된 에셋을 검색하는 검색 조건자입니다. 필터 패널에서 시작 및 종료 날짜를 지정할 수 있습니다. | <ul><li>필드 레이블</li><li>플레이스홀더</li><li>속성 이름</li><li>범위 텍스트(시작)</li><li>범위 텍스트(종료)</li><li>설명</li></ul> |
| **[!UICONTROL 날짜]** | 날짜 속성을 기반으로 하는 에셋의 슬라이더 기반 검색에 대한 검색 조건자입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 파일 크기]** | 크기 기준으로 에셋을 검색하는 검색 조건자입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>경로</li><li>설명</li></ul> |
| **[!UICONTROL 마지막으로 수정한 자산]** | 마지막으로 수정한 날짜를 기준으로 에셋을 검색하는 검색 조건자입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 승인 상태]** | 승인 메타데이터 속성을 기반으로 에셋을 검색하는 검색 조건자입니다. 기본 속성 이름은 **dam:status**&#x200B;입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 체크아웃 상태]** | AEM Assets에서 게시한 에셋의 체크아웃 상태를 기반으로 에셋을 검색하는 검색 조건자입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 체크아웃한 사람]** | 에셋을 체크아웃한 사용자를 기준으로 에셋을 검색하는 검색 조건자입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 만료 상태]** | 만료 상태를 기반으로 에셋을 검색하는 검색 조건자입니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |
| **[!UICONTROL 컬렉션 구성원]** | 자산이 컬렉션의 일부인지 여부를 기준으로 자산을 검색하는 검색 조건자입니다. | 설명 |
| **[!UICONTROL 숨김]** | 이 조건자는 최종 사용자에게 명시적으로 표시되지 않으며 일반적으로 검색 결과 유형을 **dam:Asset**(으)로 제한하는 숨겨진 제한에 사용됩니다. | <ul><li>필드 레이블</li><li>속성 이름</li><li>설명</li></ul> |

>[!NOTE]
>
>* **[!UICONTROL 옵션 조건자]**, **[!UICONTROL Publish 상태 조건자]** 및 **[!UICONTROL 등급 조건자]**&#x200B;는 Brand Portal에서 작동하지 않으므로 사용하지 마십시오.
>* 폴더 유형 조건자 `(nt:folder type)`은(는) Brand Portal에서 지원되지 않으므로 성능 문제가 발생할 수 있습니다. 게시된 사용자 정의 검색 양식에 있는 경우 검색 양식을 편집하여 삭제할 수 있습니다.

## 검색 조건자 삭제 {#delete-a-search-predicate}

검색 조건자를 삭제하려면 다음 단계를 수행합니다.

1. 관리 도구에 액세스하려면 Adobe 로고를 클릭하십시오.

   ![](assets/aemlogo.png)

1. 관리 도구 패널에서 **[!UICONTROL Forms 검색]**&#x200B;을 클릭합니다.

   ![](assets/navigation-panel-2.png)

1. **[!UICONTROL Forms 검색]** 페이지에서 **[!UICONTROL Assets 관리자 검색 레일]**&#x200B;을 선택합니다.

   ![](assets/search-forms-page.png)

1. 맨 위에 표시되는 도구 모음에서 **[!UICONTROL 편집]**&#x200B;을 클릭하여 검색 양식 편집을 엽니다.

   ![](assets/edit-search-form-2.png)

1. [!UICONTROL 검색 양식 편집] 페이지의 기본 창에서 삭제할 술어를 선택합니다. 예를 들어 **[!UICONTROL 속성 조건자]**&#x200B;를 선택합니다.

   오른쪽의 **[!UICONTROL 설정]** 탭에는 속성 조건자 필드가 표시됩니다.

1. 속성 설명을 삭제하려면 bin 아이콘을 클릭합니다. **[!UICONTROL 필드 삭제]** 대화 상자에서 **[!UICONTROL 삭제]**&#x200B;를 클릭하여 삭제 작업을 확인합니다.

   **[!UICONTROL 속성 조건자]** 필드가 기본 창에서 제거되고 **[!UICONTROL 설정]** 탭이 비어 있습니다.

   ![](assets/search-form-delete-predicate.png)

1. 변경 내용을 저장하려면 도구 모음에서 **[!UICONTROL 완료]**&#x200B;를 클릭합니다.
1. **[!UICONTROL Assets]** 사용자 인터페이스에서 오버레이 아이콘을 클릭하고 **[!UICONTROL 필터]**&#x200B;를 선택하여 **[!UICONTROL 필터]** 패널로 이동합니다. **[!UICONTROL 속성]** 조건자가 패널에서 제거되었습니다.

   ![](assets/property-predicate-removed.png)
