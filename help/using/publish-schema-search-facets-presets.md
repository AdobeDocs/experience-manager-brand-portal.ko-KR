---
title: 사전 설정, 스키마 및 패싯을 Brand Portal에 게시
seo-title: Publish presets, schema, and facets to Brand Portal
description: 사전 설정, 스키마 및 패싯을 Brand Portal에 게시하는 방법을 알아봅니다.
seo-description: Learn how to publish presets, schema, and facets to Brand Portal.
uuid: c836d9bb-074a-4113-9c91-b2bf7658b88d
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
exl-id: 9b585606-6538-459b-87a9-2e68df0087b3
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 2%

---

# 사전 설정, 스키마 및 패싯을 Brand Portal에 게시 {#publish-presets-schema-and-facets-to-brand-portal}

이 문서에서는 이미지 사전 설정, 메타데이터 스키마 및 사용자 지정 검색 패싯을 AEM 작성자 인스턴스에서 Brand Portal로 delves 합니다. 게시 기능을 사용하면 조직에서 이미지 사전 설정, 메타데이터 스키마 및 AEM 작성자 인스턴스에서 생성/수정된 검색 패싯을 재사용하여 중복 작업을 줄일 수 있습니다.

>[!NOTE]
>
>AEM 작성자 인스턴스의 이미지 사전 설정, 메타데이터 스키마 및 검색 패싯을 Brand Portal에 게시하는 기능은 AEM 6.2 SP1-CFP7 및 AEM 6.3 SP 1-CFP 1(6.3.1.1) 이상에서 사용할 수 있습니다.

## Brand Portal에 이미지 사전 설정 게시 {#publish-image-presets-to-brand-portal}

이미지 사전 설정은 이미지 전달 시 이미지에 적용되는 크기 조정 및 서식 지정 명령 세트입니다. Brand Portal에서 이미지 사전 설정을 만들고 수정할 수 있습니다. 또는 AEM 작성자 인스턴스가 다이내믹 미디어 모드에서 실행 중인 경우 사용자는 AEM 작성자에서 사전 설정을 만들고 AEM Assets Brand Portal에 게시할 수 있으며 Brand Portal에서 동일한 사전 설정을 다시 만들지 않아도 됩니다.\
사전 설정이 만들어지면 에셋 세부 렌디션 레일 및 다운로드 대화 상자에 동적 렌디션으로 나열됩니다.

