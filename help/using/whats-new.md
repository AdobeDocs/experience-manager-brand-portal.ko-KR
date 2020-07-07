---
title: AEM Assets Brand Portal의 새로운 기능
seo-title: AEM Assets Brand Portal의 새로운 기능
description: 6.4.6의 새로운 기능과 향상된 기능을 살펴보십시오.
seo-description: 6.4.6의 새로운 기능과 향상된 기능을 살펴보십시오.
uuid: 2c59d738-9b53-4f25-a205-13bf75c80b77
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: introduction
discoiquuid: fec32ca3-142b-4a11-9b92-5113fc27277a
translation-type: tm+mt
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '4462'
ht-degree: 3%

---


# AEM Assets Brand Portal의 새로운 기능 {#what-s-new-in-aem-assets-brand-portal}

Adobe Experience Manager(AEM) 자산 브랜드 포털은 승인된 크리에이티브 자산을 쉽게 획득하고 제어하며 다양한 장치에서 외부 당사자 및 내부 비즈니스 사용자에게 안전하게 배포할 수 있도록 도와줍니다. 자산 공유의 효율성을 향상시키고, 자산 출시 시간을 단축하며, 규정 준수 여부에 대한 위험을 줄일 수 있습니다. Adobe는 전반적인 브랜드 포털 경험을 개선하기 위해 노력하고 있습니다. 다음은 새로운 기능 및 개선 사항에 대한 간략한 소개입니다.

## 6.4.6의 변경 사항 {#what-changed-in-646}

브랜드 포털 6.4.6에서는 AEM Assets과 브랜드 포털 간의 인증 채널이 변경됩니다. 이제 AEM Assets 클라우드 서비스, AEM Assets 6.3 이상에서 브랜드 포털이 지원됩니다. AEM Assets 6.3 이상에서, 브랜드 포털은 이전 OAuth 게이트웨이를 통해 클래식 UI에서 이전에 구성되었으며, 이 게이트웨이는 JWT 토큰 교환을 사용하여 IMS 액세스 토큰을 인증하도록 사용합니다. 이제 AEM Assets은 브랜드 포털 임차인의 인증을 위해 IMS 토큰을 조달하는 Adobe 개발자 콘솔을 통해 브랜드 포털로 구성됩니다.

<!-- The steps to configure integration are different depending on your AEM version, and whether you are configuring for the first-time, or upgrading the existing integration:
-->

<!--
  
   | **AEM Version** |**New Integration** |**Upgrade Integration** |
