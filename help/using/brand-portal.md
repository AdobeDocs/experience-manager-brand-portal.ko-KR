---
title: AEM Assets Brand Portal 개요
seo-title: AEM Assets Brand Portal 개요
description: AEM Assets Brand Portal을 사용하면 승인된 크리에이티브 자산을 외부 사용자와 내부 비즈니스 사용자가 간편하게 구매하고 제어하며 장치 간에 안전하게 분배할 수 있습니다.
seo-description: AEM Assets Brand Portal을 사용하면 승인된 크리에이티브 자산을 외부 사용자와 내부 비즈니스 사용자가 간편하게 구매하고 제어하며 장치 간에 안전하게 분배할 수 있습니다.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
exl-id: 0f2c45e4-416e-451a-905b-06c5e42a9272
source-git-commit: d2bfd06f8cd8a9e78efbc8dd92880e0faae39176
workflow-type: tm+mt
source-wordcount: '1554'
ht-degree: 7%

---

# AEM Assets Brand Portal 개요 {#overview-of-aem-assets-brand-portal}

마케터는 경우에 따라 채널 파트너 및 내부 비즈니스 사용자와 협력하여 관련 디지털 컨텐츠를 신속하게 작성, 관리 및 고객에게 전달해야 합니다. 전체 고객 여정에서 관련 컨텐츠를 적시에 제공하는 것은 더 많은 수요, 전환, 참여 및 고객 충성도를 높이는 데 매우 중요합니다.

그러나 승인된 브랜드 로고, 지침, 캠페인 자산 또는 제품 샷을 확장 내부 팀, 파트너 및 리셀러와 효율적이고 안전하게 공유하는 것을 지원하는 솔루션을 개발하는 것은 매우 어렵습니다.

**Adobe Experience Manager(AEM) Assets Brand** Portal은 자산 분배 및 자산 기여 기능을 제공하여 전체적으로 배포된 Brand Portal 사용자와 효과적으로 공동 작업해야 하는 마케터의 요구 사항에 중점을 둡니다.