>[!NOTE]
>
>AEM 작성자 인스턴스가 다이내믹 미디어 모드 ]**에서**[!UICONTROL  실행 되 고 있지 않은 경우 (고객이 다이내믹 미디어을 구입 하지 않은 경우) **[!UICONTROL 자산의 피라미드 TIFF]** 렌디션 업로드 시에는 만들어지지 않습니다. 이미지 사전 설정 또는 동적 변환은 자산의 피라미드 TIFF ]**에서**[!UICONTROL  작동 하므로 피라미드 tiff ]**를 AEM 작성자 인스턴스에서 사용할 수 없는 경우**[!UICONTROL  Brand Portal에도 사용할 수 없습니다. 이로 인해 자산 세부 사항 페이지 및 다운로드 대화 상자의 레일 변환에 동적 변환이 없습니다.

이미지 사전 설정을 Brand Portal 게시 하려면 다음을 수행 하십시오.

1. AEM 작성자 인스턴스에서 AEM 로고를 탭/클릭 하 여 글로벌 탐색 콘솔에 액세스 한 다음 도구 아이콘을 탭/클릭 하 고 Assets > 이미지 사전 설정 ]**이동**[!UICONTROL  합니다.
1. 이미지 사전 설정 목록에서 이미지 사전 설정 또는 여러 이미지 사전 설정을 선택하고 클릭/탭합니다 **[!UICONTROL Brand Portal에 게시]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>사용자가 Publish 클릭 **[!UICONTROL 하 여 Brand Portal]** 이미지 사전 설정이 게시용으로 큐에 추가 됩니다. 사용자는 복제 에이전트 로그를 모니터 하 여 게시 성공 했는지 확인 하는 것이 좋습니다.

Brand Portal에서 이미지 사전 설정을 게시 취소 하려면 다음을 수행 하십시오.

1. AEM 작성자 인스턴스에서 AEM 로고를 탭/클릭 하 여 글로벌 탐색 콘솔에 액세스 한 다음 도구 ]**아이콘을 탭/클릭**[!UICONTROL  하 고 Assets > 이미지 사전 설정 ]**이동**[!UICONTROL  합니다.
1. 이미지 사전 설정을 선택 하 고, 맨 위에서 사용 가능한 옵션 Brand Portal ]**에서 제거를 선택**[!UICONTROL  합니다.

## Brand Portal에 메타데이터 스키마 Publish  {#publish-metadata-schema-to-brand-portal}

메타데이터 스키마는 에셋/컬렉션의 속성 페이지에 표시되는 레이아웃 및 속성을 설명합니다.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

사용자가 AEM 작성자 인스턴스에서 기본 스키마를 편집하고 Brand Portal에서 기본 스키마와 동일한 스키마를 사용하려는 경우 메타데이터 스키마 양식을 Brand Portal에 게시하면 됩니다. 이러한 시나리오에서 Brand Portal의 기본 스키마는 AEM 작성자 인스턴스에서 게시한 기본 스키마로 인해 재정의됩니다.

사용자가 AEM 작성자 인스턴스에서 사용자 정의 스키마를 만든 경우 동일한 사용자 정의 스키마를 Brand Portal에서 다시 만드는 대신 사용자 정의 스키마를 AEM에 게시할 수 있습니다. 그런 다음 사용자는 이 사용자 지정 스키마를 Brand Portal의 모든 폴더/컬렉션에 적용할 수 있습니다.

>[!NOTE]
>
>기본 스키마는 AEM 인스턴스에서 잠긴 경우(편집되지 않은 경우) Brand Portal에 게시할 수 없습니다.

![](assets/default-schema-form.png)

>[!NOTE]
>
>폴더에 AEM 작성자 인스턴스에 적용 된 스키마가 있는 경우 자산 페이지 및 AEM에서 작성자 속성 Brand Portal 일관성을 유지 하기 위해 동일한 스키마도 Brand Portal에 있어야 합니다.

AEM 작성자 인스턴스에서 Brand Portal으로 메타데이터 스키마를 게시하려면 다음을 수행합니다.

1. AEM 작성자 인스턴스에서 AEM 로고를 탭/클릭하여 전역 탐색 콘솔에 액세스하고 도구 아이콘을 탭/클릭하여 다음 위치로 이동합니다. **[!UICONTROL 에셋 > 메타데이터 스키마]**.
1. 메타데이터 스키마를 선택하고 다음을 선택합니다. **[!UICONTROL Brand Portal에 게시]** 을 참조하십시오.

>[!NOTE]
>
>사용자가 **[!UICONTROL Brand Portal에 게시]**: 메타데이터 스키마는 게시 큐에 있습니다. 사용자는 복제 에이전트의 로그를 모니터링하여 게시가 성공했는지 확인하는 것이 좋습니다.

Brand Portal에서 메타데이터 스키마 게시를 취소하려면 다음 작업을 수행하십시오.

1. AEM 작성자 인스턴스에서 AEM 로고를 탭/클릭 하 여 글로벌 탐색 콘솔에 액세스 한 다음 도구 아이콘을 탭/클릭 하 고 Assets > 메타 데이터 스키마 ]**로**[!UICONTROL  이동 합니다.
1. 메타데이터 스키마를 선택 하 고, 맨 위에서 사용 가능한 옵션을 Brand Portal ]**에서 제거를 선택**[!UICONTROL  합니다.

## Brand Portal에 검색 패싯 게시 {#publish-search-facets-to-brand-portal}

검색 양식에서 제공하는 기능 [패싯된 검색](../using/brand-portal-search-facets.md) Brand Portal 사용자를 대상으로 합니다. 검색 패싯은 Brand Portal 검색에 더 많은 세부기간을 부여합니다. 모두 [술어 추가됨](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/search-facets.html) 검색 양식에서 사용자는 검색 필터에서 검색 패싯으로 사용할 수 있습니다.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

AEM 작성자 인스턴스에서 사용자 지정 검색 양식 **[!UICONTROL Assets 관리자 Search 레일]** 을 사용 하는 경우 Brand Portal에서 동일한 양식을 다시 만드는 대신 게시 검색 AEM에서 사용자 지정 된 작성자 양식을 인스턴스 수 있습니다.

>[!NOTE]
>
>잠긴 검색 양식 **[!UICONTROL Assets AEM Assets의 관리자 Search 레일]** 을 편집 하지 않으면 Brand Portal에 게시할 수 없습니다. Brand Portal에 편집 하 고 게시 하면이 검색 양식은 Brand Portal의 검색 양식을 무시 합니다.

편집한 검색 패싯을 AEM 작성자 인스턴스에서 Brand Portal 게시 하려면 다음을 수행 하십시오.

1. Tap/click the AEM logo, and then go to **[!UICONTROL Tools > General > Search Forms]**.
1. 편집한 검색 양식을 선택 하 고 Brand Portal ]**Publish를 선택**[!UICONTROL  합니다.

   >[!NOTE]
   >
   >사용자가 **[!UICONTROL Brand Portal에 게시]**, 검색 패싯은 게시 큐에 있습니다. 사용자는 복제 에이전트의 로그를 모니터링하여 게시가 성공했는지 확인하는 것이 좋습니다.

Brand Portal에서 검색 양식 게시를 취소하려면 다음 작업을 수행하십시오.

1. AEM 작성자 인스턴스에서 AEM 로고를 탭/클릭하여 전역 탐색 콘솔에 액세스하고 도구 아이콘을 탭/클릭하여 다음 위치로 이동합니다. **[!UICONTROL 일반 > Forms 검색]**.
1. 검색 양식을 선택하고 **[!UICONTROL Brand Portal에서 제거]** 을 참조하십시오.

>[!NOTE]
>
>Brand Portal ]**의 게시 취소는**[!UICONTROL  Brand Portal의 기본 검색 양식을 유지 하며 게시 하기 전에 사용 된 마지막 검색 양식으로 복원 하지 않습니다.

### 제한 사항 {#limitations}

1. Brand Portal에서 검색 필터에 적용할 수 없는 검색 조건자는 몇 가지가 있습니다. 이러한 검색 조건자가 검색 양식의 일부로 게시 되 면 AEM 작성자 인스턴스에서 Brand Portal으로 게시 됩니다. 따라서 사용자는 Brand Portal에서 게시 된 양식에 더 적은 수의 조건자를 표시 합니다. Brand Portal ](../using/brand-portal-search-facets.md#list-of-search-predicates) 의 필터에 적용할 수 있는 조건자 검색 참조 하십시오 [ .

1. 대상 [!UICONTROL 옵션 조건자], 사용자가 사용자 정의 경로를 사용하여 AEM 작성자 인스턴스에서 옵션을 읽는 경우 Brand Portal에서 작동하지 않습니다. 이러한 추가 경로 및 옵션은 검색 양식과 함께 Brand Portal에 게시되지 않습니다. 이 경우 사용자는 **[!UICONTROL 수동]** 의 옵션 **[!UICONTROL 옵션 추가]** 다음 범위 내 **[!UICONTROL 옵션 조건자]** Brand Portal에서 이러한 옵션을 수동으로 추가합니다.

![](assets/options-predicate-manual.png)
