---
title: 릴리스 정보
seo-title: Release Notes
description: Adobe Experience Manager Assets Brand Portal 2023.02.0 릴리스의 기능, 개선 사항, 해결된 주요 문제 및 알려진 문제에 대한 통찰력을 얻을 수 있습니다.
seo-description: Get an insight into the enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 2023.02.0 release.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Kirandeep Kour
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: d5284a2ad62be2a72d168358d86b473257856592
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 7%

---

# 릴리스 정보 {#release-notes}

Adobe Experience Manager Assets Brand Portal 2023.02.0 릴리스의 새로운 기능, 개선 사항, 해결된 주요 문제 및 알려진 문제에 대한 통찰력을 얻을 수 있습니다.

## 릴리스 정보 {#release-information}

| 제품 | Adobe Experience Manager Assets Brand Portal |
|---|---|
| 버전 | 2023.02.0 |
| 날짜 | 2023년 2월 일 |

## 개요 {#overview}

Adobe Experience Manager(AEM) Assets Brand Portal을 사용하면 승인된 크리에이티브 자산을 외부 당사자 및 내부 비즈니스 사용자가 간편하게 구매하고 제어하며 장치 간에 안전하게 분배할 수 있습니다. 자산 공유의 효율성을 향상시키고 자산 출시 시간을 단축하며 규정 준수 및 무단 액세스의 위험을 줄일 수 있습니다. Brand Portal을 사용하면 자산을 언제 어디서나 기업 승인 형식으로 검색, 미리 보기, 다운로드 및 내보낼 수 있습니다.

## 의 새로운 2023.02.0 {#whats-new-in-2023.02.0}

### 해결된 중요한 문제 {#critical-issues-fixed}

#### 버그 수정 {#bug-fixes}

이 릴리스에는 다음과 같은 중요한 문제에 대한 수정 사항이 포함되어 있습니다.
* Brand Portal에서는 프로필 사진을 업데이트할 수 없습니다.
* 컨텐츠 트리 창의 크기는 조정할 수 없습니다. 파일 이름이 컨텐츠 트리의 기본 너비보다 긴 경우 컨텐츠 트리를 가로와 세로로 모두 드래그할 수 없습니다. 따라서 더 긴 파일 이름을 읽을 수 없습니다.
* 검색 양식에서 두 번 사용된 동일한 속성 설명을 위해 검색 결과가 일치하지 않습니다.
* 중간 로그인 페이지의 텍스트는 모든 언어에 대해 현지화되지 않습니다.

### 향상된 기능 {#enhancements}

이 릴리스에는 다음 개선 사항이 포함됩니다.
* 이제 PDF 자산의 향상된 미리 보기에 대해 최신 PDF 뷰어를 사용할 수 있습니다.
* 이제 관리자에 대한 자산 소싱 알림을 활성화하거나 비활성화하도록 선택할 수 있습니다. 다음으로 이동 [!UICONTROL 일반 설정] 그런 다음 활성화하거나 비활성화합니다 [!UICONTROL `Notify Administrator of asset contribution`].

   ![자산 기여 시 관리자에게 알림](assets/notify-admin.png)

* 요청 액세스가 비활성화된 경우 권한이 없는 사용자는 Brand Portal에 대한 액세스를 요청할 수 없습니다.
* Brand Portal에 대해 프로비저닝된 조직만 프로필 선택기 목록에 표시됩니다.

### 알려진 문제 {#known-issues}

이 릴리스에는 다음과 같은 알려진 문제가 포함되어 있습니다.

* 자산 소싱 보고서 컨텐츠의 부분 현지화.
* 사용자 프로필에서 일부 사용자 프로필을 편집할 수 없습니다.

## 이전 릴리스

### 2022년 10월 릴리스 {#oct-2022}

**해결된 중요한 문제**

이 릴리스에는 다음과 같은 중요한 문제에 대한 수정 사항이 포함되어 있습니다.
* Brand Portal에서 타사 도구로 대용량 파일을 복사하는 동안 응답 시간이 느려집니다.
* 표현물 수 확인란을 선택하면 개별 표현물을 선택하는 확인란이 비활성화됩니다.
* 검색에 대한 응답 시간이 느립니다.

