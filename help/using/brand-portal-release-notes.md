---
title: 릴리스 노트
seo-title: Release Notes
description: Adobe Experience Manager Assets Brand Portal 2021.10.0 릴리스의 기능, 개선 사항, 해결된 주요 문제 및 알려진 문제에 대한 통찰력을 얻을 수 있습니다.
seo-description: Get an insight into the enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 2021.10.0 release.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: a2a6eb19fb5405f59e3c88182c2a9c15f2bb4183
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 12%

---

# 릴리스 노트 {#release-notes}

Adobe Experience Manager Assets Brand Portal 2021.10.0 릴리스의 새로운 기능, 개선 사항, 해결된 주요 문제 및 알려진 문제에 대한 통찰력을 얻을 수 있습니다.

## 릴리스 정보 {#release-information}

| 제품 | Adobe Experience Manager Assets Brand Portal |
|---|---|
| 버전 | 2021.10.0 |
| 날짜 | 2021년 10월 일 |

## 개요 {#overview}

Adobe Experience Manager(AEM) Assets Brand Portal을 사용하면 승인된 크리에이티브 자산을 외부 당사자 및 내부 비즈니스 사용자가 간편하게 구매하고 제어하며 장치 간에 안전하게 분배할 수 있습니다. 자산 공유의 효율성을 향상시키고, 자산 출시 시간을 단축하며, 규정 준수 및 무단 액세스의 위험을 줄일 수 있습니다. Brand Portal을 사용하면 자산을 언제 어디서나 기업 승인 형식으로 검색, 미리 보기, 다운로드 및 내보낼 수 있습니다.

## 2021.10.0의 새로운 기능 {#whats-new-in-2021.10.0}

<!--
### New Features {#new-features}

This release includes the following new features:

* AEM Assets as a Cloud Service is now entitled to have a pre-configured Brand Portal instance. The Cloud Manager user can activate Brand Portal on the AEM Assets as a Cloud Service instance.

* Asset Sourcing feature is now available on AEM Assets as a Cloud Service. It allows the Brand Portal users to upload assets to the permitted contribution folders and publish the contribution folder from Brand Portal to AEM Assets as a Cloud Service instance. 

* An additional **[!UICONTROL Asset Download]** setting has been introduced under the **[!UICONTROL Download Settings]**. It creates a separate folder for each asset while downloading the folders, collections, or bulk download of assets. 
-->
<!-- 
* The **[!UICONTROL Download]** dialog is revamped in a list view with additional options to exclude the renditions which are not required, apply the same set of rules for similar asset types, and download the selected asset renditions.
-->

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

<!-- 
* Navigation to the **[!UICONTROL Files]**, **[!UICONTROL Collections]**, and **[!UICONTROL Shared Links]** is now possible from all the Brand Portal pages in one-click.  

* The **[!UICONTROL Renditions]** panel in the asset details page now allows the Brand Portal users to select the original asset and (or) specific asset renditions, and directly download them from the **[!UICONTROL Renditions]** panel without having to open the **[!UICONTROL Download]** dialog.
-->

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

<!-- 
* In addition to the existing **[!UICONTROL Download]** configurations, the Brand Portal administrators can also [configure permissions for different group of users]() to view and (or) download the original asset and its renditions from the asset details page. These configurations will define who can access and (or) download the asset renditions.
-->

<!--
### Enhancements {#enhancements}

Brand Portal 2021.08.0 is an internal release that introduces Business profiles for enterprise and teams customers to give organizations better control over their assets. 

This release includes the following enhancements:

* The users now have organization-specific entitlement on the new and migrated organizations. If a user is entitled to multiple organizations, the user has to select the organization at the time of login.

* The new users that are added in Admin Console must **Join Team** to get entitled to the organization. 

>[!NOTE]
>
>Business profiles are currently applicable for the new organizations that are created after August 16, 2021. 
>
>Until your organization is migrated, you can continue to use Adobe ID, Enterprise ID, or Federated ID types to access the organization.   
-->

