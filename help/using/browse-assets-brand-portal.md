---
title: Brand Portal에서 에셋 찾아보기
seo-title: Browse assets on Brand Portal
description: Brand Portal에서 다양한 보기 옵션과 UI 요소를 사용하여 에셋을 탐색하고, 에셋 계층을 탐색하고, 에셋을 검색할 수 있습니다.
seo-description: Browse through assets, traverse asset hierarchies, and search assets, using different view options and UI elements on Brand Portal.
uuid: 178ce217-0050-4922-a204-f4539d46f539
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: introduction
discoiquuid: a70ce694-81d1-4829-9e61-b6412e013e5c
exl-id: 405d7861-a140-44b1-ae1f-4f0839f05033
source-git-commit: 133ea1fc342e4460e7d0661205c7411a509143eb
workflow-type: tm+mt
source-wordcount: '1005'
ht-degree: 7%

---

# Brand Portal에서 에셋 찾아보기 {#browsing-assets-on-brand-portal}

Experience Manager Assets Brand Portal은 다양한 보기 옵션을 사용하면서 리소스 탐색, 에셋 계층 탐색 및 에셋 검색을 용이하게 하는 다양한 기능과 사용자 인터페이스 요소를 제공합니다.

맨 위에 있는 도구 모음에 있는 Experience Manager 로고를 사용하면 관리 사용자가 관리 도구 패널에 액세스할 수 있습니다.

![](assets/aemlogo.png)

![](assets/admin-tools-panel-2.png)

![](assets/bp_subheader.png)

Brand Portal의 왼쪽 상단에 있는 레일 선택기를 통해 자산 계층으로 이동하고, 검색을 간소화하고, 리소스를 표시할 수 있는 옵션을 표시할 수 있습니다.

![](assets/siderail-1.png)

Brand Portal의 오른쪽 상단에 있는 보기 선택기에서 사용 가능한 보기 (카드, 열 및 목록)를 사용하여 에셋을 보고, 탐색하고, 선택할 수 있습니다.

![](assets/viewselector.png)

## 리소스 보기 및 선택 {#viewing-and-selecting-resources}

각 보기, 탐색 및 선택은 모든 보기에서 개념적으로 동일하지만 사용하는 보기에 따라 처리 방식이 약간 다릅니다.

사용 가능한 보기 중에서 리소스를 보고, 탐색하고, (추가 작업을 위해) 선택할 수 있습니다.

* 열 보기
* 카드 보기
* 목록 보기

### 카드 보기

![](assets/card-view.png)

카드 보기는 현재 수준에서 각 항목에 대한 정보 카드를 표시합니다. 이 카드는 다음 세부 정보를 제공합니다.

* 자산/폴더를 시각적으로 표현한 것입니다.
* 유형
* 제목
* 이름
* AEM에서 Brand Portal에 자산이 게시된 날짜 및 시간
* 크기
* 치수

