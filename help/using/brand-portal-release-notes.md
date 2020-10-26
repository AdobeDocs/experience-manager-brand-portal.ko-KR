---
title: 릴리스 정보
seo-title: 릴리스 정보
description: Adobe Experience Manager 에셋 브랜드 포털 2020.10.0 릴리스의 기능, 개선 사항, 중요 문제 및 알려진 문제에 대한 통찰력을 얻을 수 있습니다.
seo-description: Adobe Experience Manager 에셋 브랜드 포털 2020.10.0 릴리스의 개선 사항, 중요 문제 및 알려진 문제에 대한 통찰력을 얻을 수 있습니다.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: df378757f901a92de7003790651f623dcb92a4e3
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 10%

---


# 릴리스 노트 {#release-notes}

Adobe Experience Manager 에셋 브랜드 포털 2020.10.0 릴리스의 새로운 기능, 개선 사항, 주요 문제 및 알려진 문제에 대한 통찰력을 얻을 수 있습니다.

## 릴리스 정보 {#release-information}

| 제품 | Adobe Experience Manager 에셋 브랜드 포털 |
|---|---|
| 버전 | 2020.10.0 |
| 날짜 | 2020년 10월 |

## 개요 {#overview}

Adobe Experience Manager(AEM) 에셋 브랜드 포털은 승인된 크리에이티브 자산을 쉽게 획득하고 제어하며 다양한 디바이스를 사용하는 외부 관계자와 내부 비즈니스 사용자에게 안전하게 배포할 수 있도록 도와줍니다. 자산 공유의 효율성을 향상시키고, 자산 출시 시간을 단축하며, 규정 준수 여부에 대한 위험을 줄일 수 있습니다. 브랜드 포털을 통해 사용자는 언제 어디에서나 회사에서 승인한 포맷으로 자산을 검색, 검색, 미리 보기, 다운로드 및 내보낼 수 있습니다.

## 2020.10.0의 새로운 기능 {#whats-new-in-2020.10.0}

### New Features {#new-features}

이 릴리스에는 다음과 같은 새로운 기능이 포함됩니다.

* 필수 **[!UICONTROL 가 아닌 표현물을 제외하고 유사한 자산 유형에 대해 동일한 규칙 세트를 적용하고 선택한 자산 표현물을 다운로드할 수 있는 추가 옵션이 있는 목록 보기에서 다운로드]** 대화 상자가 개선되었습니다.

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

* 이제 **[!UICONTROL 파일]**, **[!UICONTROL 컬렉션]**&#x200B;및 **[!UICONTROL 공유 링크]** 를 한 번의 클릭으로 모든 브랜드 포털 페이지에서탐색할 수 있습니다.

* 이제 자산 세부 사항 페이지의 **[!UICONTROL 표현물]** 패널을 통해 브랜드 포털 사용자는 원래 자산 및(또는) 특정 자산 표현물을 선택하고, **[!UICONTROL 표현물]** 패널에서 직접 다운로드하여 **[!UICONTROL 다운로드 대화 상자를]** 열지 않아도 됩니다.

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

* 기존 **[!UICONTROL 다운로드]** 구성 외에도 브랜드 포털 관리자는 다른 사용자 그룹에 대한 권한을 구성하여 자산 세부 사항 페이지에서 원본 자산과 해당 표현물을 보고 다운로드할 수도 있습니다. 이러한 구성은 자산 표현물에 액세스할 수 있는 사람을 정의하고 (또는) 다운로드할 수 있습니다.

### 향상된 기능 {#enhancements}

이 릴리스에는 다음과 같은 개선 사항이 포함됩니다.

* 게스트 사용자의 세션 시간 초과 임계값이 2시간에서 15분으로 감소되었습니다.
* 이제 사용자가 Adobe Document Cloud 뷰어에서 **[!UICONTROL PDF 페이지를 볼 수 있으므로 여러 페이지 PDF에 대한 추가 페이지]** 보기 옵션이 제거되었습니다.


<!--
### Critical Issues Fixed {#critical-issues-fixed}

This release includes fixes to the following critical issue:

* The users are not able to view the PDF pages if the PDF contains sub assets.
-->

### 알려진 문제 {#known-issues}

이 릴리스에는 다음과 같은 알려진 문제가 포함됩니다.

* 자산 보고서에서 검색하면 **[!UICONTROL 제품]** 인터페이스에 검색 결과가 없는 처리가 표시됩니다.
* 자산 세부 사항 페이지에서 관리자가 아닌 사용자는 비디오 DM 인코딩을 볼 수 없습니다.
* 개별 자산 표현물과 총 다운로드 크기의 정렬이 다운로드 대화 상자에서 왜곡됩니다.



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

브랜드 포털 사용자 인터페이스는 다음 언어로 제공됩니다.

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

이 브랜드 포털 릴리스에서 실행하도록 인증된 플랫폼을 확인하려면 **기술 요구 사항** 의 **사용자 인터페이스** 작성에 [지원되는 브라우저 섹션에 있는 표의 터치에 적합한 UI](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html)지원 열을참조하십시오.

## 링크 {#links}

* [adobe.com의 Adobe Experience Manager 제품 페이지](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [자산 브랜드 포털 설명서](https://helpx.adobe.com/experience-manager/brand-portal/user-guide.html)

## 제품 액세스 및 지원(제한된 사이트) {#product-access-and-support-restricted-sites}

다음 사이트는 고객만 사용할 수 있습니다. 고객이고 액세스 권한이 필요한 경우 Adobe 계정 관리자에게 문의하십시오.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

* [제품 액세스](https://login.marketing.adobe.com)

* [Adobe 고객 지원 센터](https://helpx.adobe.com/contact.html)