|---|---|---|
| **AEM 6.5** |[Create new integration](../using/brand-portal-configure-integration-65.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-65.md#upgrade-integration-65) | 
| **AEM 6.4** |[Create new integration](../using/brand-portal-configure-integration-64.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-64.md#upgrade-integration-64) | 
| **AEM 6.3** |[Create new integration](../using/brand-portal-configure-integration-63.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-63.md#upgrade-integration-63) | 
| **AEM 6.2** |Contact Support |Contact Support | 

   -->

Brand Portal에서 AEM Assets을 구성하는 단계는 AEM 버전과 처음 구성하는 것인지 아니면 기존 구성을 업그레이드하는 것인지에 따라 다릅니다:

<!--| **AEM Version** |**New Configuration** |**Upgrade Configuration** |
|---|---|---|
| **AEM 6.5 (6.5.4.0 and above)** |[Create configuration](../using/brand-portal-configure-integration-65.md) |[Upgrade configuration](../using/brand-portal-configure-integration-65.md#upgrade-integration-65) | 
| **AEM 6.4 (6.4.8.0 and above)** |[Create configuration](../using/brand-portal-configure-integration-64.md) |[Upgrade configuration](../using/brand-portal-configure-integration-64.md#upgrade-integration-64) | 
| **AEM 6.3 (6.3.3.8 and above)** |[Create configuration](../using/brand-portal-configure-integration-63.md) |[Upgrade configuration](../using/brand-portal-configure-integration-63.md#upgrade-integration-63) | 
| **AEM 6.2** |Contact Support |Contact Support | 
-->


<!-- AEM Assets configuration with Brand Portal on Adobe I/O is supported on:
* AEM 6.5.4.0 and above
* AEM 6.4.8.0 and above
* AEM 6.3.3.8 and above -->

| **AEM 버전** | **새 구성** | **업그레이드 구성** |
|---|---|---|
| **클라우드 서비스로서의 AEM Assets** | [구성 만들기](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5(6.5.4.0 이상)** | [구성 만들기](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [구성 업그레이드](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4(6.4.8.0 이상)** | [구성 만들기](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [구성 업그레이드](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3(6.3.3.8 이상)** | [구성 만들기](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [구성 업그레이드](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | 지원 문의 | 지원 문의 |

>[!NOTE]
>
>AEM 인스턴스를 최신 서비스 팩으로 업데이트하는 것이 좋습니다.

최신 [브랜드 포털 릴리스 정보를 참조하십시오](brand-portal-release-notes.md).

브랜드 [포털 FAQ를 참조하십시오](brand-portal-faqs.md).

## 6.4.5의 변경 사항 {#what-changed-in-645}


Brand Portal 6.4.5는 작성자 환경에 액세스하지 않아도 컨텐츠를 Brand Portal에 업로드하고 AEM Assets에 게시할 수 있는 기능을 Brand Portal 사용자(외부 에이전시/팀)에게 제공하는 데 중점을 둔 기능 릴리스입니다. 이 기능은 브랜드 포털에서 **[자산 소싱이라고](brand-portal-asset-sourcing.md)**하며, 사용자가 자산을 기부하고 다른 글로벌 브랜드 포털 사용자와 공유할 수 있는 양방향 메커니즘을 제공하여 고객 경험을 향상시킬 수 있습니다.

### 브랜드 포털의 자산 소싱 {#asset-sourcing-in-bp}

자산 소싱을 통해 AEM 사용자(관리자/비관리 사용자)는 추가 **자산 기여도** 속성을 사용하여 새 폴더를 만들 수 있으므로, 만들어진 새 폴더를 브랜드 포털 사용자가 자산 제출을 위해 열도록 할 수 있습니다. 이렇게 하면 새로 만든 기여도 폴더 내에 NEW 및 SHARED라는 두 개의 하위 폴더가 추가로 생성되는 **워크플로우가 자동으로** 트리거됩니다.

그런 다음 AEM 사용자는 BP 사용자가 필요한 참조 정보를 갖도록 하기 위해 기여도 폴더에 추가해야 하는 자산의 유형에 대한 간단한 [](brand-portal-configure-contribution-folder-properties.md) 개요를 [](brand-portal-upload-baseline-assets.md)**업로드하고 기준 자산을** SHARED폴더에업로드하여 요구 사항을 정의합니다. 그러면 관리자는 새로 만든 기여도 폴더를 브랜드 포털에 게시하기 전에 기여도 폴더에 대한 액세스 권한을 활성 브랜드 포털 **사용자에게** 부여할 수 있습니다.


사용자가 NEW **폴더에 컨텐츠** 추가가 완료되면 기여도 폴더를 다시 AEM 작성자 환경에 게시할 수 있습니다. 가져오기를 완료하고 새로 게시된 컨텐츠를 AEM Assets 내에 반영하려면 몇 분 정도 걸릴 수 있습니다.

또한 모든 기존 기능은 변경되지 않습니다. 브랜드 포털 사용자는 기여도 폴더뿐만 아니라 허용된 다른 폴더에서 자산을 보고, 검색하고, 다운로드할 수 있습니다. 또한 관리자는 기여도 폴더를 추가로 공유하고, 속성을 수정하고, 컬렉션에 자산을 추가할 수 있습니다.

>[!NOTE]
>
>브랜드 포털의 자산 소싱은 AEM 6.5.2.0 이상에서 지원됩니다.
>
>이 기능은 이전 버전(AEM 6.3 및 AEM 6.4)에서 지원되지 않습니다.

### 기여도 폴더에 자산 업로드 {#upload-assets-in-bp}

적절한 권한을 가진 브랜드 포털 사용자는 자산 요구 사항을 [다운로드하여 기여도의 필요성을 파악하고 여러 자산이 들어 있는 여러 자산 또는 폴더를 기여도 폴더에 업로드할 수 있습니다](brand-portal-download-asset-requirements.md) . 그러나 브랜드 포털 사용자는 에셋을 **NEW** 하위 폴더에 업로드할 수만 있습니다. SHARED **** 폴더는 요구 사항 및 기준 자산의 배포를 위한 것입니다. 기여도 폴더에 자산 [업로드 참조](brand-portal-upload-assets-to-contribution-folder.md)

![](assets/upload-asset6.png)

![](assets/upload-asset4.png)


### AEM Assets에 기여도 폴더 게시 {#publish-assets-to-aem}

업로드가 NEW **** 폴더에 완료되면 브랜드 포털 사용자는 기여도 폴더를 다시 AEM에 게시할 수 있습니다. 게시된 콘텐츠/자산을 AEM Assets에 가져오고 반영하는 데 몇 분이 걸릴 수 있습니다. 참조, [기여도 폴더를 AEM Assets에 게시](brand-portal-publish-contribution-folder-to-aem-assets.md)


![](assets/upload-asset5.png)

## 6.4.4의 변경 사항 {#what-changed-in-644}

Brand Portal 6.4.4 릴리스는 텍스트 검색 향상 및 상위 고객 요청 사항에 중점을 둡니다. 최신 [브랜드 포털 릴리스 정보를 참조하십시오](brand-portal-release-notes.md).

### 향상된 검색 기능 {#search-enhancements}

Brand Portal 6.4.4 버전부터는 필터링 창에서 속성 조건자에 대한 부분 텍스트 검색을 지원합니다. 부분 텍스트 검색을 허용하려면 검색 양식에서 속성 **조건자에서** 부분 검색을 활성화해야 합니다.

부분 텍스트 검색 및 와일드카드 검색에 대해 자세히 알아보려면 읽어 보십시오.

#### 부분 구문 검색 {#partial-phrase-search}

이제 필터링 창에서 검색어 부분(단어 또는 두 개)만 지정하여 자산을 검색할 수 있습니다.

**사용 사례**&#x200B;부분 구문 검색은 검색어에서 발생하는 정확한 단어 조합을 잘 모르는 경우 유용합니다.

예를 들어, 브랜드 포털의 검색 양식에서 자산 제목에 대해 속성 조건자를 부분 검색에 사용하는 경우, **camp** 용어를 지정하면 제목 구문에 단어 camp가 있는 모든 자산을 반환합니다.

![](assets/partialphrasesearch.png)

#### 와일드카드 검색 {#wildcard-search}

브랜드 포털에서는 검색 구문의 단어 일부와 함께 검색 쿼리에 별표(*)를 사용할 수 있습니다.

**사용 사례**&#x200B;검색 구문에서 발생하는 정확한 단어를 잘 모를 경우 와일드카드 검색을 사용하여 검색 쿼리의 간격을 채울 수 있습니다.

예를 들어 **scaling*** 을 지정하면 브랜드 포털의 검색 양식에서 자산 제목에 대한 부분 검색을 위해 속성 설명 **을 사용하는 경우 제목 구문에서 문자가** 올라가는 단어가 있는 모든 자산을 반환합니다.

![](assets/wildcard-prop.png)

마찬가지로 지정:

* ***hiking** 은 **제목** 구문에 캐릭터로 끝나는 단어가 있는 모든 자산을 반환합니다.

* ***scaling*** 제목 구문의 글자로 구성된 **단어가 포함된 모든 자산을** 반환합니다.

>[!NOTE]
>
>부분 검색 **확인란을** 선택하면 **기본적으로 대/소문자** 무시가 선택됩니다.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-searching.md#facetedsearchbyapplyingfilterstosearch)

## 6.4.3의 변경 사항 {#what-changed-in}

브랜드 포털 6.4.3 릴리스는 브랜드 포털 액세스 URL에서 테넌트 ID뿐만 아니라 대체 별칭을 조직에 제공하는 것, 새로운 폴더 계층 구성, 비디오 지원 개선 사항, AEM Author 인스턴스에서 브랜드 포털로 예정된 게시, 운영 개선 사항 및 고객 요청에 대한 카테고리 등에 중점을 둡니다.

### 관리자가 아닌 사용자를 위한 폴더 계층 탐색

이제 관리자는 로그인 시 관리자가 아닌 사용자(편집기, 뷰어 및 게스트 사용자)에게 폴더가 표시되는 방식을 구성할 수 있습니다. [폴더 계층](../using/brand-portal-general-configuration.md) 활성화 구성이 관리 도구 패널의 **일반 설정**&#x200B;에 추가됩니다. 구성이 다음과 같은 경우:

* **활성화된**&#x200B;루트 폴더에서 시작하는 폴더 트리는 관리자가 아닌 사용자도 볼 수 있습니다. 따라서 관리자와 유사한 탐색 경험을 제공할 수 있습니다.
* **비활성화되어**&#x200B;있으면 공유 폴더만 랜딩 페이지에 표시됩니다.

![](assets/enable-folder-hierarchy.png)
**사용 사례**

폴더 계층 [활성화](../using/brand-portal-general-configuration.md) 기능(활성화된 경우)을 사용하면 다른 계층과 공유된 동일한 이름의 폴더를 구별할 수 있습니다. 로그인하면 관리자가 아닌 사용자가 공유 폴더의 가상 상위(및 상위) 폴더를 보게 됩니다.
![](assets/disabled-folder-hierarchy1-2.png) ![](assets/enabled-hierarchy1-2.png)

공유 폴더는 가상 폴더의 각 디렉토리 내에 구성됩니다. 이러한 가상 폴더는 잠금 아이콘으로 인식할 수 있습니다.

가상 폴더의 기본 축소판은 첫 번째 공유 폴더의 축소판 이미지입니다.

![](assets/hierarchy1-nonadmin-2.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-general-configuration.md)

### 특정 폴더 계층 또는 경로에서 검색

**경로 브라우저** 설명은 검색 양식에서 소개되어 특정 디렉토리에서 자산을 검색할 수 있도록 합니다. 경로 브라우저에 대한 검색 조건자의 기본 검색 경로 `/content/dam/mac/<tenant-id>/`는 기본 검색 양식을 편집하여 구성할 수 있습니다.

* 관리자 사용자는 경로 브라우저를 사용하여 브랜드 포털의 모든 폴더 디렉토리로 이동할 수 있습니다.
* 관리자가 아닌 사용자는 경로 브라우저를 사용하여 공유된 폴더만 탐색(그리고 상위 폴더로 다시 이동)할 수 있습니다.
예를 들어, 관리자 `/content/dam/mac/<tenant-id>/folderA/folderB/folderC` 가 아닌 사용자와 공유됩니다. 사용자는 경로 브라우저를 사용하여 folderC 내에서 자산을 검색할 수 있습니다. 또한 이 사용자는 folderB 및 folderA로 이동할 수 있습니다(사용자와 공유되는 folderC의 상위 폴더이기 때문).

![](assets/edit-search-form.png)

**사용 사례**

이제 루트 폴더에서 시작하는 대신 탐색한 특정 폴더 내에서 자산 검색을 제한할 수 있습니다.

이러한 폴더 아래에서 검색하면 사용자와 공유된 자산에서만 결과가 반환됩니다.

![](assets/filter-panel.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-search-facets.md#listofsearchpredicates)

### Dynamic Media 비디오 변환 지원

Dynamic Media 혼합 모드에 있는 AEM Author 인스턴스를 사용하는 사용자는 원본 비디오 파일 외에 다이내믹 미디어 변환을 미리 보고 다운로드할 수 있습니다.

특정 테넌트 계정에서 다이내믹 미디어 표현물의 미리 보기 및 다운로드를 허용하려면 관리자는 관리 도구 패널에서 **비디오** 구성에서 Dynamic Media 구성(비디오 서비스 URL(DM-게이트웨이 URL) 및 등록 ID)을 지정해야 합니다 **** .

**사용 사례** Dynamic Media 비디오는 다음과 같이 미리 볼 수 있습니다.

* 자산 세부 사항 페이지
* 자산의 카드 보기
* 링크 공유 미리 보기 페이지

Dynamic Media 비디오 인코딩은 다음 위치에서 다운로드할 수 있습니다.

* Brand Portal
* 공유 링크

![](assets/edit-dynamic-media-config.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### 브랜드 포털에 게시 예약

AEM(6.4.2.0) [의](https://helpx.adobe.com/experience-manager/6-4/release-notes/sp-release-notes.html#main-pars_header_9658011) 작성자 인스턴스에서 브랜드 포털에 대한 자산(및 폴더) 게시 워크플로우를 나중 날짜로 예약할 수 있습니다.

마찬가지로 게시된 에셋은 브랜드 포털에서 게시 취소 워크플로우를 예약하여 나중 날짜(시간)에 포털에서 제거할 수 있습니다.

![](assets/schedule-publish.png)
![](assets/publishlater-workflow.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### URL에서 구성 가능한 테넌트 별칭

조직은 URL에 대체 접두사를 추가하여 포털 URL을 사용자 정의할 수 있습니다. 기존 포털 URL에서 테넌트 이름에 대한 별칭을 얻으려면 조직이 Adobe 지원에 문의해야 합니다.

브랜드 포털 URL의 접두사만 사용자 정의할 수 있으며 전체 URL은 사용자 지정할 수 없습니다.\
예를 들어 기존 도메인 **geometritrix.brand-portal.adobe.com** 을 사용하는 조직은 요청 시 **geometrixx.brand-portal.adobe.com** 을 만들 수 있습니다.

하지만 AEM Author 인스턴스는 테넌트 URL로만 [구성할](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) 수 있으며 테넌트 별칭(대체) URL로는 구성할 수 없습니다.

**사용 사례**&#x200B;는 Adobe에서 제공하는 URL을 고수하는 대신 포털 URL을 사용자 지정하여 브랜딩 요구 사항을 충족할 수 있습니다.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### 향상된 다운로드 환경

이 릴리스는 클릭 수와 경고 횟수가 줄면서 간소화된 다운로드 환경을 제공합니다.

* 표현물만 다운로드하도록 선택(원본 자산이 아니라)
* 원본 변환에 액세스할 수 있는 경우 자산 다운로드가 제한됩니다.

## 6.4.2의 변경 사항 {#what-changed-in-1}

브랜드 포털 6.4.2 릴리스는 조직의 에셋 배포 요구 사항을 해결하고 게스트 액세스 및 가속화된 다운로드로 최적의 경험을 통해 전 세계에 배포된 많은 사용자에게 도달할 수 있도록 지원하는 다양한 기능을 제공합니다. 또한 브랜드 포털은 관리자를 위한 새로운 구성, 새로 추가된 보고서, 고객 요청에 맞는 보고서 등을 통해 조직을 더욱 강력하게 제어할 수 있도록 지원합니다.

### 게스트 액세스

![](assets/bp-login-screen-1.png)

AEM 브랜드 포털에서는 게스트가 포털에 액세스할 수 있도록 합니다. 손님 사용자는 포털에 입장할 수 있는 자격 증명이 필요하지 않으며 모든 공용 폴더 및 컬렉션에 액세스하여 다운로드할 수 있습니다. 게스트 사용자는 자신의 lightbox(비공개 컬렉션)에 에셋을 추가하고 이를 다운로드할 수 있습니다. 관리자가 설정한 스마트 태그 검색 및 검색 예측자를 볼 수도 있습니다. 게스트 세션은 사용자가 컬렉션과 저장된 검색을 만들거나 추가로 공유하거나 폴더 및 컬렉션 설정에 액세스하고 자산을 링크로 공유할 수 있도록 허용하지 않습니다.

조직에서 여러 개의 동시 손님 세션을 사용할 수 있으며 조직당 총 사용자 할당량의 10%로 제한됩니다.

게스트 세션은 2시간 동안 활성 상태로 유지됩니다. 따라서 lightbox의 상태도 세션 시작 시간으로부터 2시간까지 유지됩니다. 두 시간 후 게스트 세션을 다시 시작해야 하므로 lightbox 상태가 손실됩니다.

### 다운로드 가속화

브랜드 포털 사용자는 IBM Aspera Connect 기반의 빠른 다운로드를 활용하여 최대 25배 더 빠르게 다운로드할 수 있으며 전 세계 위치에 상관없이 원활한 다운로드 경험을 제공할 수 있습니다. 조직에서 다운로드 가속이 활성화되면 브랜드 포털 또는 공유 링크에서 에셋을 보다 빠르게 다운로드하려면 다운로드 대화 상자에서 **다운로드 가속** 활성화 옵션을 선택해야 합니다.

![](assets/donload-assets-dialog-2.png)

조직에 대해 IBM Aspera 기반 가속 다운로드를 활성화하려면 관리자가 관리 도구 패널의 **일반 설정에서** 다운로드 가속 [활성화 옵션(기본적으로 비활성화됨)을](brand-portal-general-configuration.md#allow-download-acceleration) 활성화합니다. 브랜드 포털 및 공유 링크에서 자산 파일을 더 빨리 다운로드하는 데 필요한 사전 요구 사항 및 문제 해결 단계에 대해 자세히 알아보려면 [가이드를 참조하여 브랜드 포털에서 다운로드 시간을 단축하십시오](../using/accelerated-download.md#main-pars-header).

### 사용자 로그인 보고서

사용자 로그인을 추적하는 새로운 보고서가 도입되었습니다. 사용자 **로그인** 보고서는 조직에서 위임된 관리자와 브랜드 포털의 다른 사용자를 감사하고 유지할 수 있도록 하는 데 도움이 될 수 있습니다.

보고서 로그에는 보고서 생성 시간까지 브랜드 포털 6.4.2 배포에서 각 사용자의 이름, 이메일 ID, 페르시아(관리자, 뷰어, 편집기, 손님), 그룹, 마지막 로그인, 활동 상태 및 로그인 카운트가 표시됩니다. 관리자는 보고서를 .csv로 내보낼 수 있습니다. 사용자 로그인 보고서는 다른 보고서와 함께 조직에서 승인된 브랜드 리소스와의 사용자 상호 작용을 보다 면밀하게 모니터링하여 기업 규정 준수 여부를 보장할 수 있도록 합니다.

![](assets/user-logins-1.png)

### 원본 변환에 액세스

관리자는 원본 이미지 파일(.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop)에 대한 사용자 액세스를 제한하고 저해상도에 액세스할 수 있습니다. 브랜드 포털 또는 공유 링크에서 다운로드하는 변환. 이 액세스는 관리 도구 패널의 사용자 역할 페이지의 그룹 탭에서 사용자 그룹 수준에서 제어할 수 있습니다.

![](assets/access-original-rend-1.png)

* 기본적으로 원본 액세스 권한이 모든 사용자에 대해 활성화되면 모든 사용자가 원본 변환을 다운로드할 수 있습니다.
* 관리자는 사용자 그룹이 원래 변환에 액세스하지 못하도록 해당 확인란을 선택 취소해야 합니다.
* 사용자가 여러 그룹의 구성원이지만 그룹 중 하나에만 제한이 있는 경우 해당 사용자에게 제한이 적용됩니다.
* 제한된 그룹의 구성원도 관리자에게는 적용되지 않습니다.
* 링크로 자산을 공유하는 사용자의 권한은 공유 링크를 사용하여 자산을 다운로드하는 사용자에게 적용됩니다.

### 카드 및 목록 보기의 폴더 계층 경로

이제 카드 보기에서 비관리 사용자에게 폴더 계층 정보를 표시하는 폴더 카드(편집기, 뷰어 및 게스트 사용자). 이 기능을 사용하면 상위 계층 구조와 관련하여 사용자가 액세스하는 폴더의 위치를 알 수 있습니다.

폴더 계층 정보는 다른 폴더 계층과 공유된 다른 폴더와 유사한 이름을 가진 폴더를 구분하는 데 특히 유용합니다. 관리자가 아닌 사용자가 공유된 자산의 폴더 구조를 알지 못하는 경우 이름이 유사한 자산/폴더가 혼동되는 것처럼 보입니다.

* 각 카드에 표시된 경로는 카드 크기에 맞게 잘립니다. 그러나 잘린 패스 위에 마우스를 놓으면 전체 경로를 도구 팁으로 볼 수 있습니다.

![](assets/folder-hierarchy1-1.png)

목록 보기에는 브랜드 포털의 모든 사용자에게 표시되는 열에 있는 자산의 폴더 경로가 표시됩니다.

![](assets/list-view-1.png)

### 자산 속성을 보는 개요 옵션

브랜드 포털에서는 선택한 자산/폴더의 자산 속성을 보기 위해 관리자가 아닌 사용자(편집기, 뷰어, 게스트 사용자)에게 개요 옵션을 제공합니다. 개요 옵션이 표시됩니다.

1. 자산/폴더 선택에 대한 맨 위의 도구 모음에서.
2. 레일 선택기 선택 드롭다운에서

자산/폴더를 선택하는 동안 [개요] 옵션을 선택하면 사용자가 에셋을 만든 제목, 경로 및 시간을 볼 수 있습니다. 반면에, 자산 세부 사항 페이지에서 개요 옵션을 선택하면 사용자가 자산의 메타데이터를 볼 수 있습니다.

![](assets/overview-option-2.png)

![](assets/overview-rail-selector-2.png)

## 새로운 구성

관리자는 특정 테넌트에 대해 다음 기능을 활성화/비활성화하기 위해 6개의 새로운 구성이 추가되었습니다.

* 게스트 액세스 허용
* 사용자가 브랜드 포털에 대한 액세스 권한 요청 허용
* 관리자가 브랜드 포털에서 자산 삭제 허용
* 공개 컬렉션 만들기 허용
* 공개 스마트 컬렉션 만들기 허용
* 다운로드 가속 허용

위의 구성은 관리 도구 패널의 액세스 및 일반 설정에서 사용할 수 있습니다.

![](assets/access-configs-1.png)
![](assets/general-configs-1.png)
![](assets/admin-tools-panel-13.png)

### Adobe I/O UI로 oAuth 통합 구성

Brand Portal 6.4.2 이상에서는 Adobe.io [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/) 인터페이스를 사용하여 JWT 애플리케이션을 만듭니다. 이 JWT 응용 프로그램을 만들면 AEM Assets과 브랜드 포털의 통합을 허용합니다. 이전에는 OAuth 통합을 구성하기 위한 UI가 에서 호스팅되었습니다 `https://marketing.adobe.com/developer/`. 브랜드 포털에 자산 및 컬렉션을 게시하기 위해 AEM Assets과 브랜드 포털 통합에 대해 자세히 알아보려면 브랜드 포털과 [AEM Assets 통합 구성을 참조하십시오](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html).

## 검색 개선 사항

관리자는 대/소문자 무시 확인을 포함하는 업데이트된 속성 조건자를 사용하여 속성 대/소문자를 구분하지 않도록 지정할 수 있습니다. 이 옵션은 속성 설명 및 다중 값 속성 조건자에 사용할 수 있습니다.\
그러나 대/소문자를 구분하지 않는 검색은 속성 조건자에 대한 기본 검색보다 상대적으로 느립니다. 검색 필터에 대/소문자가 구분되지 않는 예측이 너무 많으면 검색 속도가 느려질 수 있습니다. 따라서 대/소문자를 구분하지 않는 검색을 신중하게 사용하는 것이 좋습니다.

## 6.4.1의 변경 사항 {#what-changed-in-2}

Brand Portal 6.4.1은 고객의 기대에 부응하는 경험을 제공하기 위해 검색, 검색 및 성능 향상 등 몇 가지 새로운 기능과 주요 개선 사항을 제공하는 플랫폼 업그레이드 버전입니다.

### 향상된 검색 기능

* 새 컨텐츠 트리 레일을 사용하여 자산 계층 구조를 빠르게 탐색할 수 있습니다.

![](assets/contenttree-2.png)

* 속성 페이지로 이동하는 _(p)_ 경우, _(e)_ 편집용 _,_ 복사용(ctrl+c)등새로운 키보드 단축키가 추가되었습니다.
* 대량의 자산을 검색할 수 있도록 카드 및 목록 보기에서 스크롤, 지연 로드 환경이 개선되었습니다.
* 보기 설정에 따라 서로 다른 크기의 카드에 대한 지원을 통해 향상된 카드 보기

![](assets/cardviewsettings-1.png)

* 이제 카드 보기에 날짜 레이블 위에 마우스를 올려 놓으면 날짜/시간 스탬프가 표시됩니다.

* 자산 스냅샷 아래의 **자세한** 정보가 포함된 향상된 열 보기를 사용하여 자산의 세부 사항 페이지로 이동할 수 있습니다.

![](assets/columnmoredetail.png)

* 이제 목록 보기에는 로케일, 자산 유형, 차원, 크기, 등급 및 발행물 정보 외에도 기본적으로 첫 번째 열에 자산의 파일 이름이 표시됩니다. 새 **보기 설정** 을 사용하여 목록 보기에 표시할 세부 사항의 양을 구성할 수 있습니다.

* 새로운 탐색 단추를 사용하여 자산 간 뒤로 이동하거나 자산 카운트를 보는 기능을 사용하여 자산 세부 사항 환경이 개선되었습니다.

![](assets/navbtn.png)

* 자산의 세부 사항 페이지에서 AEM에서 업로드된 오디오 파일을 미리 보는 새로운 기능입니다.
* 자산 속성에 제공된 새 관련 자산 기능. 이제 AEM의 다른 소스/파생 자산과 관련되고 브랜드 포털에 게시된 자산은 속성 페이지의 관련 자산에 대한 링크와 함께 브랜드 포털에서 자신의 관계를 유지합니다.
* 관리자가 아닌 사용자가 공개 컬렉션을 만들지 못하도록 제한하는 새로운 구성이 도입되었습니다. 조직은 Adobe 지원 팀과 협력하여 특정 계정에 이 기능을 구성할 수 있습니다.

### 향상된 검색 기능

* 검색 쿼리를 다시 실행하지 않고 검색 항목으로 이동한 후 검색 결과에서 동일한 위치로 돌아가는 기능이 도입되었습니다.
* 제공된 검색 결과 수를 표시하는 새 검색 결과 카운트입니다.
* .jpg, .png 및 .psd와 같은 세밀한 MIME 유형을 기반으로 검색 결과를 필터링하는 기능을 이전 이미지, 문서, 멀티미디어 옵션과 비교하여 파일 유형 검색 필터가 향상되었습니다.
* 이전 시간 슬라이더 기능 대신 정확한 타임스탬프를 사용하여 컬렉션에 대한 검색 필터가 개선되었습니다.
* 공개 또는 비공개 컬렉션을 검색하기 위해 새로운 액세스 유형 필터가 도입되었습니다.

![](assets/accesstypefilter.png)

### 다운로드 최적화

* 하나의 큰 파일은 zip 파일을 작성하지 않고도 직접 다운로드되므로 속도와 처리량이 향상됩니다.
* 링크 공유 기능의 Zip 다운로드 제한이 1GB에서 5GB로 늘어났습니다.

* 이제 사용자는 브랜드 포털 또는 공유 링크 기능을 통해 에셋을 다운로드하는 동안 사용자 정의 파일과 원본 파일만 다운로드하도록 선택할 수 있으며, 기본 변환을 방지할 수 있습니다.

![](assets/excludeautorendition.png)

### 향상된 성능

* 에셋 다운로드 속도가 최대 100% 향상되었습니다.
* 자산에 대한 검색 응답에서 최대 40% 향상
* 검색 성능이 최대 40% 향상되었습니다.

**참고**: 연구실에서 실시한 테스트에 따르면 향상된 기능이 제공됩니다.

### 향상된 보고 기능

**도입된 링크 공유 보고서**&#x200B;공유 링크에 대한 정보를 제공하는 새로운 보고서가 도입되었습니다. 링크 공유 보고서는 지정된 기간 동안 조직 내 및 외부 사용자와 공유된 자산에 대한 모든 URL을 나열합니다. 또한 링크가 언제 공유되었는지, 누가 누구에 의해, 언제 만료되는지 알려줍니다.

![](assets/navigatereport.png)

**사용 보고서**&#x200B;사용 보고서에 액세스하기 위해 진입점을 수정했습니다. 이제 사용 보고서가 다른 보고서와 통합되었으며 이제 자산 보고서 콘솔에서 볼 수 있습니다. 자산 보고서 콘솔에 도달하려면 관리 도구 **패널에서 보고서** 만들기/관리로 이동합니다.

![](assets/accessassetreport.png)

**브랜드 포털의 보고**&#x200B;인터페이스 사용 환경이 개선되어 보다 직관적이고 효과적으로 조직을 제어할 수 있게 되었습니다. 다양한 보고서를 만드는 것 외에도 관리자는 생성된 보고서를 다시 방문하고 브랜드 포털에 저장되므로 이를 다운로드하거나 삭제할 수 있습니다.

만들어지는 각 보고서는 기본 열을 추가하거나 제거하여 사용자 지정할 수 있습니다. 또한 사용자 지정 열을 다운로드, 만료 및 게시 보고서에 추가하여 세부기간을 제어할 수 있습니다.

### 향상된 관리 툴

미리 입력 및 검색 기능이 포함된 메타데이터, 검색 및 보고서에 대한 관리 도구의 속성 선택기가 개선되어 관리 환경이 간소화됩니다.

### 기타 개선 사항

* 이제 AEM Assets 브랜드 포털 복제 대화 상자에서 공개 폴더 게시 확인란을 선택하여 AEM 6.3.2.1 및 6.4에서 브랜드 포털에 게시된 자산을 브랜드 포털 사용자에게 공개적으로 사용할 수 있습니다.

![](assets/public-folder-publish.png)

* 관리자가 브랜드 포털에 대한 액세스를 요청한 경우 브랜드 포털 알림 영역의 알림과는 별도로 액세스 요청 이메일을 통해 알림을 받습니다.

## 6.3.2의 변경 사항 {#what-changed-in-3}

브랜드 포털 6.3.2에는 주요 고객 요청과 일반 성능 향상을 위한 새롭고 향상된 기능이 포함되어 있습니다.

### Request access to Brand Portal {#request-access-to-brand-portal}

이제 사용자는 브랜드 포털의 로그인 화면에서 사용할 수 있는 새로운 **필수 액세스** 기능을 사용하여 브랜드 포털에 대한 액세스를 요청할 수 있습니다.

![](assets/bplogin_request_access.png)

사용자에게 Adobe ID이 있는지 또는 Adobe ID을 만들어야 하는지에 따라, 사용자는 적절한 워크플로우에 따라 요청을 제출할 수 있습니다. 브랜드 포털 제품 관리자는 알림 영역에서 이러한 요청을 받고 Adobe Admin Console을 통해 액세스 권한을 부여합니다.

자세한 내용은 브랜드 포털에 [대한 액세스 권한 요청을 참조하십시오](../using/brand-portal.md#requestaccesstobrandportal).

### 다운로드한 에셋의 개선 사항 보고서 {#enhancement-in-the-assets-downloaded-report}

이제 다운로드한 자산 보고서에 지정된 날짜 및 시간 범위 내의 사용자당 자산 다운로드 수가 포함됩니다. 사용자는 이 보고서를 .csv 형식으로 다운로드하고 라이센스가 있는 자산에 대한 총 다운로드 수와 같은 데이터를 컴파일할 수 있습니다.

![](assets/reports_download_downloaded_by.png)

자세한 내용은 추가 보고서 [만들기 및 관리의 3단계와 6단계를 참조하십시오](../using/brand-portal-reports.md#createandmanageadditionalreports).

### 브랜드 포털 유지 관리 알림 {#brand-portal-maintenance-notification}

이제 브랜드 포털에서 예정된 유지 관리 활동 며칠 전에 알림 배너를 표시합니다. 샘플 알림:

![](assets/bp_maintenance_notification-1.png)

자세한 내용은 [브랜드 포털 유지 관리 알림을 참조하십시오](https://helpx.adobe.com/experience-manager/brand-portal/using/brand-portal.html#BrandPortalmaintenancenotification).

### 링크 공유 기능을 사용하여 공유된 라이센스 자산에 대한 향상된 기능 {#enhancement-for-licensed-assets-shared-using-the-link-share-feature}

링크 공유 기능을 사용하여 라이선스가 부여된 에셋을 다운로드하는 동안 해당 에셋에 대한 사용권 계약에 동의하라는 메시지가 표시됩니다.

![](assets/copyright_management.png)

자세한 내용은 링크로 자산 [공유의 12단계를 참조하십시오](../using/brand-portal-link-share.md#shareassetsasalink).

### 사용자 선택 향상 {#user-picker-enhancement}

이제 대규모 사용자 기반을 통해 고객의 요구 사항에 맞게 사용자 선택 성능이 향상되었습니다.

### Experience Cloud 브랜딩 변경 사항 {#experience-cloud-branding-changes}

이제 브랜드 포털은 새로운 Adobe Experience Cloud 브랜딩을 준수합니다.

![](assets/bp_solution_switcher.png)

## 6.3.1의 변경 사항 {#what-changed-in-4}

Brand Portal 6.3.1에는 AEM과 함께 브랜드 포털을 맞추기 위한 새롭고 향상된 기능이 포함되어 있습니다.

### 업그레이드된 사용자 인터페이스 {#upgraded-user-interface}

Adobe는 브랜드 포털 사용자 경험을 AEM과 맞추기 위해 Coral 3 사용자 인터페이스로 전환할 예정입니다. 이러한 변경 사항은 탐색 및 외양을 비롯한 전반적인 유용성을 향상시킵니다.

#### 향상된 탐색 경험 {#enhanced-navigational-experience}

* 새로운 Adobe 로고를 통해 관리 툴에 신속하게 액세스:

![](assets/aemlogo-3.png)

* 오버레이를 통한 제품 탐색:

![](assets/overlay_navigation.png)

* 상위 폴더로 빠른 탐색:

![](assets/navigationparentfolders.png)

* 필요한 컨텐츠 및 툴로 신속하게 검색 및 탐색:

![](assets/omnisearchicon.png)

### 향상된 검색 환경 {#enhanced-browsing-experience}

* 중첩된 폴더를 탐색하는 새 열 보기:

![](assets/millercolumnnavigation.png) ![](assets/multi-columnview.png)

* 폴더의 자산 목록에 업로드된 최신 자산이 맨 위에 표시됩니다.

### 향상된 검색 환경 {#enhanced-search-experience}

* 새로운 옴니어 검색 기능을 사용하면 검색 키워드를 입력할 때 자동 제안을 통해 관련 컨텐츠, 기능 또는 태그에 빠르게 액세스할 수 있습니다. 옴니어 검색은 모든 검색 기능에서 사용할 수 있습니다.

![](assets/omnisearch_whatsnew.png)

* Omni search에 검색 필터를 추가하여 검색 범위를 더 좁히고 빠르게 진행할 수도 있습니다.

![](assets/omnisearch_withfilters.png)

* 새로운 자산 등급 기반 검색을 사용하면 AEM Assets에서 게시된 경우 등급이 있는 자산을 검색할 수 있습니다.
* 새로운 다중 값 검색 기능은 AND 연산자가 있는 여러 키워드를 허용하므로 자산을 보다 빠르게 검색할 수 있습니다.
* 새로운 검색 증폭 기능을 사용하면 특정 자산이 검색 결과의 맨 위에 표시되도록 검색 관련성을 개선할 수 있습니다.
* 새로운 경로 기반 검색 기능을 사용하면 해당 폴더의 에셋을 검색할 수 있도록 중첩된 폴더의 경로를 제공할 수 있습니다.

#### 새로운 스마트 태그 기반 검색 {#new-smart-tags-based-search}

스마트 태그가 있는 이미지가 AEM Assets에서 브랜드 포털로 게시되는 경우 스마트 태그 이름을 검색 키워드로 사용하여 브랜드 포털에서 이러한 이미지를 검색할 수 있습니다. 이 기능은 파일만 사용할 수 있습니다.

### 향상된 다운로드 환경 {#enhanced-downloading-experience}

중첩된 폴더를 다운로드한 후 원래 폴더 계층 구조를 유지할 수 있습니다. 중첩된 폴더 내의 에셋은 별도의 폴더가 아니라 단일 폴더에서 다운로드할 수 있습니다.

### 향상된 성능 {#improved-performance}

검색, 검색 및 다운로드 기능이 향상되어 브랜드 포털 성능이 크게 향상되었습니다.

### New digital rights management for assets {#new-digital-rights-management-for-assets}

관리자는 자산을 공유하기 전에 자산의 만료 날짜 및 시간을 설정할 수 있습니다. 에셋이 만료되면 뷰어 및 편집자는 볼 수 있지만 다운로드할 수는 없습니다. 자산이 만료되면 관리자는 알림을 받습니다.

### 향상된 에셋 정렬 {#enhanced-asset-sorting}

목록 보기의 폴더에서 자산 정렬이 더 이상 첫 번째 페이지에 표시되는 자산의 수로 제한되지 않습니다. 첫 번째 페이지에 모두 나열되는지 여부에 관계없이 폴더의 모든 자산이 정렬됩니다.

### 향상된 보고 {#reporting-capabilities}

관리자는 3가지 유형의 보고서(다운로드, 만료, 게시)를 만들고 관리할 수 있습니다. 보고서에서 열을 구성하고 보고서를 CSV 형식으로 내보내는 기능도 사용할 수 있습니다.

![](assets/newreport.png)

### 추가 메타데이터 {#additional-metadata}

브랜드 포털 6.3.1에서는 AEM Assets 6.3과 유사한 추가 메타데이터를 제공합니다. 스키마 편집기 양식을 사용하여 자산 속성 페이지에 표시되어야 하는 메타데이터를 제어할 수 있습니다. 에셋 메타데이터는 외부 링크 공유 사용자에게 보이지 않으므로 링크 공유 URL을 사용해서만 에셋을 미리 보고 다운로드할 수 있습니다.

![](assets/additionsinmetadata.png)

### 관리자를 위한 추가 기능 {#additional-capabilities-for-administrators}

* 로그인 화면 배경 무늬의 사용자 지정을 완료하기 전에 관리자가 변경 내용을 미리 볼 수 있습니다.

![](assets/wallpaperpreview.png)

* 관리자가 새 사용자를 추가하면 사용자가 브랜드 포털에 추가할 초대 이메일에 동의하지 않아도 자동으로 추가됩니다.

### AEM Assets 6.3의 새로운 게시 기능 {#new-publishing-capabilities-in-aem-assets}

* AEM 관리자는 2017년 4분기에 제공될 AEM 6.3 SP 1-CFP 1(6.3.1.1)을 사용하여 AEM Assets의 메타데이터 스키마를 브랜드 포털에 게시할 수 있습니다.

![](assets/publish_metadataschemaaemassets.png)

* AEM 관리자는 AEM 6.2 SP1-CFP7 및 AEM 6.3 SP 1-CFP 1(6.3.1.1)을 사용하여 AEM Assets의 모든 태그를 브랜드 포털에 게시할 수 있습니다.

![](assets/publish_tags_aemassets.png)

* AEM Assets에서 스마트 태그를 비롯한 태그가 있는 자산 및 컬렉션을 게시할 수 있습니다. 그런 다음 브랜드 포털에서 이러한 태그를 검색 키워드로 사용하여 이러한 자산이나 컬렉션을 검색할 수 있습니다.