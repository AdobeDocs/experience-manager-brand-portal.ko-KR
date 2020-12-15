---
title: 태그를 Brand Portal에 게시
seo-title: 태그를 Brand Portal에 게시
description: AEM Assets에서 브랜드 포털에 태그를 게시하는 방법에 대해 알아봅니다.
seo-description: AEM Assets에서 브랜드 포털에 태그를 게시하는 방법에 대해 알아봅니다.
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 4%

---


# 태그를 Brand Portal에 게시 {#publish-tags-to-brand-portal}

AEM Assets에서 브랜드 포털에 태그를 게시하는 방법에 대해 알아봅니다.

태그는 자산을 구성하고 연결된 에셋의 검색을 향상시키는 데 유용합니다. 태그는 자산에 첨부된 키워드 또는 레이블(메타데이터)으로 간주할 수 있으며 검색 결과 에셋을 신속하게 찾을 수 있습니다. AEM Assets에서 자산에 태그를 할당하는 방법에 대해 알려면 [태그를 사용하여 에셋 구성](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)을 참조하십시오.

관련 태그가 포함된 자산(및 컬렉션)이 브랜드 포털에 게시되면 AEM의 자산 및 컬렉션과 연관된 태그가 브랜드 포털에 자동으로 게시됩니다. 게시된 태그는 검색을 통해 관련 자산을 찾을 수 있도록 하는 데 유용합니다.

>[!NOTE]
>
>그러나 태그가 연결된 자산(및 컬렉션)을 게시하기 전에 브랜드 포털에 태그를 단독으로 게시하는 것이 좋습니다. 이렇게 하면 자산(및 컬렉션)을 브랜드 포털에 보다 빠르게 게시할 수 있습니다.

## 태그 관리 {#manage-tags}

기존 태그를 사용하여 자산에 첨부하거나 AEM 태그 콘솔에서 새 태그를 만들 수 있습니다(**[!UICONTROL 도구 | 태그 지정 | AEM 태그]**). 두 시나리오 모두에서 먼저 태그를 브랜드 포털에 게시한 다음 적절한 자산에 연결해야 합니다.

AEM에서 태그를 만들려면 브랜드 포털에서 태그를 게시하고 태그를 적절한 자산(또는 컬렉션)과 연결하려면 다음 단계를 수행하십시오.

1. **태그**
만들기관리 권한으로 AEM 작성자 인스턴스에 로그인하고 전역 탐색에서  **[!UICONTROL AEM]** 태그콘솔에 액세스합니다.

   1. **[!UICONTROL 도구]**&#x200B;를 선택합니다.

   1. **[!UICONTROL 일반]**&#x200B;을 선택합니다.

   1. **[!UICONTROL 태그 지정]**&#x200B;을 선택합니다.

1. **[!UICONTROL 만들기]**&#x200B;를 선택한 다음 **[!UICONTROL 태그 만들기]** 옵션을 선택합니다.
1. 지정:

   * **[!UICONTROL 제목]**

      *(필수)* 태그의 표시 제목입니다.
   * **[!UICONTROL 이름]**
      *(필수)* 태그의 이름입니다. 지정하지 않으면 Title에서 유효한 노드 이름이 만들어집니다. [TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID)를 참조하십시오.
   * **설명**

      *(선택 사항)* 태그에 대한 설명입니다.
   * **태그**
경로 태그의 JCR 경로입니다.

1. **[!UICONTROL 제출]**&#x200B;을 선택하여 태그를 만듭니다.

   AEM 인스턴스에서 태그를 만든 후에는 태그를 자산에 연결할 수 있습니다(해당 자산의 속성 섹션 또는 태그 관리 섹션 사용).

1. **태그를 브랜드 포털에 게시합니다**.

   **[!UICONTROL AEM 태그]** 콘솔([!UICONTROL 도구)로 이동 | 태그 지정 | AEM 태그])에서 원하는 태그를 선택하고 브랜드 포털에 게시를 선택합니다.

1. **태그를 자산(또는 컬렉션)에 첨부합니다**.

   자산(또는 컬렉션)을 선택하고 해당 자산의 속성 섹션 또는 태그 관리 섹션을 사용하여 원하는 태그를 첨부합니다. AEM Assets에서 자산에 태그를 할당하는 방법에 대한 자세한 내용은 [태그 사용을 사용하여 에셋](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)을(를) 구성합니다.

1. **자산(또는 컬렉션)을 브랜드 포털에 게시합니다**.\
   자산(또는 컬렉션)을 브랜드 포털에 게시하면 첨부된 태그를 브랜드 포털에서도 사용할 수 있습니다.

   브랜드 포털의 각 자산(또는 컬렉션)에서 첨부된 태그를 보려면 브랜드 포털에 로그인하고 해당 자산을 선택합니다. 속성 섹션에서 첨부된 태그가 표시됩니다.

## 검색 승격 {#search-promote}

AEM Assets 브랜드 포털에서는 키워드 태그를 기반으로 한 검색을 위한 상위 결과로 특정 자산을 만들 수 있습니다.

검색 키워드에 대한 자산을 높이려면 다음 단계를 수행합니다.

1. AEM 작성자 인스턴스에서 자산의 **[!UICONTROL 속성]** 페이지를 엽니다.
1. **[!UICONTROL 고급]** 탭으로 이동합니다.
1. **[!UICONTROL 검색 키워드]** 섹션 내 **[!UICONTROL 검색 홍보]**&#x200B;에서 **[!UICONTROL 추가]**&#x200B;를 선택하여 검색 키워드 또는 태그를 추가합니다.

   ![](assets/search-promote.png)

1. 변경 사항을 저장합니다.
1. Brand Portal에 자산 게시.
1. 브랜드 포털에 로그인합니다. 자산의 **[!UICONTROL 속성]** 섹션에서 **[!UICONTROL 고급]** 탭을 봅니다.
**[!UICONTROL 검색 승격]** 키워드는 해당 자산의 속성에도 표시됩니다.