<!-- 
* For folder download, a separate folder is created for each asset using share link irrespective of the **[!UICONTROL Download Settings]**. 
* The Brand Portal **[!UICONTROL Usage Report]** has been modified to reflect only the active Brand Portal users.
-->

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### 해결된 중요한 문제 {#critical-issues-fixed}

이 릴리스에는 다음과 같은 중요한 문제에 대한 수정 사항이 포함되어 있습니다.

* 크기가 동일한 기여도 폴더의 자산은 Brand Portal에서 Experience Manager 자산에 게시되지 않습니다.
* 기여도 폴더의 게재 여부는 게시 취소될 때 축소되지 않습니다.
* 사용자가 폴더에서 적용된 메타데이터 스키마 프로필을 제거할 수 없습니다.
* 사용자 권한 페이지의 그룹 수가 잘못되었습니다.
* 목록을 탐색할 때 컬렉션 페이지가 너무 오래 걸립니다.

<!--
* Asset Sourcing email notifications are not delivered for some organizations. 

* Video files with extension `.mov` are not running on Brand Portal. 

* In the **[!UICONTROL Smart Collections]** dropdown list, only ten saved collections are visible. 
-->
<!--
* *_deleted tenants are listed as valid tenant which fails during the execution of TenantCustomizers/TenantUpdates where tenant id is returned as /etc/tenants/`<nodename>`.
-->

<!--
In case only the original assets are downloaded, the asset reflects its own extension and does not open until the extension is manually changed to zip. 
* The user interface of the collection folder does not respond on clicking the navigation arrow. 
* **[!UICONTROL Create]** button is visible in the **[!UICONTROL Column]** view even when the folders are empty.
* **[!UICONTROL Omni search]** fails with a 414 error message (Request-URI Too Long) if the dispatcher is bypassed while accessing the Brand Portal instance.
* An empty zip folder is downloaded if the asset contains a comma (`,`) in the file name.
* The viewer users get the option to add users to the collection they have created. 
* Inconsistent behavior is experienced when an asset (thumbnail or web rendition) is downloaded using share link.

See [what's new in Brand Portal 2021.02.0](whats-new.md).
-->


### 알려진 문제 {#known-issues}

이 릴리스에는 다음과 같은 알려진 문제가 포함됩니다.

* 사용자는 기존 조직을 마이그레이션하는 동안 Brand Portal에 로그인할 수 없습니다.

   그러나 Brand Portal에 로그인한 활성 사용자는 현재 세션이 만료될 때까지 계속 작업할 수 있습니다.

* Brand Portal에서 Admin Console으로 이동할 때 관리자는 조직을 선택할 수 있는 추가 화면이 표시될 수 있습니다.


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

이 Brand Portal 릴리스에서 실행하도록 인증된 플랫폼을 확인하려면 **터치에 적합한 UI 지원** 열을 참조하여 [기술 요구 사항](https://experienceleague.adobe.com/docs/experience-manager-65/deploying/introduction/technical-requirements.html)의 **사용자 인터페이스를 작성할 지원되는 브라우저** 섹션에 있는 표를 참조하십시오.

## 링크 {#links}

* [adobe.com의 Adobe Experience Manager 제품 페이지](https://business.adobe.com/in/products/experience-manager/adobe-experience-manager.html)
* [Assets Brand Portal 설명서](https://experienceleague.adobe.com/docs/experience-manager-brand-portal/using/home.html)

## 제품 액세스 및 지원(제한된 사이트) {#product-access-and-support-restricted-sites}

다음 사이트는 고객만 사용할 수 있습니다. 고객이고 액세스 권한이 필요한 경우 Adobe 계정 관리자에게 문의하십시오.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

<!--
* [Customer Support](https://helpx.adobe.com/contact.html)
-->