카드를 탭하거나 클릭하여 계층 구조를 아래로 이동하거나(빠른 작업이 발생하지 않도록 주의) 헤더에서 [탐색 표시를 사용하여](https://experienceleague.adobe.com/docs/experience-manager-65/authoring/essentials/basic-handling.html) 다시 위로 이동할 수 있습니다.

![](assets/cardquickactions.png)

#### 관리자가 아닌 사용자의 카드 보기

폴더 카드는 카드 보기에서 관리자가 아닌 사용자(편집자, 뷰어 및 게스트 사용자)에게 폴더 계층 구조 정보를 표시합니다. 이 기능을 사용하면 상위 계층 구조를 기준으로 사용자가 액세스하는 폴더의 위치를 알 수 있습니다.
폴더 계층 정보는 다른 폴더 계층 구조에서 공유된 다른 폴더와 유사한 이름을 갖는 폴더를 구별하는 데 특히 유용합니다. 관리자가 아닌 사용자가 공유된 에셋의 폴더 구조를 알지 못하는 경우 유사한 이름의 에셋/폴더가 혼동되는 것으로 보입니다.

* 각 카드에 표시된 경로는 카드 크기에 맞게 잘립니다. 그러나 전체 경로는 잘린 경로 위로 마우스를 가져갈 때 도구 설명으로 볼 수 있습니다.

![](assets/folder-hierarchy1.png)

**자산 속성을 보는 개요 옵션**

개요 옵션은 관리자가 아닌 사용자(편집자, 뷰어, 게스트 사용자)가 선택한 에셋/폴더의 에셋 속성을 볼 수 있습니다. 개요 옵션이 표시됩니다.

* 에셋/폴더 선택 시 맨 위의 도구 모음에서 를 클릭합니다.
* 을 클릭하여 레일 선택기를 선택합니다.

에셋/폴더를 선택한 상태에서 **[!UICONTROL 개요]** 옵션을 선택하면 에셋 생성의 제목, 경로 및 시간이 표시됩니다. 반면 에셋 세부 정보 페이지에서 개요 옵션을 선택하면 에셋의 메타데이터를 볼 수 있습니다.

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### 카드 보기에서 설정 보기

보기 선택기에서 **[!UICONTROL 보기 설정]**&#x200B;을 선택하면 **[!UICONTROL 보기 설정]** 대화 상자가 열립니다. 카드 보기에서 에셋 썸네일의 크기를 조정할 수 있습니다. 이렇게 하면 보기를 개인화하고 표시되는 썸네일 수를 제어할 수 있습니다.

![](assets/cardviewsettings.png)

### 목록 보기

![](assets/list-view.png)

목록 보기에는 현재 수준의 각 리소스에 대한 정보가 표시됩니다. 목록 보기는 다음 세부 정보를 제공합니다.

* 에셋의 썸네일 이미지
* 이름
* 제목
* 로케일
* 유형
* 차원
* 크기
* 등급
* 자산 계층 구조를 보여 주는 폴더 경로
* Brand Portal에 자산을 게시한 날짜

경로 열을 사용하면 폴더 계층 구조에서 자산 위치를 쉽게 식별할 수 있습니다. 리소스 이름을 탭/클릭하여 계층 구조를 탐색하고 헤더에서 [탐색 표시를 사용하여 ](https://experienceleague.adobe.com/docs/experience-manager-65/authoring/essentials/basic-handling.html)백업할 수 있습니다.

<!--
Comment Type: draft lastmodifiedby="mgulati" lastmodifieddate="2018-08-17T03:12:05.096-0400" type="annotation">Removed:- "Selecting assets in list view To select all items in the list, use the checkbox at the upper left of the list. When all items in the list are selected, this check box appears checked. To deselect all, click or tap the checkbox. When only some items are selected, it appears with a minus sign. To select all, click or tap the checkbox. To deselect all, click or tap the checkbox again. You can change the order of items using the dotted vertical bar at the far right of each item in the list. Click the vertical selection bar and drag the item to a new position in the list."
 -->

### 목록 보기에서 설정 보기

목록 보기에는 기본적으로 자산 **[!UICONTROL Name]**&#x200B;이(가) 첫 번째 열로 표시됩니다. 자산 **[!UICONTROL 제목]**, **[!UICONTROL 로케일]**, **[!UICONTROL 유형]**, **[!UICONTROL Dimension]**, **[!UICONTROL 크기]**, **[!UICONTROL 등급]**, 게시 상태 등의 추가 정보도 표시됩니다. 그러나 **[!UICONTROL 설정 보기]**&#x200B;를 사용하여 표시할 열을 선택할 수 있습니다.

![](assets/list-view-setting.png)

### 열 보기

![](assets/column-view.png)

열 보기를 사용하여 일련의 계단식 열을 통해 콘텐츠 트리를 탐색합니다. 이 뷰는 자산 계층 구조를 시각화하고 탐색하는 데 도움이 됩니다.

첫 번째(가장 왼쪽) 열에서 리소스를 선택하면 오른쪽에 있는 두 번째 열에 하위 리소스가 표시됩니다. 두 번째 열에서 리소스를 선택하면 오른쪽의 세 번째 열에 하위 리소스가 표시됩니다.

리소스 이름 또는 리소스 이름 오른쪽에 있는 V자형 화살표를 탭하거나 클릭하여 트리에서 위아래로 탐색할 수 있습니다.

* 탭하거나 클릭하면 리소스 이름과 V자형 화살표가 강조 표시됩니다.
* 썸네일을 탭하거나 클릭하면 리소스가 선택됩니다.
* 선택하면 확인 표시가 썸네일에 오버레이되고 리소스 이름이 강조 표시됩니다.
* 선택한 리소스의 세부 정보가 마지막 열에 표시됩니다.

열 보기에서 에셋을 선택하면 에셋의 시각적 표현이 다음 세부 정보와 함께 최종 열에 표시됩니다.

* 제목
* 이름
* 치수
* AEM에서 Brand Portal에 자산이 게시된 날짜 및 시간
* 크기
* 유형
* 추가 세부 정보 옵션을 사용하여 자산의 세부 정보 페이지로 이동합니다.

<!--
Comment Type: draft

<h3>Selecting Resources</h3>
-->

<!--
Comment Type: draft

<p>Selecting a specific resource depends on a combination of the view and the device:</p>
-->

<!--
Comment Type: draft

<table border="1" cellpadding="1" cellspacing="0" width="100%">
<tbody>
<tr>
<td> </td>
<td>Select</td>
<td>Deselect</td>
</tr>
<tr>
<td>Column View<br /> </td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the thumbnail</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
</tr>
<tr>
<td>Card View<br /> </td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap-and-hold the card</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the card</li>
<li>Mobile device:<br /> Tap the card</li>
</ul> </td>
</tr>
<tr>
<td>List View</td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the thumbnail</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
</tr>
</tbody>
</table>
-->

<!--
Comment Type: draft

Deselecting All
-->

<!--
Comment Type: draft

<p>In all cases, as you select items the count of the items selected is displayed at the upper right of the toolbar.</p>
<p>You can deselect all items and exit selection mode by clicking or tapping the X next to the count.</p>
-->

<!--
Comment Type: draft

<p>In all views, all items can be deselected by tapping escape on the keyboard if you are using a desktop device.</p>
-->

## 콘텐츠 트리 {#content-tree}

이러한 보기 외에 트리 보기를 사용하여 원하는 에셋 또는 폴더를 보고 선택하는 동안 에셋 계층을 드릴다운할 수 있습니다.

트리 보기를 열려면 왼쪽 상단의 레일 선택기를 클릭하고 메뉴에서 **[!UICONTROL 콘텐츠 트리]**&#x200B;를 선택합니다.

![](assets/contenttree.png)

콘텐츠 계층에서 원하는 에셋으로 이동합니다.

![](assets/content-tree.png)

## 자산 세부 정보 {#asset-details}

에셋 세부 사항 페이지에서는 에셋을 보거나, 다운로드하거나, 에셋의 링크를 공유하거나, 컬렉션으로 이동하거나, 해당 속성 페이지를 볼 수 있습니다. 또한 동일한 폴더의 다른 에셋에 대한 세부 정보 페이지를 연속적으로 탐색할 수 있습니다.

![](assets/asset-detail.png)

에셋의 메타데이터를 보거나 에셋의 다양한 렌디션을 보려면 에셋 세부 사항 페이지의 레일 선택기를 사용하십시오.

![](assets/asset-overview.png)

에셋 세부 정보 페이지에서 에셋에 대해 사용 가능한 모든 렌디션을 보고 **[!UICONTROL 렌디션]** 패널에서 렌디션을 선택하여 미리 볼 수 있습니다.

![](assets/renditions.png)

<!-- removed as it is fixed in 2022.02.0 release
>[!CAUTION]
>
>(**Experience Manager Assets as a Cloud Service** only) The following known issues will be fixed in the upcoming release:
>
>The **[!UICONTROL Renditions]** panel does not list all the static renditions of the assets that are published to Brand Portal after December 16, 2021.
>
>The **[!UICONTROL Renditions]** panel lists the smart crop renditions of the asset, however, the user cannot preview or download the smart crop renditions.
-->

자산 속성 페이지를 열려면 상단 표시줄의 **[!UICONTROL 속성(p)]** 옵션을 사용하십시오.

![](assets/asset-properties.png)

에셋 관계가 AEM에서 Brand Portal으로 게시되므로 에셋의 속성 페이지에서 모든 관련 에셋(AEM의 소스 또는 파생된 에셋) 목록을 볼 수도 있습니다.
