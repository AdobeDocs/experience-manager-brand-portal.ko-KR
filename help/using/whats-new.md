---
title: AEM Assets 브랜드 포털의 새로운 기능
seo-title: AEM Assets 브랜드 포털의 새로운 기능
description: 6.4.5의 새로운 기능과 향상된 기능을 살펴보십시오.
seo-description: 6.4.5의 새로운 기능과 향상된 기능을 살펴보십시오.
uuid: 2c59d738-9b53-4f25-a205-13bf75c80b77
contentOwner: bdhar
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: 참조
topic-tags: 소개
discoiquuid: fec32ca3-142b-4a11-9b92-5113fc27277a
translation-type: tm+mt
source-git-commit: f5318420b4598ece27d8dfac4f4e7e0c5a02753d

---


# AEM Assets 브랜드 포털의 새로운 기능 {#what-s-new-in-aem-assets-brand-portal}

AEM(Adobe Experience Manager) 자산 브랜드 포털을 통해 승인된 크리에이티브 자산을 손쉽게 확보, 제어 및 장치 간 외부 사용자와 내부 비즈니스 사용자에게 안전하게 배포할 수 있습니다. 자산 공유의 효율성을 향상시키고 자산 출시 시간을 단축하며 규정 준수 및 무단 액세스 위험을 줄일 수 있습니다. Adobe는 전반적인 브랜드 포털 경험을 개선하기 위해 노력하고 있습니다. 다음은 새로운 기능 및 개선 사항에 대한 간략한 개요를 제공합니다.

## 6.4.5의 변경 사항 {#what-changed-in-645}

브랜드 포털 6.4.5는 브랜드 포털 사용자(외부 에이전시/팀)에게 컨텐츠를 브랜드 포털에 업로드하고 AEM 자산에 게시할 수 있는 기능을 제공하는 데 중점을 두는 기능 릴리스입니다. 작성자 환경에 대한 액세스 권한 없이도 가능합니다. 이 기능은 브랜드 포털에서 **자산**&#x200B;소싱이라고 하며, 사용자가 자산을 기부하고 전 세계적으로 배포된 다른 브랜드 포털 사용자와 공유할 수 있는 양방향 메커니즘을 제공하여 고객 경험을 향상시킬 수 있습니다.

### 브랜드 포털의 자산 소싱 {#asset-sourcing-in-bp}

자산 소싱을 통해 AEM 관리자는 추가 자산 기여도 **속성을** 사용하여 새 폴더를 만들 수 있으므로, 만들어진 새 폴더를 브랜드 포털 사용자가 자산 제출을 위해 열도록 할 수 있습니다. 이렇게 하면 새로 만든 기여도 폴더 내에 NEW 및 SHARED라는 두 개의 추가 하위 폴더가 생성되는 워크플로우가 자동으로 **트리거됩니다** .

그런 다음 AEM 관리자는 기여도 폴더에 추가해야 하는 자산 유형과 기준선 자산 세트에 대한 개요를 SHARED **폴더에 업로드하여 BP** 사용자에게 필요한 참조 정보가 있는지 확인합니다. 그러면 관리자는 새로 만든 기여도 폴더를 브랜드 포털에 게시하기 전에 기여도 폴더에 대한 액세스 권한을 활성 브랜드 포털 사용자에게 부여할 **수** 있습니다.

사용자가 NEW 폴더에 컨텐츠 추가를 **완료하면** 기여도 폴더를 다시 AEM 작성자 환경에 게시할 수 있습니다. 가져오기를 완료하고 AEM Assets 내에서 새로 게시된 컨텐츠를 반영하는 데 몇 분이 걸릴 수 있습니다.

또한 모든 기존 기능은 변경되지 않습니다. 브랜드 포털 사용자는 기여도 폴더뿐만 아니라 허용된 다른 폴더에서도 자산을 보고, 검색하고, 다운로드할 수 있습니다. 또한 관리자는 기여도 폴더를 추가로 공유하고 속성을 수정하고 컬렉션에 자산을 추가할 수 있습니다. 최신 [브랜드 포털 릴리스 정보를 참조하십시오](brand-portal-release-notes.md).

>[!NOTE]
>
>브랜드 포털 사용자는 콘텐츠/에셋을 새 폴더에만 업로드할 **수** 있습니다.

>[!NOTE]
>
>브랜드 포털 계정/테넌트의 최대 업로드 제한은 **10GB입니다** .



![](assets/asset-sourcing.png)

### 브랜드 포털에서 자산 업로드 {#upload-assets-in-bp}

브랜드 포털 사용자는 기여도 폴더가 공유될 때마다 자동으로 펄스/이메일 알림을 수신하게 되므로 SHARED **폴더에서** 기본 컨텐츠를 다운로드하여 프로젝트의 요구 사항을 파악할 수 있습니다.

Brand Portal users with appropriate permissions can upload multiple assets or folders containing multiple assets to the contribution folder. However, please note that Brand Portal users are only able to upload assets to the NEW subfolder. **** The **SHARED** folder is meant for the distribution of project details and baseline assets.

