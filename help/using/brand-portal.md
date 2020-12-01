---
title: AEM Assets 브랜드 포털 개요
seo-title: AEM Assets 브랜드 포털 개요
description: AEM Assets 브랜드 포털은 승인된 크리에이티브 자산을 손쉽게 확보, 제어 및 다양한 디바이스에서 외부 관계자와 내부 비즈니스 사용자에게 안전하게 배포할 수 있도록 지원합니다.
seo-description: AEM Assets 브랜드 포털은 승인된 크리에이티브 자산을 손쉽게 확보, 제어 및 다양한 디바이스에서 외부 관계자와 내부 비즈니스 사용자에게 안전하게 배포할 수 있도록 지원합니다.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
translation-type: tm+mt
source-git-commit: ecd53a7d92dd020e6a3527793ff11efadcb531ee
workflow-type: tm+mt
source-wordcount: '1524'
ht-degree: 10%

---


# AEM Assets 브랜드 포털 개요 {#overview-of-aem-assets-brand-portal}

마케터는 고객과 연관성 높은 디지털 컨텐츠를 신속하게 제작, 관리 및 전달하려면 채널 파트너 및 내부 비즈니스 사용자와 공동 작업해야 하는 경우가 있습니다. 고객 여정 전반에서 연관성 있는 콘텐츠를 적시에 전달하여 높은 수요, 전환율, 고객 참여, 고객 충성도 향상에 중요합니다.

그러나 승인된 브랜드 로고, 지침, 캠페인 자산 또는 제품 샷을 다양한 내부 팀, 파트너 및 리셀러와 효율적이고 안전하게 공유할 수 있는 솔루션을 개발하는 것은 매우 어려운 일입니다.

**Adobe Experience Manager(AEM) 자산 브랜드** 포털은 자산 배포 및 자산 기여도 기능을 제공함으로써 글로벌 배포된 브랜드 포털 사용자와 효과적으로 공동 작업해야 하는 마케터의 필요성에 중점을 둡니다.

에셋 배포를 사용하면 승인된 크리에이티브 자산을 손쉽게 확보, 제어 및 모든 디바이스에서 외부 관계자와 내부 비즈니스 사용자에게 안전하게 배포할 수 있습니다. 반면에 자산 기여도를 통해 브랜드 포털 사용자는 작성 환경에 액세스할 필요 없이 에셋을 브랜드 포털에 업로드하고 AEM Assets에 게시할 수 있습니다. 기여도 기능을 브랜드 포털의 **자산 소싱**이라고 합니다. 또한 브랜드 포털 사용자(외부 에이전시/팀)의 자산 배포 및 기여도에 대한 전반적인 브랜드 포털 경험을 향상시키고 자산 출시 시간을 단축하며, 규정 준수 및 무단 액세스 위험을 감소시킵니다.
브랜드 포털의 [자산 소싱 참조](brand-portal-asset-sourcing.md).

브라우저 기반의 포털 환경을 사용하면 승인된 포맷으로 에셋을 손쉽게 업로드, 탐색, 검색, 미리 보기 및 내보낼 수 있습니다.

## Brand Portal로 AEM Assets 구성 {#configure-brand-portal}

AEM(Adobe Experience Manager) Assets는 Brand Portal 테넌트의 인증을 위한 IMS 토큰을 조달하는 Adobe 개발자 콘솔을 통해 Brand Portal로 구성됩니다.

>[!NOTE]
>
>Adobe 개발자 콘솔을 통해 브랜드 포털에서 AEM Assets을 구성하는 것은 Cloud Service, AEM Assets 6.3 이상으로 AEM Assets에서 지원됩니다.

### 브랜드 포털 {#prerequisites}을(를) 사용하여 AEM Assets을 구성하는 사전 요구 사항

Brand Portal을 사용하여 AEM Assets를 구성하려면 다음 항목이 필요합니다.

* 실행 중인 AEM Assets 인스턴스.
* Brand Portal 테넌트 URL
* Brand Portal 테넌트의 IMS 조직에 대한 시스템 관리자 권한이 있는 사용자

자세한 내용은 [브랜드 포털](../using/configure-aem-assets-with-brand-portal.md)으로 AEM Assets 구성을 참조하십시오.

