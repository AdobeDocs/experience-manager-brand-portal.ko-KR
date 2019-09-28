---
title: 브랜드 포털에 태그 게시
seo-title: 브랜드 포털에 태그 게시
description: Learn how to publish tags from AEM Assets to Brand Portal.
seo-description: Learn how to publish tags from AEM Assets to Brand Portal.
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: 게시
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: 참조
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d

---


# Publish tags to Brand Portal {#publish-tags-to-brand-portal}

Learn how to publish tags from AEM Assets to Brand Portal.

Tags are useful in organizing assets and enhance the searchability of assets to which they are associated. Tags can be thought of as keywords or labels (metadata) that are attached with assets, and allow assets to be quickly found as the result of a search. To know how to assign tags to assets in AEM Assets, refer use tags to organize assets.[](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)

Tags (associated with assets and collections in AEM) are auto-published to Brand Portal when the assets (and collections) with associated tags are published to Brand Portal. The published tags are helpful in enabling the searches to find the associated assets.

>[!NOTE]
>
>It is, however, recommended to exclusively publish tags to Brand Portal before publishing the assets (and collections) with which the tags are associated. This ensures faster publishing of the assets (and collections) to Brand Portal.

## Manage tags {#manage-tags}

기존 태그를 사용하여 자산에 첨부하거나 AEM 태그 콘솔에서 새 태그를 만들 수&#x200B;**[!UICONTROL 있습니다(도구| 태그 지정| AEM 태그]**). 두 시나리오 모두에서 먼저 태그를 브랜드 포털에 게시한 다음 적절한 자산에 연결해야 합니다.

AEM 파섹

1. **태그 만들기**&#x200B;관리 권한으로 AEM 작성자 인스턴스에 로그인하고 **[!UICONTROL 전역 탐색에서 AEM 태그]** 콘솔에 액세스합니다.

   1. 도구 **[!UICONTROL 선택]**

   1. 일반 **[!UICONTROL 선택]**

   1. 태그 지정 **[!UICONTROL 선택]**

1. 만들기를 **[!UICONTROL 선택한]** 다음 태그 **[!UICONTROL 만들기 옵션을]** 선택합니다.
1. 지정:

   * **[!UICONTROL 제목]**
      *(필수)* 태그의 표시 제목입니다.
   * **[!UICONTROL 이름]**
      *(필수* ) 태그의 이름입니다. 지정하지 않으면 제목에서 유효한 노드 이름이 생성됩니다. TagID [를 참조하십시오](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID).
   * **설명**
      *(선택 사항)* 태그에 대한 설명입니다.
   * **태그**&#x200B;경로의 JCR 경로입니다.

1. 제출을 **[!UICONTROL 선택하여]** 태그를 만듭니다.

   AEM 인스턴스에서 태그를 만들면 태그를 자산에 연결할 수 있습니다(해당 자산의 속성 섹션 또는 태그 관리 섹션 사용).

1. **Publish the tag to Brand Portal**.

   AEM **[!UICONTROL 태그]** 콘솔로 이동([!UICONTROL 도구| 태그 지정| AEM 태그])에서 원하는 태그를 선택하고 브랜드 포털에 게시를 선택합니다.

1. **태그를 자산(또는 컬렉션)에**&#x200B;첨부합니다.

   자산(또는 컬렉션)을 선택하고 해당 자산의 속성 섹션 또는 태그 관리 섹션을 사용하여 원하는 태그를 첨부합니다. AEM 자산에서 자산에 태그를 할당하는 방법에 대한 자세한 내용은 태그를 [사용하여 자산을](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)구성합니다.

1. **자산(또는 컬렉션)을 브랜드 포털에 게시합니다**.\
   자산(또는 컬렉션)을 브랜드 포털에 게시하면 첨부된 태그를 브랜드 포털에서도 사용할 수 있습니다.

   브랜드 포털의 각 자산(또는 컬렉션)에서 첨부된 태그를 보려면 브랜드 포털에 로그인하여 자산을 선택합니다. 속성 섹션에서 첨부된 태그가 표시됩니다.

## 검색 승격 {#search-promote}

AEM Assets 브랜드 포털을 사용하면 키워드 태그를 기반으로 한 검색에 대한 상위 결과로 특정 자산을 만들 수 있습니다.

검색 키워드에 대한 자산을 높이려면 다음 단계를 따르십시오.

1. AEM **[!UICONTROL 작성자]** 인스턴스에서 자산의 속성 페이지를 엽니다.
1. 고급 **[!UICONTROL 탭으로]** 이동합니다.
1. 검색 **[!UICONTROL 키워드]****[!UICONTROL 권한]** 향상 내의 검색 **[!UICONTROL 승격]** 섹션에서 추가를 선택하여검색 키워드 또는 태그를 추가합니다.

   ![](assets/search-promote.png)

1. 변경 사항을 저장합니다.
1. Brand Portal에 자산 게시.
1. 브랜드 포털에 로그인합니다. View Advanced tab in Properties section of the asset.
********
Note that the Search Promote keyword is also visible in the Properties of that asset.****
