---
title: 릴리스 노트
seo-title: 릴리스 노트
description: Adobe Experience Manager Assets Brand Portal 2021.02.0 릴리스의 기능, 개선 사항, 해결된 주요 문제 및 알려진 문제에 대한 통찰력을 얻을 수 있습니다.
seo-description: Adobe Experience Manager Assets Brand Portal 2021.02.0 릴리스의 개선 사항, 해결된 주요 문제 및 알려진 문제에 대한 통찰력을 얻을 수 있습니다.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: d2bfd06f8cd8a9e78efbc8dd92880e0faae39176
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 9%

---

# 릴리스 노트 {#release-notes}

Adobe Experience Manager Assets Brand Portal 2021.02.0 릴리스의 새로운 기능, 개선 사항, 해결된 주요 문제 및 알려진 문제에 대한 통찰력을 얻을 수 있습니다.

## 릴리스 정보 {#release-information}

| 제품 | Adobe Experience Manager Assets Brand Portal |
|---|---|
| 버전 | 2021.02.0 |
| 날짜 | 2021년 2월 |

## 개요 {#overview}

Adobe Experience Manager(AEM) Assets Brand Portal을 사용하면 승인된 크리에이티브 자산을 외부 당사자 및 내부 비즈니스 사용자가 간편하게 구매하고 제어하며 장치 간에 안전하게 분배할 수 있습니다. 자산 공유의 효율성을 향상시키고, 자산 출시 시간을 단축하며, 규정 준수 및 무단 액세스의 위험을 줄일 수 있습니다. Brand Portal을 사용하면 자산을 언제 어디서나 기업 승인 형식으로 검색, 미리 보기, 다운로드 및 내보낼 수 있습니다.

## 2021.02.0의 새로운 기능 {#whats-new-in-2021.02.0}

### 새 기능 {#new-features}

이 릴리스에는 다음과 같은 새로운 기능이 포함되어 있습니다.

* 이제 Cloud Service으로 AEM Assets에 사전 구성된 Brand Portal 인스턴스가 있을 수 있습니다. Cloud Manager 사용자는 AEM Assets에서 Brand Portal을 Cloud Service 인스턴스로 활성화할 수 있습니다.

* 이제 AEM Assets에서 Cloud Service으로 자산 소싱 기능을 사용할 수 있습니다. 이를 통해 Brand Portal 사용자는 허용된 기여도 폴더에 자산을 업로드하고 Brand Portal의 기여도 폴더를 Cloud Service 인스턴스로 AEM Assets에 게시할 수 있습니다.

* 추가 **[!UICONTROL 자산 다운로드]** 설정이 **[!UICONTROL 다운로드 설정]**&#x200B;에 도입되었습니다. 폴더, 컬렉션 또는 자산의 벌크 다운로드를 다운로드하는 동안 각 자산에 대해 별도의 폴더를 만듭니다.

<!-- 
* The **[!UICONTROL Download]** dialog is revamped in a list view with additional options to exclude the renditions which are not required, apply the same set of rules for similar asset types, and download the selected asset renditions. See [steps to download assets from Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets).
-->

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

<!-- 
* Navigation to the **[!UICONTROL Files]**, **[!UICONTROL Collections]**, and **[!UICONTROL Shared Links]** is now possible from all the Brand Portal pages in one-click.  

* The **[!UICONTROL Renditions]** panel in the asset details page now allows the Brand Portal users to select the original asset and (or) specific asset renditions, and directly download them from the **[!UICONTROL Renditions]** panel without having to open the **[!UICONTROL Download]** dialog. See [download assets from asset details page](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets-from-asset-details-page).
-->

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

<!-- 
* In addition to the existing **[!UICONTROL Download]** configurations, the Brand Portal administrators can also [configure permissions for different group of users](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions) to view and (or) download the original asset and its renditions from the asset details page. These configurations will define who can access and (or) download the asset renditions.
-->

### 향상된 기능 {#enhancements}

이 릴리스에는 다음 개선 사항이 포함됩니다.

* 폴더 다운로드의 경우, 공유 링크를 사용하여 **[!UICONTROL 다운로드 설정]**&#x200B;에 관계없이 각 자산에 대해 별도의 폴더가 만들어집니다.
* Brand Portal **[!UICONTROL 사용 보고서]**&#x200B;가 활성 Brand Portal 사용자만 반영하도록 수정되었습니다.

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### 해결된 중요한 문제 {#critical-issues-fixed}

이 릴리스에는 다음과 같은 중요한 문제에 대한 수정 사항이 포함되어 있습니다.

