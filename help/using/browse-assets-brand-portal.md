---
title: 브랜드 포털에서 자산 찾아보기
seo-title: 브랜드 포털에서 자산 찾아보기
description: 브랜드 포털에서 다양한 보기 옵션 및 UI 요소를 사용하여 자산 검색, 자산 계층 트래버스 및 자산 검색
seo-description: 브랜드 포털에서 다양한 보기 옵션 및 UI 요소를 사용하여 자산 검색, 자산 계층 트래버스 및 자산 검색
uuid: 178ce217-0050-4922-a204-f4539d46f539
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: introduction
discoiquuid: a70ce694-81d1-4829-9e61-b6412e013e5c
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# Browse assets on Brand Portal {#browsing-assets-on-brand-portal}

AEM Assets 브랜드 포털에서는 다양한 보기 옵션을 사용하는 동안 리소스 탐색, 자산 계층 탐색 및 자산 검색을 용이하게 하는 다양한 기능과 사용자 인터페이스 요소를 제공합니다.

맨 위의 AEM 도구 모음에 있는 AEM 로고는 관리 사용자가 관리 도구 패널에 액세스할 수 있도록 합니다.

![](assets/aemlogo.png)

![](assets/admin-tools-panel-2.png)

![](assets/bp_subheader.png)<br />

브랜드 포털의 왼쪽 상단에 있는 레일 선택기가 아래로 내려와서 자산 계층으로 이동하고, 검색을 간소화하고, 리소스를 표시할 수 있는 옵션을 제공합니다.

![](assets/siderail-1.png)

브랜드 포털의 오른쪽 상단에 있는 보기 선택기에서 사용 가능한 보기(카드, 열 및 목록)를 사용하여 자산을 보고, 탐색하고, 선택할 수 있습니다.

![](assets/viewselector.png)

## 리소스 보기 및 선택 {#viewing-and-selecting-resources}

보기, 탐색 및 선택은 모든 보기에서 개념적으로는 같지만 사용 중인 보기에 따라 처리 방식이 약간 다릅니다.

사용 가능한 보기 중 하나에서 리소스를 보고, 탐색하고(추가 작업을 위해) 선택할 수 있습니다.

* 열 보기 
* 카드 보기
* 목록 보기

### 카드 보기

![](assets/card-view.png)

카드 보기는 현재 수준에서 각 항목에 대한 정보 카드를 표시합니다. 이러한 카드에는 다음과 같은 세부 사항이 제공됩니다.

* 자산/폴더의 시각적 표현.
* 유형
* 제목
* 이름
* 자산이 AEM에서 브랜드 포털에 게시된 날짜 및 시간
* 크기
* 크기