자산 배포를 사용하면 승인된 크리에이티브 자산을 외부 사용자와 내부 비즈니스 사용자가 간편하게 구매하고 제어하며 장치 간에 안전하게 분배할 수 있습니다. 반면에, 자산 기여 기능을 사용하면 Brand Portal 사용자가 작성 환경에 액세스하지 않아도 자산을 Brand Portal에 업로드하고 AEM Assets에 게시할 수 있습니다. 기여도 기능은 Brand Portal **에서**자산 소싱이라고 합니다. 또한 Brand Portal 사용자(외부 에이전시/팀)의 자산 분배 및 기여에 대한 전반적인 Brand Portal 경험을 향상하고 자산의 출시 시간을 가속화하고, 규정 준수 및 무단 액세스의 위험을 감소시킵니다.
Brand Portal](brand-portal-asset-sourcing.md)의 [자산 소싱을 참조하십시오.

브라우저 기반 포털 환경을 사용하면 승인된 형식으로 자산을 쉽게 업로드, 탐색, 검색, 미리 보기 및 내보낼 수 있습니다.

## Brand Portal로 AEM Assets 구성 {#configure-brand-portal}

Brand Portal과 Adobe Experience Manager Assets를 구성하면 Brand Portal 사용자에 대한 자산 게시, 자산 분배 및 자산 기여 기능이 활성화됩니다.

>[!NOTE]
>
>AEM Assets as a Cloud Service, AEM Assets 6.3 이상에서 Brand Portal으로 AEM Assets을 구성할 수 있습니다.

AEM Assets as a Cloud Service은 Cloud Manager에서 Brand Portal을 활성화하여 Brand Portal으로 자동으로 구성됩니다. 활성화 워크플로우는 백엔드에 필수 구성을 만들고 Cloud Service 인스턴스로 AEM Assets과 동일한 IMS 조직에서 Brand Portal을 활성화합니다.

반면, AEM Assets(온-프레미스 및 관리 서비스)는 Brand Portal 테넌트의 인증을 위해 IMS(Adobe Identity Management Services) 토큰을 전달하는 Adobe 개발자 콘솔을 사용하여 Brand Portal으로 수동으로 구성합니다.

자세한 내용은 [Brand Portal에서 AEM Assets 구성](../using/configure-aem-assets-with-brand-portal.md)을 참조하십시오.

## Brand Portal의 사용자 성향 {#Personas}

Brand Portal은 다음 사용자 역할을 지원합니다.

* 게스트 사용자
* 뷰어
* 편집자
* 관리자

다음 표에는 이러한 역할의 사용자가 수행할 수 있는 작업이 나열되어 있습니다.

|  | **찾아보기** | **검색** | **다운로드** | **폴더 공유** | **컬렉션 공유** | **링크로 자산 공유** | **관리 도구에 액세스** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **게스트 사용자** | ✓* | ✓* | ✓* | x | x | x | x |
| **뷰어** | ✓ | ✓ | ✓ | x | x | x | x |
| **편집자** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **관리자** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

* 게스트 사용자는 공용 폴더 및 컬렉션에서만 자산을 검색, 액세스 및 검색할 수 있습니다.

<!--
&#42; Viewer users can access and download the public assets shared with them, and can add these assets to create their own collections.

>[!NOTE]
>
>There is a known issue that the share link for collections is currently visible to the viewer users. The viewer users does not have the privilege to add users to create a share link. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.
-->

### 게스트 사용자 {#guest-user}

인증을 받지 않은 Brand Portal의 자산에 대한 액세스 권한이 제한된 사용자는 게스트 사용자입니다. 게스트 세션을 통해 공용 폴더 및 컬렉션에 액세스할 수 있습니다. 게스트 사용자는 자산 세부 사항을 탐색하고 공용 폴더 및 컬렉션 구성원의 전체 자산 보기를 가질 수 있습니다. 공개 자산을 검색, 다운로드 및 [!UICONTROL Lightbox] 컬렉션에 추가할 수 있습니다.

그러나 게스트 세션에서는 컬렉션과 저장된 검색을 만들지 못하고 추가로 공유할 수 없습니다. 게스트 세션의 사용자는 폴더 및 컬렉션 설정에 액세스할 수 없으며 자산을 링크로 공유할 수 없습니다. 다음은 게스트 사용자가 수행할 수 있는 작업 목록입니다.

[공개 자산 찾아보기 및 액세스](browse-assets-brand-portal.md)

[공개 자산 검색](brand-portal-searching.md)

[공개 자산 다운로드](brand-portal-download-assets.md)

[[!UICONTROL Lightbox]에 자산 추가](brand-portal-light-box.md#add-assets-to-lightbox)

### 뷰어 {#viewer}

Brand Portal의 표준 사용자는 일반적으로 뷰어 역할을 가진 사용자입니다. 이 역할을 가진 사용자는 허용된 폴더, 컬렉션 및 자산에 액세스할 수 있습니다. 또한 자산(원본 또는 특정 표현물)을 검색, 미리 보기, 다운로드 및 내보내고, 계정 설정을 구성하고, 자산을 검색할 수도 있습니다. 다음은 뷰어가 수행할 수 있는 작업 목록입니다.

[자산 찾아보기](browse-assets-brand-portal.md)

[자산 검색](brand-portal-searching.md)

[자산 다운로드](brand-portal-download-assets.md)

### 편집자 {#editor}

편집자 역할을 가진 사용자는 뷰어가 수행할 수 있는 모든 작업을 수행할 수 있습니다. 또한 및 편집기는 관리자가 공유하는 파일과 폴더를 볼 수 있습니다. 편집자 역할을 가진 사용자는 다른 사용자와 컨텐츠(파일, 폴더, 컬렉션)를 공유할 수도 있습니다.

편집자는 뷰어가 수행할 수 있는 작업 외에도 다음과 같은 추가 작업을 수행할 수 있습니다.

[폴더 공유](brand-portal-sharing-folders.md)

[컬렉션 공유](brand-portal-share-collection.md)

[링크로 자산 공유](brand-portal-link-share.md)

### 관리자 {#administrator}

관리자는 [!UICONTROL Admin Console]에서 시스템 관리자 또는 Brand Portal 제품 관리자로 표시된 사용자를 포함합니다. 관리자는 시스템 관리자와 사용자를 추가 및 제거하고, 사전 설정을 정의하고, 사용자에게 이메일을 보내고, 포털 사용량 및 저장소 보고서를 볼 수 있습니다.

관리자는 편집기에서 다음과 같은 추가 작업을 수행할 수 있는 모든 작업을 수행할 수 있습니다.

[사용자, 그룹 및 사용자 역할 관리](brand-portal-adding-users.md)

[월페이퍼, 페이지 헤더 및 이메일 사용자 정의](brand-portal-branding.md)

[사용자 정의 검색 패싯 사용](brand-portal-search-facets.md)

[메타데이터 스키마 양식 사용](brand-portal-metadata-schemas.md)

[이미지 사전 설정 또는 동적 변환 적용](brand-portal-image-presets.md)

[보고서를 사용한 작업](brand-portal-reports.md)

위의 작업 외에 AEM Assets의 작성자는 다음 작업을 수행할 수 있습니다.

[Brand Portal에서 AEM Assets 구성](../using/configure-aem-assets-with-brand-portal.md)

[폴더를 Brand Portal에 게시](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-folder.html)

[컬렉션을 Brand Portal에 게시](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-collection.html)

## Brand Portal url {#tenant-alias-for-portal-url}에 대한 대체 별칭

Brand Portal 6.4.3 이상에서 조직은 Brand Portal 임차인의 기존 URL에 대해 하나의 대체(별칭) URL을 가질 수 있습니다. 별칭 URL은 URL에 대체 접두사가 있어 만들 수 있습니다.\
Brand Portal URL의 접두사만 사용자 지정할 수 있으며 전체 URL은 사용자 지정할 수 없습니다. 예를 들어 기존 도메인 **[!UICONTROL geometritrix.brand-portal.adobe.com]**&#x200B;이 있는 조직은 요청 시 **[!UICONTROL geometrixx.brand-portal.adobe.com]**&#x200B;을 만들 수 있습니다.

그러나 AEM 작성자 인스턴스는 테넌트 ID가 없고 임차인 별칭(대체) URL이 없는 [구성된](../using/configure-aem-assets-with-brand-portal.md)일 수 있습니다.

>[!NOTE]
>
>기존 포털 URL에서 테넌트 이름에 대한 별칭을 가져오려면 조직이 새 테넌트 별칭 생성 요청을 통해 Adobe 지원에 문의해야 합니다. 이 요청은 먼저 별칭을 사용할 수 있는지 확인한 다음 별칭을 만들어 처리됩니다.
>
>이전 별칭을 바꾸거나 이전 별칭을 삭제하려면 동일한 프로세스를 수행해야 합니다.

## Brand Portal {#request-access-to-brand-portal}에 대한 액세스 요청

사용자는 로그인 화면에서 Brand Portal에 대한 액세스를 요청할 수 있습니다. 이러한 요청은 Brand Portal 관리자에게 전송되며, 이 관리자는 Adobe [!UICONTROL Admin Console]을 통해 사용자에게 액세스 권한을 부여합니다. 액세스 권한이 부여되면 사용자는 알림 이메일을 받게 됩니다.

액세스를 요청하려면 다음을 수행하십시오.

1. Brand Portal 로그인 페이지에서 **[!UICONTROL 여기]**&#x200B;를 클릭하여 **[!UICONTROL 액세스 필요?]**. 그러나 게스트 세션을 입력하려면 **[!UICONTROL 게스트 액세스?]**&#x200B;에 해당하는 **[!UICONTROL 여기를 클릭]**&#x200B;을 선택하십시오.

   ![Brand Portal 로그인 화면](assets/bp-login-requestaccess.png)

   [!UICONTROL 액세스 요청] 페이지가 열립니다.

1. 조직의 Brand Portal에 대한 액세스를 요청하려면 유효한 [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID] 또는 [!UICONTROL Federated ID]이 있어야 합니다.

   [!UICONTROL 액세스 요청] 페이지에서 ID(시나리오 1)를 사용하여 로그인하거나 [!UICONTROL Adobe ID](시나리오 2):<br />
   ![[!UICONTROL 액세스 요청]](assets/bplogin_request_access_2.png)

   **시나리오 1**
   1. [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID] 또는 [!UICONTROL Federated ID]가 있는 경우 **[!UICONTROL 로그인]**을 클릭합니다.
[!UICONTROL 로그인] 페이지가 열립니다.
   1. [!UICONTROL Adobe ID] 자격 증명을 입력하고 **[!UICONTROL 로그인]**.<br />

   ![Adobe 로그인](assets/bplogin_request_access_3.png)

   [!UICONTROL 액세스 요청] 페이지로 리디렉션됩니다.<br />
   **시나리오 2**
   1. [!UICONTROL Adobe ID]이 없는 경우 만들려면 [!UICONTROL 액세스 요청] 페이지에서 **[!UICONTROL Adobe ID]**을 클릭하십시오.
[!UICONTROL 로그인] 페이지가 열립니다.
   1. **[!UICONTROL Adobe ID 가져오기]**를 클릭합니다.
[!UICONTROL 등록] 페이지가 열립니다.
   1. 이름과 성, 이메일 ID 및 암호를 입력합니다.
   1. **[!UICONTROL 등록]**.<br />을 선택합니다.

   ![](assets/bplogin_request_access_5.png)

   [!UICONTROL 액세스 요청] 페이지로 리디렉션됩니다.

1. 다음 페이지에는 액세스를 요청하는 데 사용된 이름과 이메일 ID가 표시됩니다. 관리자의 설명을 그대로 두고 **[!UICONTROL Submit]**.<br />

   ![](assets/bplogin-request-access.png)

## 제품 관리자는 액세스 권한 {#grant-access-to-brand-portal} 부여

Brand Portal 제품 관리자는 받은 편지함에서 Brand Portal 알림 영역 및 이메일을 통해 액세스 요청을 받습니다.

![액세스 요청 알림](assets/bplogin_request_access_7.png)

액세스 권한을 부여하려면 제품 관리자가 Brand Portal 알림 영역에서 관련 알림을 클릭한 다음 **[!UICONTROL 액세스 권한 부여]**를 클릭해야 합니다.
또는 제품 관리자는 액세스 요청 이메일에 제공된 링크에 따라 Adobe [!UICONTROL Admin Console]을 방문하여 사용자를 관련 제품 구성에 추가할 수 있습니다.

[Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) 홈 페이지로 리디렉션됩니다. 사용자를 만들고 제품 프로필(이전의 제품 구성)에 할당하려면 Adobe [!UICONTROL Admin Console]을 사용하여 Brand Portal의 그룹으로 표시됩니다. [!UICONTROL Admin Console]에서 사용자를 추가하는 방법에 대한 자세한 내용은 [사용자 추가](brand-portal-adding-users.md#add-a-user)를 참조하십시오(사용자를 추가하려면 절차에서 4-7단계를 수행).

## Brand Portal 언어 {#brand-portal-language}

Adobe [!UICONTROL Experience Cloud 설정]에서 Brand Portal 언어를 변경할 수 있습니다.

![액세스 요청 알림](assets/BPLang.png)

언어를 변경하려면 다음을 수행하십시오.

1. 상단 메뉴에서 [!UICONTROL 사용자] > [!UICONTROL 프로필 편집]을 선택합니다.<br />

   ![프로필 편집](assets/EditBPProfile.png)

1. [!UICONTROL Experience Cloud 설정] 페이지의 [!UICONTROL 언어] 드롭다운 메뉴에서 언어를 선택합니다.

## Brand Portal 유지 관리 알림 {#brand-portal-maintenance-notification}

Brand Portal을 유지 보수 목적으로 아래로 이동하도록 예약하기 전에 Brand Portal에 로그인한 후 알림이 배너로 표시됩니다. 샘플 알림:

![](assets/bp_maintenance_notification.png)

이 알림을 취소하고 Brand Portal을 계속 사용할 수 있습니다. 이 알림은 모든 새 세션에 표시됩니다.

## 릴리스 및 시스템 정보 {#release-and-system-information}

* [새로운 기능](whats-new.md)
* [릴리스 노트](brand-portal-release-notes.md)
* [지원되는 파일 형식](brand-portal-supported-formats.md)

## 관련 리소스 {#related-resources}

* [고객 지원 Adobe](https://helpx.adobe.com/kr/marketing-cloud/contact-support.html)
* [AEM 포럼](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community)