>[!IMPORTANT]
>
>AEM Assets Brand Portal의 펄스 알림은 2022년 12월 1일부터 중단됩니다. 펄스 알림 대신 다음 이벤트에 대한 이메일 알림을 계속 받게 됩니다.
>* 링크를 통한 자산 공유
>* 액세스 워크플로우 요청
>* 기여도 폴더 공유
>* AEM으로 내보내기 시작
>* AEM으로 내보내기 완료
>


### 2022년 8월 릴리스 {#aug-2022}

**해결된 중요한 문제**

이 릴리스에는 다음과 같은 중요한 문제에 대한 수정 사항이 포함되어 있습니다.
* NUI가 Experience Manager에서 자산을 처리하지 못하면 Brand Portal에 부정확한 자산 가져오기 상태가 표시됩니다.
* 미리 보기 작업이 실패하면 실패를 알리는 알림이 없습니다.
* 각 자산에 대한 totalUploadedSize 속성에 대한 부정확한 값이 수정되었습니다.
* 를 클릭하면 **모든 항목 다운로드** 그리고 자산에 사용할 수 있는 표현물이 많습니다. Brand Portal은 잘못된 .ZIP 파일을 다운로드합니다.
* 일부 문자열의 번역은 Brand Portal 사용자 인터페이스에서 잘립니다.

### 2022년 5월 릴리스 {#may-2022}

**새로운 기능**

Brand Portal은 이제 12시간마다 자동 작업을 실행하여 AEM에 게시된 모든 Brand Portal 에셋을 삭제합니다. 따라서 폴더 크기를 임계값 제한 이하로 유지하기 위해 기여도 폴더에 에셋을 수동으로 삭제할 필요가 없습니다.

**해결된 중요한 문제**

이 릴리스에는 다음과 같은 중요한 문제에 대한 수정 사항이 포함되어 있습니다.

* 색상 태그가 있는 자산이 포함된 폴더나 컬렉션을 다운로드하면 XML 파일도 다운로드됩니다.
* 표현물이 포함된 비디오를 다운로드하면 Brand Portal에서 잘못된 .ZIP 파일을 만듭니다.
* AEM 작성기에서 사전 설정 및 자산을 만들고 Brand Portal에 게시한 다음 자산을 다운로드하는 동안 동적 변환을 선택하면 다운로드한 .ZIP 파일을 추출할 수 없습니다.
* Brand Portal에서 사용할 수 있는 특정 폴더에서 비디오 자산을 다운로드하는 동안 문제가 발생합니다.
* 이메일을 사용하여 기여도 폴더의 URL을 공유하는 경우 탐색 표시를 사용하여 상위 폴더에 액세스하는 동안 뷰어 및 편집기 역할에 문제가 발생합니다.
* 게시된 소싱 보고서에 잘못된 작업 시작 시간이 표시됩니다.

### 2022년 2월 릴리스 {#feb-2022}

**새로운 기능**

* 게스트 사용자에 대한 세션 시간 제한 임계값이 2시간에서 15분으로 줄었습니다.
* 추가 **[!UICONTROL 페이지 보기]** 사용자가 이제 Adobe Document Cloud 뷰어에서 PDF 페이지를 볼 수 있으므로 다중 페이지 PDF에 대한 옵션이 제거되었습니다.
* 사용자가 폴더를 검색, 탐색 또는 열 수 없습니다. 사용자 인터페이스에 오류 메시지가 표시됩니다. `Failed to load data`.
* 다음 **[!UICONTROL 표현물]** 패널에 Brand Portal에 게시된 자산의 모든 정적 표현물이 나열되지는 않습니다.
* 다음 **[!UICONTROL 표현물]** 패널에 자산의 스마트 자르기 렌디션이 나열되지만 사용자가 스마트 자르기 렌디션을 미리 보거나 다운로드할 수 없습니다.
* 다운로드 대화 상자에는 선택한 자산의 스마트 자르기 표현물이 표시되지만 스마트 자르기 렌디션은 다운로드할 수 없습니다.
* 관리자가 아닌 사용자가 자산을 다운로드할 때 원래 자산 표현물만 받게 됩니다. 시스템 및 사용자 지정 표현물은 다운로드되지 않습니다.
* 검색 필터를 적용하여 자산을 다운로드할 때 `Download` 버튼은 다운로드 대화 상자에서 비활성화되며 사용자가 자산을 다운로드할 수 없습니다.
* If `Smart Tags` 및 (또는) `Color Tags` 활성화되면 다운로드 대화 상자에 `json` 를 변환으로 지정하고 다음 파일을 다운로드합니다. `json` 보관된 zip 폴더에 있는 파일입니다.
* 링크가 Brand Portal 로그인 페이지로 리디렉션되므로 익명 사용자는 공유 링크를 사용하여 자산을 다운로드할 수 없습니다.
* 시스템이 활성 동시 사용자 수에 대한 올바른 값을 반영하지 않습니다.

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