## 브랜드 포털의 사용자 개인{#Personas}

브랜드 포털은 다음 사용자 역할을 지원합니다.

* 손님 사용자
* 뷰어
* 편집자
* 관리자

다음 표에는 이러한 역할의 사용자가 수행할 수 있는 작업이 나와 있습니다.

|  | **찾아보기** | **검색** | **다운로드** | **폴더 공유** | **컬렉션 공유** | **링크로 자산 공유** | **관리 도구 액세스** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **손님 사용자** | ✓* | ✓* | ✓* | x | x | x | x |
| **뷰어** | ✓ | ✓ | ✓ | x | x | x | x |
| **편집자** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **관리자** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

* 게스트 사용자는 공개 폴더 및 컬렉션에서만 자산을 검색, 액세스 및 검색할 수 있습니다.

<!--
&#42; Viewer users can access and download the public assets shared with them, and can add these assets to create their own collections.

>[!NOTE]
>
>There is a known issue that the share link for collections is currently visible to the viewer users. The viewer users does not have the privilege to add users to create a share link. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.
-->

### 손님 사용자 {#guest-user}

인증을 받지 않고 브랜드 포털의 에셋에 대한 액세스 권한이 제한된 모든 사용자는 게스트 사용자입니다. 게스트 세션을 통해 공개 폴더 및 컬렉션에 액세스할 수 있습니다. 게스트 사용자는 자산 세부 사항을 탐색하고 공개 폴더 및 컬렉션 구성원에 대한 전체 자산 보기를 가질 수 있습니다. 공개 자산을 검색, 다운로드 및 [!UICONTROL Lightbox] 컬렉션에 추가할 수 있습니다.

그러나 게스트 세션에서는 컬렉션 및 저장된 검색을 만들 수 없으며 추가로 공유할 수 없습니다. 게스트 세션의 사용자는 폴더 및 컬렉션 설정에 액세스할 수 없으며 에셋을 링크로 공유할 수 없습니다. 손님 사용자가 수행할 수 있는 작업 목록은 다음과 같습니다.

[공개 에셋 검색 및 액세스](browse-assets-brand-portal.md)

[공개 자산 검색](brand-portal-searching.md)

[공개 에셋 다운로드](brand-portal-download-assets.md)