You can navigate down the hierarchy by tapping/clicking cards (taking care to avoid the quick actions) or up again by using the [breadcrumbs in the header](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

![](assets/cardquickactions.png)

#### 관리자가 아닌 사용자를 위한 카드 보기

폴더 카드, 카드 보기에서 비관리 사용자(편집기, 뷰어 및 손님 사용자)에게 폴더 계층 정보를 표시합니다. 이 기능을 사용하면 상위 계층 구조와 관련하여 사용자가 액세스하는 폴더의 위치를 알 수 있습니다.
폴더 계층 정보는 다른 폴더 계층과 공유된 다른 폴더와 이름이 유사한 폴더를 구별하는 데 특히 유용합니다. 관리자가 아닌 사용자가 공유된 자산의 폴더 구조를 모를 경우 이름이 유사한 자산/폴더가 혼동되는 것처럼 보입니다.

* 각 카드에 표시되는 경로는 카드 크기에 맞게 잘립니다. 그러나 잘린 경로 위에 마우스를 놓으면 전체 경로를 도구 설명으로 볼 수 있습니다.

![](assets/folder-hierarchy1.png)

**자산 속성을 보는 개요 옵션**

개요 옵션은 관리자가 아닌 사용자(편집기, 뷰어, 손님 사용자)가 선택한 자산/폴더의 자산 속성을 볼 수 있습니다. 개요 옵션은 다음과 같이 표시됩니다.

* 을 클릭합니다.
* 레일 선택기를 선택하는 드롭다운에 있습니다.

자산/ **[!UICONTROL 폴더를]**선택한 동안 개요 옵션을 선택하면 제목, 경로 및 자산 생성 시간을 볼 수 있습니다. 반면에 자산 세부 사항 페이지에서 개요 옵션을 선택하면 사용자가 자산의 메타데이터를 볼 수 있습니다.

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### 카드 보기에서 설정 보기

**[!UICONTROL 뷰]**선택기에서 설정**[!UICONTROL &#x200B;보기를 선택하면 설정]** 보기 대화 상자가 열립니다. 카드 보기에서 자산 축소판의 크기를 조정할 수 있습니다. 이렇게 하면 보기를 개인화하고 표시되는 축소판 수를 제어할 수 있습니다.

![](assets/cardviewsettings.png)

### 목록 보기

![](assets/list-view.png)

목록 보기에는 현재 수준의 각 리소스에 대한 정보가 표시됩니다. 목록 보기에서는 다음 세부 사항을 제공합니다.

* 에셋의 축소판 이미지
* 이름
* 제목
* 로케일
* 유형
* 차원
* 크기
* 등급
* 자산 계층 구조를<sup>보여주는 폴더 경로*</sup>
* 브랜드 포털에 자산을 게시한 날짜

경로 열을 사용하면 폴더 계층 구조에서 자산 위치를 쉽게 식별할 수 있습니다. You can navigate down the hierarchy by tapping/clicking the resource name, and back up by using the [breadcrumbs in the header](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

<!--
Comment Type: draft lastmodifiedby="mgulati" lastmodifieddate="2018-08-17T03:12:05.096-0400" type="annotation">Removed:- "Selecting assets in list view To select all items in the list, use the checkbox at the upper left of the list. When all items in the list are selected, this check box appears checked. To deselect all, click or tap the checkbox. When only some items are selected, it appears with a minus sign. To select all, click or tap the checkbox. To deselect all, click or tap the checkbox again. You can change the order of items using the dotted vertical bar at the far right of each item in the list. Tap/click the vertical selection bar and drag the item to a new position in the list."
 -->

### 목록 보기에서 설정 보기

목록 보기에는 기본적으로 **[!UICONTROL 자산]**이름이 첫 번째 열로 표시됩니다. 자산 제목**[!UICONTROL ,]**로케일 **[!UICONTROL ,]**로케일**[!UICONTROL &#x200B;유형]**, **[!UICONTROL 차원]**, 크기, 크기,********크기, 등급, 게시 상태와 같은 추가 정보가 표시됩니다. However, you can select the columns to be shown using**[!UICONTROL  View Settings]**.

![](assets/list-view-setting.png)

### 열 보기 

![](assets/column-view.png)

열 보기를 사용하여 일련의 계단식 열을 통해 컨텐츠 트리를 탐색합니다. 이 보기는 자산 계층을 시각화하고 트래버스하는 데 도움이 됩니다.

첫 번째(맨 왼쪽) 열에서 리소스를 선택하면 오른쪽의 두 번째 열에 하위 리소스가 표시됩니다. 두 번째 열에서 리소스를 선택하면 오른쪽의 세 번째 열에 하위 리소스가 표시됩니다.

리소스 이름 또는 리소스 이름 오른쪽에 있는 V자형을 탭하거나 클릭하여 트리에서 위아래로 탐색할 수 있습니다.

* 탭하거나 클릭하면 리소스 이름과 V자형이 강조 표시됩니다.
* 축소판을 탭하거나 클릭하면 리소스가 선택됩니다.
* 이 옵션을 선택하면 축소판에 확인 표시가 겹쳐 표시되고 리소스 이름이 강조 표시됩니다.
* 선택한 리소스의 세부 정보가 마지막 열에 표시됩니다.

열 보기에서 자산을 선택하면 자산의 시각적 표현이 다음 세부 정보와 함께 마지막 열에 표시됩니다.

* 제목
* 이름
* 크기
* 자산이 AEM에서 브랜드 포털에 게시된 날짜 및 시간
* 크기
* 유형
* 자세한 정보 옵션 - 자산의 세부 정보 페이지로 이동합니다.

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

<h4>Deselecting All</h4>
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

## 컨텐츠 트리 {#content-tree}

이러한 보기 외에도 트리 보기를 사용하여 원하는 자산 또는 폴더를 보고 선택하는 동안 자산 계층 구조를 드릴다운합니다.

트리 보기를 열려면 왼쪽 상단에 있는 레일 선택기를 탭/클릭하고 메뉴에서 **[!UICONTROL 컨텐츠 트리를]**선택합니다.

![](assets/contenttree.png)

컨텐츠 계층에서 원하는 자산으로 이동합니다.

![](assets/content-tree.png)

## 자산 세부 정보 {#asset-details}

자산 세부 사항 페이지에서는 자산을 보거나, 다운로드하고, 자산의 링크를 공유하거나, 컬렉션으로 이동하거나, 자산 페이지를 볼 수 있습니다. 또한 동일한 폴더의 다른 자산의 세부 정보 페이지를 연속해서 탐색할 수 있습니다.

![](assets/asset-detail.png)

자산의 메타데이터를 보거나 다양한 표현물을 보려면 자산 세부 사항 페이지에서 레일 선택기를 사용합니다.

![](assets/asset-overview.png)

자산 세부 사항 페이지에서 자산의 사용 가능한 모든 변환을 보고 미리 볼 변환을 선택할 수 있습니다.

![](assets/renditions.png)

자산 속성 페이지를 열려면 상단 **[!UICONTROL 막대에서 속성(p)]**옵션을 사용합니다.

![](assets/asset-properties.png)

자산 관계는 AEM에서 브랜드 포털까지 게시되므로 자산의 속성 페이지에서 모든 관련 자산(소스 또는 AEM의 파생 자산)의 목록을 볼 수도 있습니다.
