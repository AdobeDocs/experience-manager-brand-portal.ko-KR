---
title: Publish 사전 설정, 스키마 및 Brand Portal 패싯
description: 사전 설정, 스키마 및 패싯을 Brand Portal에 게시하는 방법을 알아봅니다.
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
exl-id: 9b585606-6538-459b-87a9-2e68df0087b3
source-git-commit: 4d9d7afa2cd45ea68c2e15338c92aa29ecf09f91
workflow-type: tm+mt
source-wordcount: '1116'
ht-degree: 0%

---

# Publish 사전 설정, 스키마 및 Brand Portal 패싯 {#publish-presets-schema-and-facets-to-brand-portal}

이 문서에서는 AEM 작성자 인스턴스에서 Brand Portal으로 이미지 사전 설정, 메타데이터 스키마 및 사용자 지정 검색 패싯을 게시하는 방법에 대해 설명합니다. 게시 기능을 사용하면 AEM 작성자 인스턴스에서 만들거나 편집한 이미지 사전 설정, 메타데이터 스키마 및 검색 패싯을 재사용할 수 있습니다. 이 접근 방식은 중복 노력을 줄입니다.

>[!NOTE]
>
>AEM 작성자 인스턴스의 이미지 사전 설정, 메타데이터 스키마 및 검색 패싯을 Brand Portal에 게시하는 기능은 AEM 6.2 SP1-CFP7 및 AEM 6.3 SP 1-CFP 1(6.3.1.1) 이상에서 사용할 수 있습니다.

## Brand Portal에 대한 Publish 이미지 사전 설정 {#publish-image-presets-to-brand-portal}

이미지 사전 설정은 이미지 전달 시 이미지에 적용되는 크기 조정 및 서식 지정 명령 세트입니다. Brand Portal에서 이미지 사전 설정을 만들고 수정할 수 있습니다. 또는 AEM Author 인스턴스가 Dynamic Media 모드에서 실행 중인 경우 사용자가 AEM Author에서 사전 설정을 만들고 이를 AEM Assets Brand Portal에 게시할 수 있습니다. 이 방법을 사용하면 Brand Portal에서 동일한 사전 설정을 다시 생성하지 않습니다.
사전 설정이 만들어지면 에셋 세부 렌디션 레일 및 다운로드 대화 상자에 동적 렌디션으로 나열됩니다.

>[!NOTE]
>
>AEM 작성자 인스턴스가 **[!UICONTROL Dynamic Media 모드]**&#x200B;에서 실행되고 있지 않은 경우(고객이 Dynamic Media을 구매하지 않은 경우), 업로드할 때 자산의 **[!UICONTROL 피라미드 TIFF]** 렌디션이 만들어지지 않습니다. 이미지 사전 설정 또는 동적 변환은 자산의 **[!UICONTROL 피라미드 TIFF]**&#x200B;에서 작동합니다. 따라서 AEM 작성자 인스턴스에서 **[!UICONTROL 피라미드 TIFF]**&#x200B;을(를) 사용할 수 없는 경우 Brand Portal에서 사용할 수 없습니다. 따라서 에셋 세부 사항 페이지 및 다운로드 대화 상자의 렌디션 레일에 동적 렌디션이 없습니다.

Brand Portal에 이미지 사전 설정을 게시하려면 다음을 수행하십시오.

1. AEM 작성자 인스턴스에서 AEM 로고를 클릭하여 전역 탐색 콘솔에 액세스하고 도구 아이콘을 클릭한 다음 **[!UICONTROL Assets > 이미지 사전 설정]**(으)로 이동합니다.
1. 이미지 사전 설정 목록에서 이미지 사전 설정 또는 여러 이미지 사전 설정을 선택하고 **[!UICONTROL Publish to Brand Portal]**&#x200B;을(를) 클릭합니다.

![](assets/publishpreset.png)

