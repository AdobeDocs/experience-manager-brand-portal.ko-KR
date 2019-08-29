---
title: 브랜드 포털에 태그 게시
seo-title: 브랜드 포털에 태그 게시
description: AEM 자산에서 브랜드 포털에 태그를 게시하는 방법을 알아봅니다.
seo-description: AEM 자산에서 브랜드 포털에 태그를 게시하는 방법을 알아봅니다.
uuid: 4167367 E -1 AF 8-476 B -97 A 5-730 C 43 BD 0816
topic-tags: 게시
products: sg_ Experiencemanager/brand_ portal
content-type: 참조
discoiquuid: 3 C 8 E 9251-195 D -4 C 56-A 9 A 9-27 BC 8 B 2 A 82 A 4
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Publish tags to Brand Portal {#publish-tags-to-brand-portal}

자산에서 [!DNL AEM] 에 태그를 게시하는 방법을 알아봅니다 [!DNL Brand Portal].

태그는 자산을 구성하는 데 유용하며 자산이 연결된 자산의 검색 가능성을 향상시킵니다. 태그는 자산에 첨부된 키워드 또는 레이블 (메타데이터) 로 간주할 수 있으며 검색 결과로 자산을 빠르게 찾을 수 있습니다. [!DNL AEM] 자산에 있는 자산에 태그를 할당하는 방법을 알려면, 태그를 [사용하여 자산을 구성하는](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)방법을 참조하십시오.

태그 (자산 [!DNL AEM]및 컬렉션과 연관된 태그) 는 관련 태그가 있는 자산 (및 컬렉션) [!DNL Brand Portal] 이 게시될 때 자동으로 게시됩니다 [!DNL Brand Portal]. 게시된 태그는 검색을 활성화하여 연결된 자산을 찾는 데 유용합니다.

>[!NOTE]
>
>하지만 태그가 연결되어 있는 자산 (및 컬렉션) [!DNL Brand Portal] 를 게시하기 전에 전용으로 태그를 게시하도록 권장합니다. 자산 (및 컬렉션) 를 빠르게 게시할 [!DNL Brand Portal]수 있습니다.

## Manage tags {#manage-tags}

기존 태그를 사용하여 자산에 첨부하거나 [!DNL AEM] 태그 콘솔에서 새 태그를 만들 수 있습니다&#x200B;**(도구). | tagging |[!DNL AEM]태그**). 두 시나리오 모두에서 태그를 먼저 게시한 [!DNL Brand Portal] 다음 적절한 자산에 연결해야 합니다.

태그를 만들고 [!DNL AEM], 태그를 게시하고, 태그를 [!DNL Brand Portal]적절한 자산 (또는 컬렉션) 와 연결하려면 다음 단계를 수행합니다.

1. **Create tags**
sign in [!DNL AEM] author instance with administrative rights, and access **[!DNL AEM]tags** console from global navigation:

   1. 도구 **선택**

   2. **일반 선택**

   3. **태그 지정 선택**

2. **만들기를** 선택한 다음 태그 **만들기** 옵션을 선택합니다.
3. Specify:

   * **제목**
      *(필수)* 태그의 표시 제목입니다.
   * **이름**
      *(필수)* 태그의 이름입니다. 지정하지 않으면 제목에서 유효한 노드 이름이 만들어집니다. [Tagid를 참조하십시오](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID).
   * **설명**
      *(선택 사항)* 태그에 대한 설명입니다.
   * **태그 경로**
jcr 경로의 경로입니다.

4. **제출을** 선택하여 태그를 만듭니다.

   [!DNL AEM] 인스턴스에 태그를 만들었으면 태그를 자산에 첨부할 수 있습니다 (속성 섹션 사용 또는 해당 자산의 태그 관리 섹션 사용).

5. **태그를에 게시합니다[!DNL Brand Portal]**.

   **[!DNL AEM]태그** 콘솔로 이동 (도구) | tagging | [!DNL AEM] 태그) 에서 원하는 태그를 선택하고 게시를 **[!DNL Brand Portal]**&#x200B;선택합니다.

6. **태그를 자산 (또는 컬렉션)**&#x200B;에 첨부합니다.

   자산 (또는 컬렉션) 를 선택하고 해당 자산의 속성 섹션 또는 태그 관리 섹션을 사용하여 원하는 태그를 첨부합니다. 자산에 있는 자산에 태그를 할당하는 방법에 대한 자세한 [!DNL AEM] 내용은 Use Tags [to Organize Assets](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)를 참조하십시오.

7. **자산 (또는 컬렉션)[!DNL Brand Portal]**&#x200B;를에 게시\
   자산 (또는 컬렉션) 를에 게시하면 [!DNL Brand Portal]첨부된 태그도 사용할 수 [!DNL Brand Portal]있습니다.

   해당 자산 (또는 컬렉션) 에 첨부된 태그를 보려면 [!DNL Brand Portal]로그인하여 [!DNL Brand Portal] 자산을 선택하고 속성 섹션에서 첨부된 태그를 보게 됩니다.

## 검색 승격 {#search-promote}

[!DNL AEM] 자산을 사용하면 [!DNL Brand Portal] 키워드 태그를 기반으로 한 검색의 최상위 결과로 특정 자산을 만들 수 있습니다.

검색 키워드에 대한 자산을 높이려면 다음 단계를 수행하십시오.

1. 작성자 인스턴스에서 자산의 **속성** [!DNL AEM] 페이지를 엽니다.
2. **고급** 탭으로 이동합니다.
3. 검색 **키워드** **섹션에서 승급 검색** 섹션에서 **추가를** 선택하여 검색 키워드 또는 태그를 추가합니다.

   ![](assets/search-promote.png)

4. 변경 사항을 저장합니다.
5. 자산을에 게시합니다 [!DNL Brand Portal].
6. [!DNL Brand Portal]로그인합니다. **자산의** **속성** 섹션에서 고급 탭을 봅니다.
**검색 홍보** 키워드는 해당 자산의 속성에도 표시됩니다.
