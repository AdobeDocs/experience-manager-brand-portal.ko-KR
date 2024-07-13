---
title: Brand Portal에 Publish 태그 추가
seo-title: Publish tags to Brand Portal
description: Experience Manager Assets에서 Brand Portal으로 태그를 게시하는 방법에 대해 알아봅니다.
seo-description: Learn how to publish tags from Experience Manager Assets to Brand Portal.
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
exl-id: 842656a6-1a2b-4b64-954d-1e663923a1a1
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 2%

---

# Brand Portal에 Publish 태그 추가 {#publish-tags-to-brand-portal}

Experience Manager Assets에서 Brand Portal으로 태그를 게시하는 방법에 대해 알아봅니다.

태그는 자산을 구성하고 자산과 연결된 자산의 검색 가능성을 향상시키는 데 유용합니다. 태그는 자산과 함께 첨부된 키워드 또는 레이블(메타데이터)로 생각할 수 있으며 검색 결과 자산을 빠르게 찾을 수 있습니다. Experience Manager Assets의 자산에 태그를 할당하는 방법에 대해 알아보려면 [태그를 사용하여 자산 구성](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/organize-assets.html)을 참조하세요.

연결된 태그가 있는 자산(및 컬렉션)이 Brand Portal에 게시되면 태그(AEM의 자산 및 컬렉션과 연결됨)가 Brand Portal에 자동으로 게시됩니다. 게시된 태그는 검색을 활성화하여 관련 에셋을 찾는 데 유용합니다.

>[!NOTE]
>
>그러나 태그가 연결된 에셋(및 컬렉션)을 게시하기 전에 태그를 Brand Portal에 독점적으로 게시하는 것이 좋습니다. 이렇게 하면 에셋(및 컬렉션)을 Brand Portal에 보다 빠르게 게시할 수 있습니다.

## 태그 관리 {#manage-tags}

기존 태그를 사용하여 에셋에 첨부하거나 AEM 태그 콘솔에서 새 태그를 만들 수 있습니다(**[!UICONTROL 도구) | 태깅 | AEM 태그]**). 두 시나리오 모두에서 먼저 태그를 Brand Portal에 게시한 다음 적절한 자산과 연결해야 합니다.

AEM에서 태그를 만들고, Brand Portal에서 태그를 게시하고, 태그를 적절한 자산(또는 컬렉션)에 연결하려면 다음 단계를 수행하십시오.

1. **태그 만들기**
관리 권한을 사용하여 AEM 작성자 인스턴스에 로그인하고 전역 탐색에서 **[!UICONTROL AEM 태그]** 콘솔에 액세스합니다.

   1. **[!UICONTROL 도구]** 선택

   1. **[!UICONTROL 일반]** 선택

   1. **[!UICONTROL 태그 지정]** 선택

1. **[!UICONTROL 만들기]**&#x200B;를 선택한 다음 **[!UICONTROL 태그 만들기]** 옵션을 선택하십시오.
1. 지정:

   * **[!UICONTROL 제목]**
     *(필수)* 태그에 대한 표시 제목입니다.
   * **[!UICONTROL 이름]**
     *(필수)* 태그의 이름입니다. 지정하지 않으면 제목에서 올바른 노드 이름이 만들어집니다. [TagID](https://experienceleague.adobe.com/docs/experience-manager-65/developing/platform/tagging/framework.html)를 참조하십시오.
   * **설명**
     *(선택 사항)* 태그에 대한 설명입니다.
   * **태그 경로**
태그의 JCR 경로.

1. 태그를 만들려면 **[!UICONTROL 제출]**&#x200B;을 선택하십시오.

   AEM 인스턴스에 태그를 생성하면 해당 자산의 속성 섹션 또는 태그 관리 섹션 을 사용하여 자산에 태그를 첨부할 수 있습니다.

1. **Brand Portal에 태그를 Publish**.

   **[!UICONTROL AEM 태그]** 콘솔([!UICONTROL 도구)로 이동 | 태깅 | AEM 태그])에서 원하는 태그를 선택하고 Brand Portal으로 Publish을 이동합니다.

1. **자산(또는 컬렉션)에 태그를 첨부합니다**.

   에셋(또는 컬렉션)을 선택하고 해당 에셋의 속성 섹션 또는 태그 관리 섹션을 사용하여 원하는 태그를 첨부합니다. AEM Assets의 자산에 태그를 할당하는 방법에 대한 자세한 내용은 [태그를 사용하여 자산 구성](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/organize-assets.html)을 참조하세요.

1. **Publish 에셋(또는 컬렉션)을 Brand Portal**&#x200B;에 연결합니다.\
   에셋(또는 컬렉션)을 Brand Portal에 게시하면 첨부된 태그를 Brand Portal에서도 사용할 수 있습니다.

   Brand Portal의 각 에셋(또는 컬렉션)에서 첨부된 태그를 보려면 Brand Portal에 로그인하고 에셋을 선택하면 속성 섹션에 첨부된 태그가 표시됩니다.

## 검색 승격 {#search-promote}

AEM Assets Brand Portal을 사용하면 키워드 태그를 기반으로 특정 에셋을 검색 결과의 맨 위로 올리도록 할 수 있습니다.

검색 키워드에 대한 자산을 향상시키려면 다음 단계를 따르십시오.

1. AEM 작성자 인스턴스에서 자산의 **[!UICONTROL 속성]** 페이지를 엽니다.
1. **[!UICONTROL 고급]** 탭으로 이동합니다.
1. **[!UICONTROL 검색 키워드 개선]** 섹션 내의 **[!UICONTROL 검색 승격]**&#x200B;에서 **[!UICONTROL 추가]**&#x200B;를 선택하여 검색 키워드나 태그를 추가합니다.

   ![](assets/search-promote.png)

1. 변경 사항을 저장합니다.
1. Brand Portal에 자산을 Publish 합니다.
1. Brand Portal에 로그인. 자산의 **[!UICONTROL 속성]** 섹션에서 **[!UICONTROL 고급]** 탭을 봅니다.
**[!UICONTROL Search Promote]** 키워드도 해당 자산의 속성에 표시됩니다.