[Lightbox에 자산  [!UICONTROL 추가]](brand-portal-light-box.md#add-assets-to-lightbox)

### 뷰어 {#viewer}

브랜드 포털의 표준 사용자는 일반적으로 뷰어 역할을 가진 사용자입니다. 이 역할의 사용자는 허용된 폴더, 컬렉션 및 자산에 액세스할 수 있습니다. 또한 사용자는 자산(원본 또는 특정 변환)을 검색, 미리 보기, 다운로드 및 내보내고 계정 설정을 구성하고 자산을 검색할 수 있습니다. 다음은 뷰어가 수행할 수 있는 작업 목록입니다.

[자산 찾아보기](browse-assets-brand-portal.md)

[자산 검색](brand-portal-searching.md)

[자산 다운로드](brand-portal-download-assets.md)

### 편집자 {#editor}

편집자 역할을 가진 사용자는 뷰어에서 수행할 수 있는 모든 작업을 수행할 수 있습니다. 또한, 편집기는 관리자가 공유하는 파일과 폴더를 볼 수 있습니다. 편집자 역할을 가진 사용자는 다른 사람과 컨텐츠(파일, 폴더, 컬렉션)를 공유할 수도 있습니다.

뷰어에서 수행할 수 있는 작업 외에 편집기는 다음과 같은 추가 작업을 수행할 수 있습니다.

[폴더 공유](brand-portal-sharing-folders.md)

[컬렉션 공유](brand-portal-share-collection.md)

[링크로 자산 공유](brand-portal-link-share.md)

### 관리자 {#administrator}

관리자는 [!UICONTROL Admin Console]에 시스템 관리자 또는 브랜드 포털 제품 관리자로 표시된 사용자를 포함합니다. 관리자는 시스템 관리자와 사용자를 추가 및 제거하고 사전 설정을 정의하며 사용자에게 이메일을 보내고 포털 사용 및 저장소 보고서를 볼 수 있습니다.

관리자는 편집자가 다음과 같은 추가 작업을 수행할 수 있는 모든 작업을 수행할 수 있습니다.

[사용자, 그룹 및 사용자 역할 관리](brand-portal-adding-users.md)

[배경 무늬, 페이지 머리글 및 이메일 사용자 정의](brand-portal-branding.md)

[사용자 정의 검색 패싯 사용](brand-portal-search-facets.md)

[메타데이터 스키마 양식 사용](brand-portal-metadata-schemas.md)

[이미지 사전 설정 또는 동적 변환 적용](brand-portal-image-presets.md)

[보고서를 사용한 작업](brand-portal-reports.md)

위의 작업 외에 AEM Assets의 작성자는 다음 작업을 수행할 수 있습니다.

[Brand Portal로 AEM Assets 구성](../using/configure-aem-assets-with-brand-portal.md)

[폴더를 Brand Portal에 게시](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-folder.html)

[컬렉션을 Brand Portal에 게시](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-collection.html)

## 브랜드 포털 url {#tenant-alias-for-portal-url}에 대한 대체 별칭

브랜드 포털 6.4.3부터 조직은 브랜드 포털 테넌트의 기존 URL에 대해 하나의 대체(별칭) URL을 가질 수 있습니다. 별칭 URL은 URL에 대체 접두사가 있으면 만들 수 있습니다.\
브랜드 포털 URL의 접두사만 사용자 정의할 수 있으며 전체 URL은 사용자 지정할 수 없습니다. 예를 들어 기존 도메인 **[!UICONTROL geometritrix.brand-portal.adobe.com]**&#x200B;이 있는 조직은 요청에 따라 만들어진 **[!UICONTROL geometrixx.brand-portal.adobe.com]**&#x200B;을 가져올 수 있습니다.

그러나 AEM 작성자 인스턴스는 테넌트 ID를 가진 [configured](../using/configure-aem-assets-with-brand-portal.md)만 될 수 있고 테넌트 별칭(대체) URL에는 없을 수 있습니다.

>[!NOTE]
>
>기존 포털 URL에서 테넌트 이름에 대한 별칭을 얻으려면 조직은 새 테넌트 별칭 생성 요청으로 Adobe 지원에 문의해야 합니다. 이 요청은 우선 별칭이 사용 가능한지 확인한 다음 별칭을 만들어 처리됩니다.
>
>이전 별칭을 대체하거나 삭제하려면 동일한 프로세스를 따라야 합니다.

## 브랜드 포털 {#request-access-to-brand-portal}에 대한 액세스 요청

사용자는 로그인 화면에서 브랜드 포털에 대한 액세스 권한을 요청할 수 있습니다. 이러한 요청은 Adobe [!UICONTROL Admin Console]을 통해 사용자에게 액세스 권한을 부여하는 브랜드 포털 관리자에게 전송됩니다. 액세스 권한이 부여되면 사용자는 알림 이메일을 수신하게 됩니다.

액세스를 요청하려면 다음을 수행합니다.

1. 브랜드 포털 로그인 페이지에서 **[!UICONTROL 액세스 필요?]******. 그러나 게스트 세션에 입장하려면 **[!UICONTROL 손님 액세스?]**&#x200B;에 해당하는 **[!UICONTROL 여기를 클릭]**&#x200B;합니다.

   ![브랜드 포털 로그인 화면](assets/bp-login-requestaccess.png)

   [!UICONTROL 액세스 요청] 페이지가 열립니다.

1. 조직의 브랜드 포털에 대한 액세스를 요청하려면 유효한 [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID] 또는 [!UICONTROL Federated ID]이 있어야 합니다.

   [!UICONTROL 액세스 요청] 페이지에서 ID(시나리오 1)를 사용하여 로그인하거나 [!UICONTROL Adobe ID](시나리오 2)을 만듭니다.<br />
   ![[!UICONTROL 액세스 요청]](assets/bplogin_request_access_2.png)

   **시나리오 1**
   1. [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID] 또는 [!UICONTROL Federated ID]이 있는 경우 **[!UICONTROL 로그인]**을 클릭합니다.
[!UICONTROL 로그인] 페이지가 열립니다.
   1. [!UICONTROL Adobe ID] 자격 증명을 입력하고 **[!UICONTROL 로그인]**&#x200B;을 클릭합니다.<br />

   ![Adobe 로그인](assets/bplogin_request_access_3.png)

   [!UICONTROL 액세스 요청] 페이지로 리디렉션됩니다.<br />
   **시나리오 2**
   1. [!UICONTROL Adobe ID]이 없으면 **[!UICONTROL 액세스 요청] 페이지에서 &lt;a2/>Adobe ID]**을 클릭합니다.