>[!NOTE]
>
>사용자가 **[!UICONTROL Brand Portal으로 Publish]**&#x200B;를 클릭하면 이미지 사전 설정이 게시 큐에 있습니다. 사용자는 복제 에이전트의 로그를 모니터링하여 게시가 성공했는지 확인하는 것이 좋습니다.

Brand Portal에서 이미지 사전 설정 게시를 취소하려면 다음 작업을 수행하십시오.

1. AEM 작성자 인스턴스에서 AEM 로고를 클릭하여 전역 탐색 콘솔에 액세스하고 **[!UICONTROL 도구]** 아이콘을 클릭하고 **[!UICONTROL Assets > 이미지 사전 설정]**&#x200B;으로 이동합니다.
1. 이미지 사전 설정을 선택하고 맨 위에 있는 옵션에서 **[!UICONTROL Brand Portal에서 제거]**&#x200B;를 선택합니다.

## Brand Portal에 Publish 메타데이터 스키마 {#publish-metadata-schema-to-brand-portal}

메타데이터 스키마는 에셋/컬렉션의 속성 페이지에 표시되는 레이아웃 및 속성을 설명합니다.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

사용자가 AEM 작성자 인스턴스에서 기본 스키마를 편집하고 Brand Portal에서 기본 스키마와 동일한 스키마를 사용하려는 경우 메타데이터 스키마 양식을 Brand Portal에 게시합니다. 이러한 시나리오에서는 AEM 작성자 인스턴스에서 게시한 기본 스키마가 Brand Portal의 기본 스키마를 재정의합니다.

사용자가 AEM 작성자 인스턴스에서 사용자 정의 스키마를 만든 경우 동일한 사용자 정의 스키마를 다시 만드는 대신 Brand Portal에 사용자 정의 스키마를 게시할 수 있습니다. 그런 다음 사용자는 이 사용자 지정 스키마를 Brand Portal의 모든 폴더/컬렉션에 적용할 수 있습니다.

>[!NOTE]
>
>기본 스키마가 AEM 인스턴스에서 잠긴 경우 Brand Portal에 게시할 수 없습니다. 즉, 편집되지 않습니다.

![](assets/default-schema-form.png)

>[!NOTE]
>
>폴더에 AEM 작성자 인스턴스에 적용된 스키마가 있는 경우 Brand Portal에도 동일한 스키마가 있어야 합니다. 이렇게 하면 AEM Author 및 Brand Portal의 에셋 속성 페이지에서 일관성을 유지하는 데 도움이 됩니다.

AEM 작성자 인스턴스에서 Brand Portal으로 메타데이터 스키마를 게시하려면 다음을 수행합니다.

1. AEM 작성자 인스턴스에서 AEM 로고를 클릭하여 전역 탐색 콘솔에 액세스하고 도구 아이콘을 클릭하고 **[!UICONTROL Assets > 메타데이터 스키마]**&#x200B;로 이동합니다.
1. 메타데이터 스키마를 선택하고 맨 위에 있는 옵션에서 **[!UICONTROL Publish to Brand Portal]**&#x200B;을(를) 선택합니다.

>[!NOTE]
>
>사용자가 **[!UICONTROL Publish to Brand Portal]**&#x200B;을(를) 클릭하면 메타데이터 스키마가 게시 큐에 있습니다. 사용자는 복제 에이전트의 로그를 모니터링하여 게시가 성공했는지 확인하는 것이 좋습니다.

Brand Portal에서 메타데이터 스키마 게시를 취소하려면 다음 작업을 수행하십시오.

1. AEM 작성자 인스턴스에서 AEM 로고를 클릭하여 전역 탐색 콘솔에 액세스하고 도구 아이콘을 클릭하고 **[!UICONTROL Assets > 메타데이터 스키마]**&#x200B;로 이동합니다.
1. 메타데이터 스키마를 선택하고 맨 위에 있는 옵션에서 **[!UICONTROL Brand Portal에서 제거]**&#x200B;를 선택합니다.