* 원래 자산만 다운로드되는 경우, 자산은 자체 확장을 반영하며, 확장이 수동으로 zip으로 변경될 때까지 열리지 않습니다.
* 탐색 화살표를 클릭하면 컬렉션 폴더의 사용자 인터페이스가 응답하지 않습니다.
* **** 폴더가 비어  **** 있어도 [열] 보기에 만들기 단추가 표시됩니다.
* **[!UICONTROL Brand Portal]** 인스턴스에 액세스하는 동안 디스패처가 우회되는 경우 옴니 검색이 414 오류 메시지(Request-URI Too Long)로 실패합니다.
* 자산에 파일 이름에 쉼표(`,`)가 들어 있는 경우 빈 zip 폴더가 다운로드됩니다.
* 뷰어 사용자에게는 사용자가 만든 컬렉션에 추가할 수 있는 옵션이 제공됩니다.
* 공유 링크를 사용하여 자산(축소판 또는 웹 표현물)을 다운로드할 때 일관되지 않은 동작이 발생합니다.

[Brand Portal 2021.02.0](whats-new.md)의 새로운 기능 을 참조하십시오.


### 알려진 문제 {#known-issues}

이 릴리스에는 다음과 같은 알려진 문제가 포함되어 있습니다.

* 사용자가 자산 소싱 게시 워크플로우에 대한 이메일 알림을 받지 않습니다.

<!--
### Known Issues {#known-issues}

This release includes the following known issue:

* Search on the **[!UICONTROL Asset Reports]** shows processing on the product interface with no search result.
* The video DM encodes are not visible to the non-admin users on the asset details page.
* The alignment of the size of individual asset renditions and total download size is distorted in the Download dialog.
-->


<!--
* Download Settings configuration to configure asset download from Brand Portal. Fast download, custom renditions, and system renditions are the available configurations. 
-->

<!--
* Document Viewer has been introduced to enhance the PDF viewing experience. New options are available for viewing the PDF files in Brand Portal.

* Advances in the asset download process which improves the Brand Portal user experience while [downloading assets from Brand Portal](brand-portal-download-assets.md). Brand Portal administrators can configure **[!UICONTROL Fast Download]**, **[!UICONTROL Custom Renditions]**, and **[!UICONTROL System Renditions]** from the **[!UICONTROL Download]** settings. 

For details, see [what's new in Brand Portal 6.4.7](whats-new.md). 

### Critical Issues Fixed {#critical-issues-fixed-647}

This release includes fixes to the following critical issues:

* The viewer users are not permitted to share link for collections but the option to share is visible to them on the product interface.

* The **[!UICONTROL Download]** button on the options bar does not list all the licensed assets of the selected folder.

* The search takes longer to show the results for certain keywords.

* The **[!UICONTROL Agree]** and **[!UICONTROL Disagree]** check boxes does not appear on bulk selection of licensed and unlicensed assets during download.

* Filter-based search shows processing on the product interface with no search result. 

* The assets do not download from share link if the shared folder contains numerous and large assets.


### Known Issues {#known-issues-647}

This release includes the following known issues:

* If multiple assets are selected, license text does not appear on clicking Terms and Conditions on the license agreement page during download using share link.   

-->

## 언어 {#languages}

Brand Portal 사용자 인터페이스는 다음 언어로 제공됩니다.

* 영어
* 독일어
* 프랑스어
* 스페인어
* 이탈리아어
* 브라질 포르투갈어
* 일본어
* 중국어 간체
* 한국어

## 인증된 플랫폼 {#certified-platforms}

이 Brand Portal 릴리스에서 실행하도록 인증된 플랫폼을 확인하려면 **터치에 적합한 UI 지원** 열을 참조하여 [기술 요구 사항](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html)의 **사용자 인터페이스를 작성할 지원되는 브라우저** 섹션에 있는 표를 참조하십시오.

## 링크 {#links}

* [adobe.com의 Adobe Experience Manager 제품 페이지](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Assets Brand Portal 설명서](https://helpx.adobe.com/kr/experience-manager/brand-portal/user-guide.html)

## 제품 액세스 및 지원(제한된 사이트) {#product-access-and-support-restricted-sites}

다음 사이트는 고객만 사용할 수 있습니다. 고객이고 액세스 권한이 필요한 경우 Adobe 계정 관리자에게 문의하십시오.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

* [제품 액세스](https://login.marketing.adobe.com)

* [고객 지원 Adobe](https://helpx.adobe.com/contact.html)