[!UICONTROL 
[!UICONTROL 로그인] 페이지가 열립니다.
   1. **[!UICONTROL Adobe ID 가져오기]**를 클릭합니다.
[!UICONTROL 등록] 페이지가 열립니다.
   1. 이름과 성, 이메일 ID 및 암호를 입력합니다.
   1. **[!UICONTROL 등록]**&#x200B;을 선택합니다.<br />

   ![](assets/bplogin_request_access_5.png)

   [!UICONTROL 액세스 요청] 페이지로 리디렉션됩니다.

1. 다음 페이지에는 액세스 권한을 요청하는 데 사용한 이름 및 이메일 ID가 표시됩니다. 관리자의 주석을 그대로 두고 **[!UICONTROL 제출]**.<br />을 클릭합니다.

   ![](assets/bplogin-request-access.png)

## 제품 관리자가 {#grant-access-to-brand-portal} 액세스 권한을 부여합니다.

브랜드 포털 제품 관리자는 자신의 브랜드 포털 알림 영역과 받은 편지함에서 이메일을 통해 액세스 요청을 받습니다.

![액세스 요청 알림](assets/bplogin_request_access_7.png)

액세스 권한을 부여하려면 제품 관리자가 브랜드 포털 알림 영역에서 관련 알림을 클릭한 다음 **[!UICONTROL 액세스 권한 부여]**를 클릭해야 합니다.
또는 제품 관리자는 액세스 요청 이메일에 제공된 링크를 따라 Adobe [!UICONTROL Admin Console]을 방문하고 해당 사용자를 관련 제품 구성에 추가할 수 있습니다.

[Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) 홈 페이지로 리디렉션됩니다. Adobe [!UICONTROL Admin Console]을 사용하여 사용자를 만들고 제품 프로필(이전의 제품 구성)에 할당하여 브랜드 포털에서 그룹으로 표시합니다. [!UICONTROL Admin Console]에서 사용자를 추가하는 방법에 대한 자세한 내용은 [사용자](brand-portal-adding-users.md#add-a-user) 추가(사용자를 추가하는 절차의 4-7단계 참조)를 참조하십시오.

## 브랜드 포털 언어 {#brand-portal-language}

Adobe [!UICONTROL Experience Cloud 설정]에서 브랜드 포털 언어를 변경할 수 있습니다.

![액세스 요청 알림](assets/BPLang.png)

언어를 변경하려면 다음을 수행하십시오.

1. 상단 메뉴에서 [!UICONTROL 사용자] > [!UICONTROL 프로필 편집]을 선택합니다.<br />

   ![프로필 편집](assets/EditBPProfile.png)

1. [!UICONTROL Experience Cloud 설정] 페이지의 [!UICONTROL 언어] 드롭다운 메뉴에서 언어를 선택합니다.

## 브랜드 포털 유지 관리 알림 {#brand-portal-maintenance-notification}

유지 관리를 위해 브랜드 포털이 다운되도록 예약되기 전에 브랜드 포털에 로그인한 후 알림이 배너로 표시됩니다. 샘플 알림:

![](assets/bp_maintenance_notification.png)

이 알림을 무시하고 브랜드 포털을 계속 사용할 수 있습니다. 이 알림은 모든 새 세션에 표시됩니다.

## 릴리스 및 시스템 정보 {#release-and-system-information}

* [새로운 기능](whats-new.md)
* [릴리스 노트](brand-portal-release-notes.md)
* [지원되는 파일 형식](brand-portal-supported-formats.md)

## 관련 리소스 {#related-resources}

* [Adobe 고객 지원 센터](https://helpx.adobe.com/kr/marketing-cloud/contact-support.html)
* [AEM 포럼](https://www.adobe.com/go/aod_forums_en)