## Brand Portal에 대한 Publish 검색 패싯 {#publish-search-facets-to-brand-portal}

검색 양식은 Brand Portal의 사용자에게 [패싯된 검색](../using/brand-portal-search-facets.md) 기능을 제공합니다. 검색 패싯은 Brand Portal 검색에 더 많은 세부기간을 부여합니다. 검색 양식에서 [추가된 술어](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/administer/search-facets)를 검색 필터에서 검색 패싯으로 사용할 수 있습니다.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

AEM 작성자 인스턴스의 **[!UICONTROL Assets 관리 검색 레일]**&#x200B;에서 사용자 정의 검색 양식을 사용하려면 다시 만드는 대신 Brand Portal에 직접 게시하십시오.

>[!NOTE]
>
>잠긴 검색 양식을 **[!UICONTROL Assets 관리자 검색 레일]**&#x200B;에 AEM Assets에서 Brand Portal으로 게시하려면 먼저 편집해야 합니다. 편집하고 게시하면 이 검색 양식은 Brand Portal의 기존 검색 양식을 재정의합니다.

편집된 검색 패싯을 AEM 작성자 인스턴스에서 Brand Portal에 게시하려면 다음을 수행하십시오.

1. AEM 로고를 클릭한 다음 **[!UICONTROL 도구 > 일반 > Forms 검색]**(으)로 이동합니다.
1. 편집한 검색 양식을 선택하고 **[!UICONTROL Publish to Brand Portal]**&#x200B;을(를) 선택합니다.

   >[!NOTE]
   >
   >사용자가 **[!UICONTROL Brand Portal으로 Publish]**&#x200B;를 클릭하면 검색 패싯이 게시 큐에 있습니다. 사용자는 복제 에이전트의 로그를 모니터링하여 게시가 성공했는지 확인하는 것이 좋습니다.

Brand Portal에서 검색 양식 게시를 취소하려면 다음 작업을 수행하십시오.

1. AEM 작성자 인스턴스에서 AEM 로고를 클릭하여 전역 탐색 콘솔에 액세스하고 도구 아이콘을 클릭한 다음 **[!UICONTROL 일반 > Forms 검색]**(으)로 이동합니다.
1. 검색 양식을 선택하고 맨 위에 있는 옵션에서 **[!UICONTROL Brand Portal에서 제거]**&#x200B;를 선택합니다.

>[!NOTE]
>
>**[!UICONTROL Brand Portal에서 게시 취소]** 작업은 Brand Portal에 기본 검색 양식을 남겨 두고 게시 전에 마지막으로 사용한 검색 양식으로 복원되지 않습니다.

### 제한 사항 {#limitations}

1. Brand Portal의 검색 필터에 적용할 수 있는 검색 조건자는 거의 없습니다. 이러한 검색 조건자가 AEM 작성자 인스턴스에서 Brand Portal으로 검색 양식의 일부로 게시되면 필터링됩니다. 따라서 Brand Portal에 게시된 양식에서 보다 적은 수의 술어를 볼 수 있습니다. [Brand Portal의 필터에 적용할 수 있는 검색 조건자](../using/brand-portal-search-facets.md#list-of-search-predicates)를 참조하십시오.

1. [!UICONTROL 옵션 설명]의 경우 사용자가 AEM 작성자 인스턴스에서 옵션을 읽는 데 사용자 지정 경로를 사용하는 경우 Brand Portal에서 작동하지 않습니다. 이러한 추가 경로 및 옵션은 검색 양식과 함께 Brand Portal에 게시되지 않습니다. 이 경우 사용자는 Brand Portal에서 **[!UICONTROL 옵션 조건자]** 내의 **[!UICONTROL 옵션 추가]**&#x200B;에서 **[!UICONTROL 수동]** 옵션을 선택하여 이러한 옵션을 수동으로 추가할 수 있습니다.

![](assets/options-predicate-manual.png)