![](assets/upload-asset6.png)

![](assets/upload-asset4.png)

>[!NOTE]
>
>Brand Portal users do not have permission to delete an uploaded asset.

### Publish contribution folder to AEM Assets {#publish-assets-to-aem}

Once upload is complete to the NEW folder, Brand Portal users can then publish the contribution folder back to AEM. **** It may take few minutes to import and reflect the published content/assets in AEM Assets.

The Brand Portal user and the AEM Administrator will receive pulse/email notifications both at the beginning and at the completion of the publish action, along with the job progress status (Queued/In-Progress/Success). AEM and Brand Portal administrators can also view the job status from their respective interfaces.

![](assets/upload-asset5.png)

## What changed in 6.4.4 {#what-changed-in-644}

Brand Portal 6.4.4 release focuses on enhancements to text search and top customer requests. See latest Brand Portal Release Notes.[](brand-portal-release-notes.md)

### Search enhancements {#search-enhancements}

브랜드 포털 6.4.4 버전부터는 필터링 창에서 속성 조건자에 대한 부분 텍스트 검색을 지원합니다. 부분 텍스트 검색을 허용하려면 검색 양식에서 속성 **조건자에서** 부분 검색을 활성화해야 합니다.

Read on to know more about partial text search and wildcard search.

#### Partial phrase search {#partial-phrase-search}

이제 필터링 창에서 검색된 구문 중 단어 또는 두 개 부분만 지정하여 자산을 검색할 수 있습니다.

**사용**&#x200B;사례부분 구문 검색은 검색어에서 발생하는 단어의 정확한 조합을 잘 모르는 경우 유용합니다.

예를 들어, 브랜드 포털의 검색 양식에서 자산 제목에 대한 부분 검색에 속성 조건자를 사용하는 경우, **camp** 용어를 지정하면 제목 구문에 camp라는 단어가 있는 모든 자산이 반환됩니다.

![](assets/partialphrasesearch.png)

#### 와일드카드 검색 {#wildcard-search}

브랜드 포털에서는 검색 구문의 단어 일부와 함께 검색 쿼리에 별표(*)를 사용할 수 있습니다.

**사용 사례**&#x200B;검색된 구문에서 발생하는 정확한 단어를 잘 모를 경우 와일드카드 검색을 사용하여 검색 쿼리의 간격을 채울 수 있습니다.

예를 들어, **scripe*****을 지정하면 브랜드 포털의 검색 양식에서 자산 제목에서 부분 검색에 속성 조건자를 사용하는 경우 제목 구문에 문자가** 올라간단어가 있는 모든 자산을 반환합니다.

![](assets/wildcard-prop.png)

마찬가지로 지정:

* ***climb** 는 **제목 구문에 글자로 끝나는 단어가 있는 모든 자산을** 반환합니다.

* ***climb*** 은 제목 구문의 글자로 구성된 단어가 포함된 모든 **자산을 반환합니다** .

>[!NOTE]
>
>부분 검색 **확인란을 선택하면** 기본적으로 **대소문자** 무시가 선택됩니다.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-searching.md#facetedsearchbyapplyingfilterstosearch)

## 6.4.3의 변경 사항 {#what-changed-in}

브랜드 포털 6.4.3 릴리스는 — 브랜드 포털 액세스 URL에서 임차인 ID 외에 대체 별칭을 조직에 제공, 새로운 폴더 계층 구성, 비디오 지원 개선 사항, AEM 작성자 인스턴스에서 브랜드 포털로 예약된 게시, 운영 개선 사항 — 카테고리를 고객 요청에 연결합니다.

### 관리자가 아닌 사용자를 위한 폴더 계층 탐색

이제 관리자는 로그인 시 관리자가 아닌 사용자(편집기, 뷰어 및 게스트 사용자)에게 폴더가 표시되는 방식을 구성할 수 있습니다. [폴더 계층](../using/brand-portal-general-configuration.md) 활성화 구성이 관리 도구 **패널의 일반**&#x200B;설정에 추가됩니다. 구성이 다음과 같은 경우:

* **활성화되면**&#x200B;루트 폴더에서 시작하는 폴더 트리가 관리자가 아닌 사용자에게 표시됩니다. 따라서 관리자와 유사한 탐색 경험을 제공할 수 있습니다.
* **비활성화하면**&#x200B;공유 폴더만 랜딩 페이지에 표시됩니다.

![](assets/enable-folder-hierarchy.png)
사용**사례**

폴더 계층 [활성화](../using/brand-portal-general-configuration.md) 기능(활성화되면)을 사용하면 다른 계층과 공유된 동일한 이름으로 폴더를 구별할 수 있습니다. 로그인하면 관리자가 아닌 사용자가 공유 폴더의 가상 상위(및 상위) 폴더를 보게 됩니다.
![](assets/disabled-folder-hierarchy1-2.png) ![](assets/enabled-hierarchy1-2.png)