* The users are unable to search, navigate, or open folders. The user interface reflects the error message: `Failed to load data`. 
* The **[!UICONTROL Renditions]** panel does not list all the static renditions of the assets that are published to Brand Portal.
* The **[!UICONTROL Renditions]** panel lists the smart crop renditions of the asset, however, the user cannot preview or download the smart crop renditions.
* The download dialog lists the smart crop renditions of the selected asset, however, the user cannot download the smart crop renditions. 
* A non-admin user is getting only the original asset rendition when downloading an asset. The system and custom renditions are not downloaded.  
* When applying search filter to download an asset, the `Download` button is disabled in the download dialog and does not allows the user to download the asset.
* If `Smart Tags` and (or) `Color Tags` are enabled, the download dialog lists the `json` files as renditions and downloads these `json` files in the archived zip folder.
* The anonymous users are unable to download assets using a shared link because the link redirects to the Brand Portal login page. 
* The system is not reflecting the correct value for the number of active concurrent users.
-->

<!--
### New features {#new-features}

Brand Portal now executes automatic jobs every twelve hours to delete all Brand Portal assets that are published to AEM. As a result, you do not need to delete the assets in the Contribution folder manually to keep the folder size below the threshold limit. See [What's new in Experience Manager Assets Brand Portal](whats-new.md).
-->

<!--
This release includes fixes to the following critical issues:

* When you download a folder or a collection that includes assets with color tags, an XML file gets downloaded as well.

* When you download a video that includes renditions, Brand Portal creates an invalid .ZIP file.

* When you create presets and assets on AEM author and publish them to Brand Portal and then select dynamic renditions while downloading the assets, you cannot extract the downloaded .ZIP file.

* Issues while downloading video assets from certain folders available on Brand Portal.

* When you share the Contribution folder’s URL using an email, Viewer and Editor roles face issues while accessing its parent folder using the breadcrumb.

* Sourcing published report displays an incorrect job start time.
>
 
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
* 포르투갈어(브라질)
* 일본어
* 중국어 간체
* 한국어

## 인증된 플랫폼 {#certified-platforms}

이 Brand Portal 릴리스에서 실행하도록 인증된 플랫폼을 확인하려면 **터치에 적합한 UI 지원** 테이블의 열 **사용자 인터페이스 작성을 위해 지원되는 브라우저** 섹션 [기술 요구 사항](https://experienceleague.adobe.com/docs/experience-manager-65/deploying/introduction/technical-requirements.html).

## 링크 {#links}

* [adobe.com의 Adobe Experience Manager 제품 페이지](https://business.adobe.com/in/products/experience-manager/adobe-experience-manager.html)
* [Assets Brand Portal 설명서](https://experienceleague.adobe.com/docs/experience-manager-brand-portal/using/home.html)

## 제품 액세스 및 지원(제한된 사이트) {#product-access-and-support-restricted-sites}

이러한 사이트는 고객만 사용할 수 있습니다. 고객이고 액세스 권한이 필요한 경우 Adobe 계정 관리자에게 문의하십시오.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

<!--
* [Customer Support]()
-->