공유 폴더는 가상 폴더의 각 디렉토리 내에 구성됩니다. 이러한 가상 폴더는 잠금 아이콘을 사용하여 인식할 수 있습니다.

가상 폴더의 기본 축소판은 첫 번째 공유 폴더의 축소판 이미지입니다.

![](assets/hierarchy1-nonadmin-2.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-general-configuration.md)

### 특정 폴더 계층 구조 또는 경로에서 검색

**경로 브라우저** 조건자는 특정 디렉토리에서 자산을 검색할 수 있도록 검색 양식에서 도입됩니다. The default search path of search predicate for Path Browser is /content/dam/mac/&lt;tenant-id&gt;/, which can be configured by editing the default search form.**

* Admin users can use Path Browser to navigate to any folder directory on Brand Portal.
* Non-admin users can use Path Browser to navigate only to the folders (and navigate back to the parent folders) shared with them.
For example, /content/dam/mac/&lt;tenant-id&gt;/folderA/folderB/folderC is shared with a non-admin user. ** The user can search for assets within folderC using Path Browser. This user can also navigate to folderB and folderA (since they are ancestors of the folderC that is shared with the user).

![](assets/edit-search-form.png)

**The use case**

You can now restrict asset search within a specific folder you have browsed to, instead of beginning at the root folder.

Note that searching under these folders returns results only from the assets that have been shared with the user.

![](assets/filter-panel.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-search-facets.md#listofsearchpredicates)

### Dynamic Media video renditions support

Users whose AEM Author instance is on Dynamic Media hybrid mode can preview and download the dynamic media renditions, in addition to the original video files.

To allow preview and download of dynamic media renditions on specific tenant accounts, administrators need to specify Dynamic Media Configuration (video service URL (DM-Gateway URL) and registration ID to fetch the dynamic video) in Video configuration from admin tools panel.********

**The use case
Dynamic Media videos can be previewed on:**

* Asset details page
* 자산의 카드 보기
* Link share preview page

다이내믹 미디어 비디오 인코딩은 다음 사이트에서 다운로드할 수 있습니다.

* 브랜드 포털
* 공유 링크

![](assets/edit-dynamic-media-config.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### 브랜드 포털에 예약된 게시

AEM(6.4.2.0) [에서](https://helpx.adobe.com/experience-manager/6-4/release-notes/sp-release-notes.html#main-pars_header_9658011) 만든 이 인스턴스에서 브랜드 포털로의 게시 워크플로우는 이후 날짜로 예약할 수 있습니다.

마찬가지로 게시된 자산은 나중 날짜(시간)에 포털에서 게시 취소 워크플로우를 예약하여 제거할 수 있습니다.

![](assets/schedule-publish.png)
![](assets/publishlater-workflow.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### URL에서 구성 가능한 테넌트 별칭

조직은 URL에 대체 접두사를 지정하여 포털 URL을 사용자 정의할 수 있습니다. 기존 포털 URL에서 임차인 이름에 대한 별칭을 얻으려면 조직이 Adobe 지원에 문의해야 합니다.

브랜드 포털 URL의 접두사만 사용자 지정할 수 있으며 전체 URL은 사용자 지정할 수 없습니다.\
예를 들어 기존 도메인 **geometrix.brand-portal.adobe.com** 을 사용하는 조직은 **요청 시 geometrixx.brand-portal.adobe.com** 을 만들 수 있습니다.

그러나 AEM 작성자 인스턴스는 테넌트 ID로만 [구성할](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) 수 있으며 임차인 별칭(대체) URL로는 구성할 수 없습니다.

**사용 사례**&#x200B;조직은 Adobe에서 제공하는 URL을 고수하는 대신 포털 URL을 사용자 정의하여 브랜딩 요구 사항을 충족할 수 있습니다.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### 향상된 다운로드 환경

이 릴리스는 클릭 수 및 경고 수 감소를 통해 간소화된 다운로드 환경을 제공합니다.

* 표현물만 다운로드하도록 선택(원본 자산이 아니라).
* 원본 변환에 액세스할 수 없을 때 자산 다운로드가 제한됩니다.

## 6.4.2의 변경 사항 {#what-changed-in-1}

브랜드 포털 6.4.2 릴리스는 조직의 에셋 배포 요구 사항을 해결하고 게스트 액세스를 통해 전 세계에 배포되는 많은 사용자에게 이를 수 있도록 지원하는 다양한 기능을 제공합니다. 이를 통해 다운로드가 가속화되고 최적의 환경을 제공할 수 있습니다. 또한 브랜드 포털은 관리자를 위한 새로운 구성, 새로 추가된 보고서, 고객 요청에 맞는 보고서 등을 통해 조직을 보다 효과적으로 제어할 수 있습니다.

### 게스트 액세스

![](assets/bp-login-screen-1.png)

AEM 브랜드 포털을 통해 고객이 포털에 액세스할 수 있습니다. 손님 사용자는 포털에 입장할 수 있는 자격 증명이 필요하지 않으며 모든 공용 폴더 및 컬렉션에 액세스하여 다운로드할 수 있습니다. 게스트 사용자는 자신의 Lightbox(비공개 컬렉션)에 에셋을 추가하고 동일한 에셋을 다운로드할 수 있습니다. 또한 관리자가 설정한 스마트 태그 검색 및 검색 조건자를 볼 수 있습니다. 게스트 세션에서는 컬렉션을 만들고 저장된 검색을 만들거나 추가로 공유하거나 폴더 및 컬렉션 설정에 액세스하고 자산을 링크로 공유할 수 없습니다.

조직에서 여러 개의 동시 손님 세션을 사용할 수 있으며 조직당 총 사용자 할당량의 10%로 제한됩니다.

게스트 세션은 2시간 동안 활성 상태로 유지됩니다. 따라서 lightbox의 상태는 세션 시작 시간으로부터 2시간까지 유지됩니다. 2시간 후 게스트 세션을 다시 시작해야 하므로 라이트박스 상태가 손실됩니다.

### 다운로드 시간 단축

Brand Portal users can leverage IBM Aspera Connect based fast downloads to get speeds up to 25x faster and enjoy a seamless download experience irrespective of their location across the globe. 브랜드 포털 또는 공유 링크에서 에셋을 보다 빠르게 다운로드하려면 조직에서 다운로드 가속이 **활성화된 경우 다운로드 대화 상자에서** 다운로드 가속 활성화 옵션을 선택해야 합니다.

![](assets/donload-assets-dialog-2.png)

To enable IBM Aspera based accelerated download for the organization, administrators Enable Download Acceleration option (which is disabled by default) from General Settings in the administrative tools panel. ****[](brand-portal-general-configuration.md#allow-download-acceleration) To know more about prerequisites and troubleshooting steps for downloading asset files faster from Brand Portal and shared links, refer Guide to accelerate downloads from Brand Portal.[](../using/accelerated-download.md#main-pars-header)

### User Logins Report

A new report, to track user logins, has been introduced. The User Logins report can be instrumental in enabling organizations to audit and keep a check on the delegated administrators and other users of Brand Portal.****

The report logs display names, email IDs, personas (admin, viewer, editor, guest), groups, last login, activity status, and login count of each user from Brand Portal 6.4.2 deployment until the time of report generation. Administrators can export the report as .csv. Along with other reports, User Logins report enables organizations to more closely monitor user interactions with the approved brand resources, thereby ensuring conformance to corporate compliance offices.

![](assets/user-logins-1.png)

### Access to original renditions

Administrators can restrict user access to original image files (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop) and give access to low-resolution renditions which they download from Brand Portal or shared link. This access can be controlled at user group level from Groups tab of User Roles page in admin tools panel.

![](assets/access-original-rend-1.png)

* By default, all the users are able to download original renditions as the Access to Original is enabled for all.
* Administrators need to deselect the respective checkboxes to prevent a group of users from accessing original renditions.
* 사용자가 여러 그룹의 구성원이지만 그룹 중 하나에만 제한이 있는 경우 해당 사용자에게 제한이 적용됩니다.
* The restrictions do not apply to administrators, even though they are members of restricted groups.
* 링크로 자산을 공유하는 사용자의 권한은 공유 링크를 사용하여 자산을 다운로드하는 사용자에게 적용됩니다.

### 카드 및 목록 보기의 폴더 계층 경로

이제 카드 보기에서 폴더 계층 정보를 관리자가 아닌 사용자(편집기, 뷰어 및 손님 사용자)에게 표시합니다. 이 기능을 사용하면 상위 계층 구조와 관련하여 사용자가 액세스하는 폴더의 위치를 알 수 있습니다.

폴더 계층 정보는 다른 폴더 계층과 공유된 다른 폴더와 이름이 유사한 폴더를 구별하는 데 특히 유용합니다. 관리자가 아닌 사용자가 공유된 자산의 폴더 구조를 모를 경우 이름이 유사한 자산/폴더가 혼동되는 것처럼 보입니다.

* 각 카드에 표시되는 경로는 카드 크기에 맞게 잘립니다. 그러나 잘린 경로 위로 마우스를 가져가면 전체 경로를 도구 팁으로 볼 수 있습니다.

![](assets/folder-hierarchy1-1.png)

목록 보기는 모든 브랜드 포털 사용자에게 열에 있는 자산의 폴더 경로를 보여줍니다.

![](assets/list-view-1.png)

### 자산 속성을 보는 개요 옵션

브랜드 포털에서는 관리자가 아닌 사용자(편집기, 뷰어, 게스트 사용자)에게 선택된 자산/폴더의 자산 속성을 볼 수 있는 개요 옵션을 제공합니다. 개요 옵션은 다음과 같이 표시됩니다.

1. 자산/폴더 선택 상단에 있는 도구 모음에서.
2. 레일 선택기 선택 드롭다운에서

자산/폴더를 선택하는 동안 개요 옵션을 선택하면 제목, 경로 및 자산 생성 시간을 볼 수 있습니다. 반면에 자산 세부 사항 페이지에서 개요 옵션을 선택하면 사용자가 자산의 메타데이터를 볼 수 있습니다.

![](assets/overview-option-2.png)

![](assets/overview-rail-selector-2.png)

## 새로운 구성

관리자는 특정 테넌트에 대해 다음 기능을 활성화/비활성화하기 위해 6개의 새로운 구성이 추가되었습니다.

* 게스트 액세스 허용
* 사용자가 브랜드 포털에 대한 액세스를 요청할 수 있도록 허용
* 관리자가 브랜드 포털에서 자산 삭제 허용
* 공개 컬렉션 만들기 허용
* 공개 스마트 컬렉션 만들기 허용
* 다운로드 가속 허용

위의 구성은 관리 도구 패널의 액세스 및 일반 설정에서 사용할 수 있습니다.

![](assets/access-configs-1.png)
![](assets/general-configs-1.png)
![](assets/admin-tools-panel-13.png)

### Adobe.io가 UI를 호스팅하여 Auth 통합 구성

브랜드 포털 6.4.2 버전부터는 Adobe.io [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/) 인터페이스를 사용하여 JWT 애플리케이션을 만듭니다. 이 경우 브랜드 포털과 AEM 자산 통합을 허용하도록 Auth 통합을 구성할 수 있습니다. Previously, the UI for configuring OAuth integrations was hosted in https://marketing.adobe.com/developer/. [](https://marketing.adobe.com/developer/) 자산 및 컬렉션을 브랜드 포털에 게시하기 위해 AEM 자산과 브랜드 포털을 통합하는 방법에 대한 자세한 내용은 브랜드 [포털과 AEM 자산 통합 구성을 참조하십시오](https://helpx.adobe.com/in/experience-manager/6-4/assets/using/brand-portal-configuring-integration.html).

## 검색 개선 사항

Administrators can make the property predicates non-case sensitive by using the updated property predicate, which has a check for Ignore Case. This option is available for property predicate and multi-value property predicate.\
However, the non-case sensitive search is comparatively slower than default search for property predicate. If there are too many non-case sensitive predicates in the search filter, the search can slow down. It is, therefore, advised to use the non-case sensitive search judiciously.

## What changed in 6.4.1 {#what-changed-in-2}

Brand Portal 6.4.1 is a platform upgrade release which brings in several new features and vital enhancements such as browsing, searching, and performance enhancements to deliver fulfilling customer experiences.

### Browse Enhancements

* New Content Tree rail to quickly navigate an asset hierarchy.

![](assets/contenttree-2.png)

* Introduced new keyboard shortcuts, for example (p) for navigation to properties page, (e) for Edit, and (ctrl+c) for copy operations.______
* Improved scrolling, lazy loading experience in card and list view for browsing large number of assets.
* Enhanced Card View with support for different-sized cards based on view setting.

![](assets/cardviewsettings-1.png)

* Card view now displays date/time stamp on hovering above the date label.

* Enhanced Column view with More Details under the asset snapshot, which lets you navigate to details page of an asset.****

![](assets/columnmoredetail.png)

* 이제 목록 보기에는 로케일, 자산 유형, 차원, 크기, 등급 및 게시 정보 외에 기본적으로 첫 번째 열에 자산의 파일 이름이 표시됩니다. 새 **보기** 설정을 사용하여 목록 보기에 표시할 세부 사항의 양을 구성할 수 있습니다.

* 새로운 탐색 단추를 사용하여 자산 간 뒤로 이동하거나 자산 카운트를 보는 기능을 사용하여 자산 세부 사항 환경을 개선했습니다.

![](assets/navbtn.png)

* 자산의 세부 사항 페이지에서 AEM에서 업로드된 오디오 파일을 미리 보는 새로운 기능입니다.
* 자산 속성에 제공된 새 관련 자산 기능. AEM의 다른 소스/파생 자산과 관련되고 브랜드 포털에 게시된 자산은 이제 브랜드 포털에서 관련 자산에 대한 링크가 있는 관계를 유지합니다.
* 관리자가 아닌 사용자가 공개 컬렉션을 만들지 못하도록 제한하는 새로운 구성이 도입되었습니다. 조직은 Adobe 지원 팀과 협력하여 특정 계정에서 이 기능을 구성할 수 있습니다.

### 향상된 검색 기능

* 검색 쿼리를 다시 실행하지 않고 검색 항목으로 이동한 후 검색 결과에서 동일한 위치로 되돌리기 위해 도입된 기능입니다.
* 새 검색 결과 수를 입력하여 검색 결과를 표시합니다.
* 이전 이미지, 문서, 멀티미디어 옵션과 비교하여 .jpg, .png 및 .psd와 같은 세밀한 MIME 유형을 기반으로 검색 결과를 필터링할 수 있는 향상된 파일 유형 검색 필터.
* 이전 시간 슬라이더 기능 대신 정확한 타임스탬프를 사용하여 컬렉션에 대한 검색 필터가 향상되었습니다.
* 공개 또는 비공개 컬렉션을 검색하기 위해 새로운 액세스 유형 필터가 도입되었습니다.

![](assets/accesstypefilter.png)

### 최적화 다운로드

* 하나의 대용량 파일은 zip 파일을 작성하지 않고도 직접 다운로드되므로 속도와 처리량이 향상됩니다.
* 링크 공유 기능에 대한 Zip 다운로드 제한이 1GB에서 5GB로 늘어났습니다.

* 이제 사용자는 브랜드 포털 또는 공유 링크 기능을 통해 에셋을 다운로드하는 동안 사용자 정의 파일과 원본 파일만 다운로드하도록 선택할 수 있고 기본 변환을 방지할 수 있습니다.

![](assets/excludeautorendition.png)

### 향상된 성능

* 자산 다운로드 속도가 최대 100% 향상되었습니다.
* 자산에 대한 검색 응답에서 최대 40% 향상
* 검색 성능이 최대 40% 향상되었습니다.

**참고**:연구실에서 실시한 테스트에 따르면 향상된 기능이 포함되어 있습니다.

### 향상된 보고 기능

**도입된 링크 공유**&#x200B;보고서 공유 링크에 대한 정보를 제공하는 새로운 보고서가 도입되었습니다. 링크 공유 보고서는 지정된 기간 동안 조직 내 및 외부 사용자와 공유된 자산에 대한 모든 URL을 나열합니다. 또한 링크가 공유된 시기, 작성자 및 만료일이 표시됩니다.

![](assets/navigatereport.png)

**사용 보고서에 액세스하기 위해 진입점을 수정했습니다.**&#x200B;이제 사용 보고서가 다른 보고서와 통합되었으며 이제 자산 보고서 콘솔에서 볼 수 있습니다. 자산 보고서 콘솔에 도달하려면 관리 도구 **패널에서 보고서** 만들기/관리로 이동합니다.

![](assets/accessassetreport.png)

**브랜드 포털의 보고**&#x200B;인터페이스를 통한 사용자 환경이 개선되어 보다 직관적이고 효과적으로 조직을 제어할 수 있게 되었습니다. 관리자는 다양한 보고서를 만드는 것 외에도 생성된 보고서를 다시 방문하여 다운로드하거나 삭제할 수 있습니다. 이러한 보고서는 브랜드 포털에 저장되므로 이러한 보고서를 삭제할 수 있습니다.

만들어지는 각 보고서는 기본 열을 추가하거나 제거하여 사용자 지정할 수 있습니다. 또한 사용자 지정 열을 다운로드, 만료 및 게시 보고서에 추가하여 세부기간을 제어할 수 있습니다.

### 향상된 관리 툴

미리 입력 및 탐색 기능이 있는 메타데이터, 검색 및 보고서에 대한 관리 도구의 속성 선택기를 개선하여 관리 경험을 간소화할 수 있습니다.

### 기타 개선 사항

* AEM 6.3.2.1 및 6.4에서 브랜드 포털에 게시된 자산은 이제 AEM Assets 브랜드 포털 복제 대화 상자에서 공개 폴더 게시 확인란을 표시하여 브랜드 포털의 일반 사용자가 공개적으로 사용할 수 있도록 할 수 있습니다.

![](assets/public-folder-publish.png)

* 관리자가 액세스 요청 이메일을 통해, 누군가 브랜드 포털에 대한 액세스를 요청한 경우 브랜드 포털 알림 영역의 알림과는 별도로 알림을 받습니다.

## 6.3.2의 변경 사항 {#what-changed-in-3}

Brand Portal 6.3.2에는 주요 고객 요청과 일반 성능 향상을 위한 새로운 기능과 향상된 기능이 포함되어 있습니다.

### 브랜드 포털에 대한 액세스 요청 {#request-access-to-brand-portal}

이제 사용자는 브랜드 포털의 로그인 화면에서 사용할 수 있는 새로운*****액세스 권한이 필요함을 사용하여 브랜드 포털에 대한 액세스를 요청할 수 있습니다.

![](assets/bplogin_request_access.png)

사용자가 Adobe ID를 가지고 있는지 또는 Adobe ID를 만들어야 하는지에 따라 사용자는 적절한 워크플로우에 따라 요청을 제출할 수 있습니다. 브랜드 포털 제품 관리자는 알림 영역에서 이러한 요청을 받고 Adobe Admin Console을 통해 액세스 권한을 부여합니다.

자세한 내용은 브랜드 포털에 [대한 액세스 권한 요청을 참조하십시오](../using/brand-portal.md#requestaccesstobrandportal).

### 다운로드된 자산 보고서의 개선 사항 {#enhancement-in-the-assets-downloaded-report}

이제 다운로드한 자산 보고서에 지정된 날짜 및 시간 범위 내의 사용자당 자산 다운로드 수가 포함됩니다. 사용자는 이 보고서를 .csv 형식으로 다운로드하고 라이센스가 있는 자산에 대한 총 다운로드 수와 같은 데이터를 컴파일할 수 있습니다.

![](assets/reports_download_downloaded_by.png)

자세한 내용은 추가 보고서 [](../using/brand-portal-reports.md#createandmanageadditionalreports)만들기 및 관리의 3단계와 6단계를 참조하십시오.

### 브랜드 포털 유지 관리 알림 {#brand-portal-maintenance-notification}

이제 브랜드 포털에서 예정된 유지 관리 활동 며칠 전에 알림 배너를 표시합니다. 샘플 알림:

![](assets/bp_maintenance_notification-1.png)

자세한 내용은 브랜드 포털 [유지 관리 알림을](https://helpx.adobe.com/experience-manager/brand-portal/using/brand-portal.html#BrandPortalmaintenancenotification)참조하십시오.

### 링크 공유 기능을 사용하여 공유된 라이센스 자산에 대한 향상된 기능 {#enhancement-for-licensed-assets-shared-using-the-link-share-feature}

링크 공유 기능을 사용하여 라이선스가 부여된 에셋을 다운로드하는 동안 해당 에셋에 대한 사용권 계약에 동의하라는 메시지가 표시됩니다.

![](assets/copyright_management.png)

자세한 내용은 링크로 [](../using/brand-portal-link-share.md#shareassetsasalink)자산 공유의 12단계를 참조하십시오.

### 향상된 사용자 선택기 {#user-picker-enhancement}

이제 사용자 피커 성능이 크게 사용자 기반을 갖춘 고객의 요구 사항에 맞게 개선되었습니다.

### Experience Cloud 브랜딩 변경 사항 {#experience-cloud-branding-changes}

이제 브랜드 포털은 새로운 Adobe Experience Cloud 브랜딩을 준수합니다.

![](assets/bp_solution_switcher.png)

## 6.3.1의 변경 사항 {#what-changed-in-4}

Brand Portal 6.3.1에는 AEM과 브랜드 포털을 맞추기 위한 새롭고 향상된 기능이 포함되어 있습니다.

### 업그레이드된 사용자 인터페이스 {#upgraded-user-interface}

Adobe는 브랜드 포털 사용자 경험을 AEM과 정렬하기 위해 Coral 3 사용자 인터페이스로 전환합니다. 이러한 변경 사항은 탐색, 모양 등 전반적인 유용성을 향상시킵니다.

#### 향상된 탐색 경험 {#enhanced-navigational-experience}

* 새로운 Adobe 로고를 통해 관리 툴을 신속하게 이용할 수 있습니다.

![](assets/aemlogo-3.png)

* 오버레이를 통한 제품 탐색:

![](assets/overlay_navigation.png)

* 상위 폴더로 빠른 탐색:

![](assets/navigationparentfolders.png)

* 필요한 컨텐츠 및 툴로 신속하게 검색 및 탐색:

![](assets/omnisearchicon.png)

### 향상된 검색 환경 {#enhanced-browsing-experience}

* 중첩된 폴더를 검색할 수 있는 새 열 보기:

![](assets/millercolumnnavigation.png) ![](assets/multi-columnview.png)

* 폴더의 자산 목록에서 업로드된 최신 자산이 맨 위에 표시됩니다.

### 향상된 검색 환경 {#enhanced-search-experience}

* 새로운 옴니어 검색 기능을 사용하면 검색 키워드를 입력할 때 자동 제안을 통해 관련 컨텐츠, 기능 또는 태그에 신속하게 액세스할 수 있습니다. 전체 검색 기능은 모든 검색 기능에서 사용할 수 있습니다.

![](assets/omnisearch_whatsnew.png)

* Omni 검색에 검색 필터를 추가하여 검색 범위를 좁히고 검색 속도를 높일 수도 있습니다.

![](assets/omnisearch_withfilters.png)

* 새로운 자산 등급 기반 검색을 사용하면 AEM 자산에서 게시되는 경우 등급이 있는 자산을 검색할 수 있습니다.
* 새로운 다중 값 검색 기능은 AND 연산자가 있는 여러 키워드를 허용하여 자산을 보다 빠르게 검색합니다.
* 새로운 검색 증폭 기능을 사용하면 특정 자산이 검색 결과의 맨 위에 표시되도록 검색 관련성을 개선할 수 있습니다.
* 새로운 경로 기반 검색 기능을 사용하면 해당 폴더의 에셋을 검색할 수 있도록 중첩 폴더의 경로를 제공할 수 있습니다.

#### 새로운 스마트 태그 기반 검색 {#new-smart-tags-based-search}

스마트 태그가 있는 이미지가 AEM Assets에서 브랜드 포털에 게시되는 경우 스마트 태그 이름을 검색 키워드로 사용하여 브랜드 포털에서 이러한 이미지를 검색할 수 있습니다. 이 기능은 파일만 사용할 수 있습니다.

### 향상된 다운로드 환경 {#enhanced-downloading-experience}

중첩된 폴더를 다운로드한 후 원래 폴더 계층 구조를 유지할 수 있습니다. 중첩된 폴더 내의 에셋은 별도의 폴더가 아니라 단일 폴더에서 다운로드할 수 있습니다.

### 향상된 성능 {#improved-performance}

검색, 검색 및 다운로드 기능이 향상되어 브랜드 포털 성능이 크게 향상되었습니다.

### 자산을 위한 새로운 디지털 권한 관리 {#new-digital-rights-management-for-assets}

관리자는 자산을 공유하기 전에 자산의 만료 날짜 및 시간을 설정할 수 있습니다. 에셋이 만료되면 뷰어 및 편집자는 볼 수 있지만 다운로드할 수 없습니다. 자산이 만료되면 관리자는 알림을 받습니다.

### 향상된 에셋 정렬 {#enhanced-asset-sorting}

목록 보기의 폴더에서 자산 정렬이 더 이상 첫 번째 페이지에 표시되는 자산 수로 제한되지 않습니다. 폴더의 모든 자산은 첫 번째 페이지에 모두 나열되는지 여부에 관계없이 정렬됩니다.

### 향상된 보고 {#reporting-capabilities}

관리자는 다운로드, 만료, 게시 등 세 가지 유형의 보고서를 만들고 관리할 수 있습니다. 보고서에서 열을 구성하고 보고서를 CSV 형식으로 내보내는 기능도 사용할 수 있습니다.

![](assets/newreport.png)

### 추가 메타데이터 {#additional-metadata}

브랜드 포털 6.3.1에서는 AEM Assets 6.3과 유사한 추가 메타데이터를 제공합니다.스키마 편집기 양식을 사용하여 자산 속성 페이지에 표시되어야 하는 메타데이터를 제어할 수 있습니다. 자산 메타데이터는 외부 링크 공유 사용자에게 표시되지 않으며, 링크 공유 URL을 사용해서만 자산을 미리 보고 다운로드할 수 있습니다.

![](assets/additionsinmetadata.png)

### 관리자를 위한 추가 기능 {#additional-capabilities-for-administrators}

* 로그인 화면 배경 무늬에 대한 사용자 지정을 완료하기 전에 관리자가 변경 내용을 미리 볼 수 있습니다.

![](assets/wallpaperpreview.png)

* 관리자가 새 사용자를 추가한 후 브랜드 포털에 추가할 초대장을 수락하지 않아도 자동으로 추가됩니다.

### AEM Assets 6.3의 새로운 게시 기능 {#new-publishing-capabilities-in-aem-assets}

* AEM 관리자는 AEM 6.3 SP 1-CFP 1(6.3.1.1)을 사용하여 AEM 자산에서 브랜드 포털에 메타데이터 스키마를 게시할 수 있습니다. 이 스키마는 2017년 4분기에 제공될 예정입니다.

![](assets/publish_metadataschemaaemassets.png)

* AEM 관리자는 AEM 6.2 SP1-CFP7 및 AEM 6.3 SP 1-CFP 1(6.3.1.1)을 사용하여 AEM 자산의 모든 태그를 브랜드 포털에 게시할 수 있습니다.

![](assets/publish_tags_aemassets.png)

* AEM 자산에서 스마트 태그를 비롯한 태그가 있는 자산 및 컬렉션을 게시할 수 있습니다. 그런 다음 브랜드 포털에서 이러한 태그를 검색 키워드로 사용하여 이러한 자산 또는 컬렉션을 검색할 수 있습니다.

## Frequently asked questions {#frequently-asked-questions}

**Ques. 기존 자산, 기능 또는 구성을 이용하지 못할 수 있습니까?**
Ans**.** 모든 기존 기능과 구성은 그대로 유지됩니다. 최종 사용자는 영향을 받지 않으며 컨텐츠는 그대로 유지됩니다.

**Ques. 새로운 버전의 브랜드 포털로 전환하는 경우**
Ans**.** Brand Portal 6.4.4는 2019년 2월에 출시되었습니다. 다음 브랜드 포털 버전은 2019년 3분기에 출시될 예정입니다.

>[!NOTE]
>
>출시 일정은 잠정적이며 변경될 수 있습니다. Adobe 계정 관리자 또는 고객 지원에 문의하여 업데이트된 릴리스 일정을 얻으십시오.

**Ques. 사용자에게 영향을 미칩니까?**
Ans**.** 이 변경 사항은 브랜드 포털 내에서만 적용되므로 최종 사용자에게 영향을 주지 않습니다.

**Ques. 제가 해야 할 일이 있나요?**
Ans**.** 관리자가 작업을 수행할 필요가 없습니다. 새로운 브랜드 포털에 액세스하면 설명서를 참조하여 모든 벨소리 및 휘파람 기능을 확인하십시오.

**Ques. 질문 사항은 누구에게 문의해야 합니까?**
Ans**.** Adobe 계정 관리자 또는 고객 지원에 문의하십시오.