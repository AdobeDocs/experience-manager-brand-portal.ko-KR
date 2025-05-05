---
title: Experience Manager Assets Brand Portal 개요
description: Experience Manager Assets Brand Portal을 통해 승인된 Creative Assets를 외부 당사자와 내부 비즈니스 사용자에게 여러 장치를 통해 손쉽게 확보하고 제어하고 안전하게 배포하는 방법에 대해 알아봅니다.
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
exl-id: 0f2c45e4-416e-451a-905b-06c5e42a9272
source-git-commit: 86585e7e04a19f59f9594409e6d7704f457ab8e2
workflow-type: tm+mt
source-wordcount: '1622'
ht-degree: 4%

---

# Experience Manager Assets Brand Portal 개요 {#overview-of-aem-assets-brand-portal}

마케터는 채널 파트너 및 내부 비즈니스 사용자와 협력하여 관련 디지털 콘텐츠를 생성하고, 관리하고, 고객에게 신속하게 전달해야 하는 경우가 있습니다. 전체 고객 여정에서 관련 콘텐츠를 적시에 전달하는 것은 더 많은 수요, 전환, 참여 및 고객 충성도를 이끄는 데 중요합니다.

그러나 승인된 브랜드 로고, 캠페인 자산 또는 제품 샷과 같은 것을 팀, 파트너 및 리셀러와 효율적이고 안전하게 공유할 수 있도록 지원하는 솔루션 개발은 어려운 과제입니다. 이 프로세스에서 효율성과 보안을 모두 보장하려면 신중한 계획과 실행이 필요합니다.

**Adobe Experience Manager(AEM) Assets Brand Portal**&#x200B;은(는) 자산 배포 및 자산 기여 기능을 제공하여 전 세계에 배포된 Brand Portal 사용자와 효과적으로 공동 작업해야 하는 마케터의 요구에 중점을 둡니다.

Asset distribution을 사용하면 승인된 크리에이티브 에셋을 획득, 제어하고, 장치 간에 외부 관련자와 내부 비즈니스 사용자에게 안전하게 배포할 수 있습니다. 그러나 에셋 기여를 통해 Brand Portal 사용자는 작성 환경에 액세스하지 않아도 에셋을 Brand Portal에 업로드하고 Experience Manager Assets에 게시할 수 있습니다. 기여 기능을 **Brand Portal의 Assets 소싱**&#x200B;이라고 합니다. 또한 이를 함께 사용하면 Brand Portal 사용자(외부 에이전시/팀)의 자산 배포 및 기여에 대한 전반적인 Brand Portal 경험을 개선할 수 있고, 자산 출시 시기를 앞당길 수 있으며, 규정 미준수 및 무단 액세스의 위험을 줄일 수 있습니다.
[Brand Portal의 자산 소싱](brand-portal-asset-sourcing.md)을 참조하세요.

브라우저 기반 포털 환경을 사용하면 승인된 형식으로 에셋을 쉽게 업로드, 찾아보기, 검색, 미리 보기 및 내보낼 수 있습니다.

## Brand Portal로 Experience Manager Assets 구성 {#configure-brand-portal}

Brand Portal과 함께 Adobe Experience Manager Assets을 구성하면 Brand Portal 사용자에게 자산 게시, 자산 배포 및 자산 기여 기능이 활성화됩니다.

>[!NOTE]
>
>Brand Portal을 사용하여 Experience Manager Assets을 구성하는 기능은 Experience Manager Assets as a Cloud Service, Experience Manager Assets 6.3 이상에서 지원됩니다.

Experience Manager Assets as a Cloud Service은 Cloud Manager에서 Brand Portal을 활성화하여 Brand Portal에 자동으로 구성됩니다. 활성화 워크플로우는 백엔드에서 필요한 구성을 만들고 Experience Manager Assets as a Cloud Service 인스턴스와 동일한 IMS 조직에서 Brand Portal을 활성화합니다.

하지만 Experience Manager Assets(온 프레미스 및 관리 서비스)는 Brand Portal 테넌트의 인증을 위해 Adobe Identity Management IMS(Services) 토큰을 전달하는 Adobe Developer Console을 사용하여 Brand Portal으로 수동으로 구성합니다.

자세한 내용은 [Brand Portal을 사용하여 Experience Manager Assets 구성](../using/configure-aem-assets-with-brand-portal.md)을 참조하십시오.

## Brand Portal의 사용자 담당자 {#Personas}

Brand Portal은 다음 사용자 역할을 지원합니다.

* 게스트 사용자
* 뷰어
* 편집기
* 관리자

다음 표에는 이러한 역할의 사용자가 수행할 수 있는 작업이 나열되어 있습니다.

|  | **찾아보기** | **검색** | **다운로드** | **폴더 공유** | **컬렉션 공유** | **링크로 자산 공유** | **관리 도구에 액세스** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **게스트 사용자** | ✓* | ✓* | ✓* | x | x | x | x |
| **뷰어** | ✓ | ✓ | ✓ | x | x | x | x |
| **편집기** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **관리자** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

>[!NOTE]
>
>게스트 사용자는 공용 폴더 및 컬렉션에서만 에셋을 찾아보고, 액세스하고, 검색할 수 있습니다.

<!--
&#42; Viewer users can access and download the public assets shared with them, and can add these assets to create their own collections.

>[!NOTE]
>
>There is a known issue that the share link for collections is currently visible to the viewer users. The viewer users does not have the privilege to add users to create a share link. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.
-->

### 게스트 사용자 {#guest-user}

Experience Manager Assets Brand Portal에서 [게스트가 Brand Portal에 액세스](#request-access-to-brand-portal)할 수 있습니다. 게스트 사용자는 포털에 로그인하기 위해 자격 증명이 필요하지 않으며 공용 폴더 및 컬렉션에 액세스할 수 있습니다. 게스트 사용자는 에셋 세부 사항을 탐색하고 공개 폴더 및 컬렉션의 멤버에 대한 전체 에셋 보기를 가질 수 있습니다. 공개 자산을 검색 및 다운로드하고 [!UICONTROL Lightbox] 컬렉션에 추가할 수 있습니다.

그러나 게스트 세션에서는 컬렉션 및 저장된 검색을 만들 수 없도록 제한하고 추가로 공유합니다. 게스트 세션의 사용자는 폴더 및 컬렉션 설정에 액세스할 수 없으며 링크로 에셋을 공유할 수 없습니다. 다음은 게스트 사용자가 수행할 수 있는 작업 목록입니다.

* [공개 에셋 검색 및 액세스](browse-assets-brand-portal.md)

* [공개 에셋 검색](brand-portal-searching.md)

* [공개 에셋 다운로드](brand-portal-download-assets.md)

* [[!UICONTROL Lightbox]에 자산 추가](brand-portal-light-box.md#add-assets-to-lightbox)

자세한 내용을 보려면 [Brand Portal에 대한 게스트 액세스](../using/guest-access.md)(으)로 이동하십시오.

### 뷰어 {#viewer}

[!DNL Admin Console]에서 정의되었으며 Viewer 역할로 Brand Portal에 액세스할 수 있는 Brand Portal 사용자입니다. 이 역할을 가진 사용자는 Brand Portal에 로그인하여 허용된 폴더, 컬렉션 및 에셋에 액세스할 수 있습니다. 또한 에셋(원본 또는 특정 렌디션)을 검색, 미리 보기, 다운로드 및 내보내고, 계정 설정을 구성하고, 에셋을 검색할 수 있습니다. 다음은 뷰어에서 수행할 수 있는 작업 목록입니다.

* [에셋 찾아보기](browse-assets-brand-portal.md)

* [에셋 검색](brand-portal-searching.md)

* [자산 다운로드](brand-portal-download-assets.md)

### 편집기 {#editor}

편집기 역할을 가진 사용자는 뷰어가 수행할 수 있는 모든 작업을 수행할 수 있습니다. 또한 편집기는 관리자가 공유하는 파일 및 폴더를 볼 수 있습니다. 편집기 역할을 가진 사용자는 다른 사용자와 컨텐츠(파일, 폴더, 컬렉션)를 공유할 수도 있습니다.

뷰어가 수행할 수 있는 작업 외에도 편집기는 다음과 같은 추가 작업을 수행할 수 있습니다.

* [폴더 공유](brand-portal-sharing-folders.md)

* [컬렉션 공유](brand-portal-share-collection.md)

* [링크로 자산 공유](brand-portal-link-share.md)

### 관리자 {#administrator}

관리자가 [!UICONTROL Admin Console]에서 시스템 관리자 또는 Brand Portal 제품 관리자로 표시된 사용자를 포함합니다. 관리자는 시스템 관리자와 사용자를 추가 및 제거하고, 사전 설정을 정의하고, 사용자에게 이메일을 보내고, 포털 사용 및 저장소 보고서를 볼 수 있습니다.

>[!NOTE]
>
>Brand Portal에서 [!UICONTROL Admin Console]에서 지원 관리자 역할로 표시된 사용자는 시스템 관리자와 동일한 권한을 갖습니다.

관리자는 편집기가 수행할 수 있는 모든 작업을 수행할 수 있습니다. 다음은 관리자가 수행할 수 있는 추가 작업입니다.

* [사용자, 그룹 및 사용자 역할 관리](brand-portal-adding-users.md)
* [배경 무늬, 페이지 헤더 및 이메일 사용자 지정](brand-portal-branding.md)
* [사용자 정의 검색 패싯 사용](brand-portal-search-facets.md)
* [메타데이터 스키마 사용](brand-portal-metadata-schemas.md)
* [이미지 사전 설정 또는 동적 변환 적용](brand-portal-image-presets.md)
* [보고서 작업](brand-portal-reports.md)

위의 작업 외에도 AEM Assets의 작성자는 다음 작업을 수행할 수 있습니다.

* [Brand Portal에서 AEM Assets 구성](../using/configure-aem-assets-with-brand-portal.md)
* [폴더를 Brand Portal에 게시](https://experienceleague.adobe.com/ko/docs/experience-manager-65/content/assets/brandportal/brand-portal-publish-folder)
* [컬렉션을 Brand Portal에 게시](https://experienceleague.adobe.com/ko/docs/experience-manager-65/content/assets/brandportal/brand-portal-publish-collection)

## Brand Portal URL에 대한 대체 별칭 {#tenant-alias-for-portal-url}

Brand Portal 6.4.3 이상에서 조직은 Brand Portal 테넌트의 각 기존 URL에 대해 하나의 대체(별칭) URL을 가질 수 있습니다. 별칭 URL은 URL에 대체 접두사를 사용하여 만들 수 있습니다.\
테넌트 이름이 32자를 초과하는 경우 테넌트 별칭을 만들어야 합니다.
Brand Portal URL의 접두사만 사용자 정의할 수 있으며 전체 URL은 사용자 정의할 수 없습니다. 예를 들어 기존 도메인이 `geomettrix.brand-portal.adobe.com`인 조직은 요청 시 `geomettrixinc.brand-portal.adobe.com`을(를) 만들 수 있습니다.

그러나 AEM 작성자 인스턴스는 테넌트 별칭(대체) URL이 아닌 테넌트 ID URL로만 [구성](../using/configure-aem-assets-with-brand-portal.md)될 수 있습니다.

>[!NOTE]
>
>기존 포털 URL에서 테넌트 이름에 대한 별칭을 얻으려면 조직에서 새 테넌트 별칭 만들기 요청을 사용하여 고객 지원 센터에 문의해야 합니다. 먼저 별칭을 사용할 수 있는지 확인한 다음 이 요청을 처리할 별칭을 만듭니다.
>
>이전 별칭을 바꾸거나 삭제하려면 동일한 프로세스를 따라야 합니다.

## Brand Portal 액세스 요청 {#request-access-to-brand-portal}

사용자는 로그인 화면에서 Brand Portal 액세스를 요청할 수 있습니다. 이러한 요청은 Brand Portal 관리자에게 전송되며, 관리자는 Adobe [!UICONTROL Admin Console]을(를) 통해 사용자에게 액세스 권한을 부여합니다. 액세스 권한이 부여되면 사용자에게 알림 이메일이 전송됩니다.

액세스 권한을 요청하려면 다음을 수행하십시오.

1. Brand Portal 로그인 페이지에서 **[!UICONTROL 액세스 필요 여부에 해당하는**&#x200B;[!UICONTROL &#x200B;여기를 클릭&#x200B;]&#x200B;**을 선택합니다.]**. 그러나 게스트 세션을 시작하려면 **[!UICONTROL 게스트 액세스?]**&#x200B;에 해당하는 **[!UICONTROL 여기를 클릭]**&#x200B;하세요.

   ![Brand Portal 로그인 화면](assets/bp-login-requestaccess.png)

   [!UICONTROL 액세스 요청] 페이지가 열립니다.

1. 조직의 Brand Portal에 대한 액세스를 요청하려면 유효한 [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID] 또는 [!UICONTROL Federated ID]이(가) 있어야 합니다.

   [!UICONTROL 액세스 요청] 페이지에서 ID를 사용하여 로그인하거나(시나리오 1) [!UICONTROL Adobe ID]&#x200B;(시나리오 2)을(를) 만듭니다.

   ![[!UICONTROL 액세스 요청]](assets/bplogin_request_access_2.png)

   **시나리오 1**

   1. [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID] 또는 [!UICONTROL Federated ID]이 있는 경우 **[!UICONTROL 로그인]**&#x200B;을 클릭하세요.
[!UICONTROL 로그인] 페이지가 열립니다.

   1. [!UICONTROL Adobe ID] 자격 증명을 제공하고 **[!UICONTROL 로그인]**&#x200B;을 클릭합니다.

      ![Adobe 로그인](assets/bplogin_request_access_3.png)

   [!UICONTROL 액세스 요청] 페이지로 리디렉션되었습니다.

   **시나리오 2**

   1. [!UICONTROL Adobe ID]이 없는 경우 새로 만들려면 [!UICONTROL 액세스 요청] 페이지에서 **[!UICONTROL Adobe ID 가져오기]**&#x200B;를 클릭하세요.
[!UICONTROL 로그인] 페이지가 열립니다.
   1. **[!UICONTROL Adobe ID 가져오기]**&#x200B;를 클릭합니다.
[!UICONTROL 등록] 페이지가 열립니다.
   1. 이름과 성, 이메일 ID 및 암호를 입력합니다.
   1. **[!UICONTROL 등록]**&#x200B;을 선택하세요.

      ![](assets/bplogin_request_access_5.png)

   [!UICONTROL 액세스 요청] 페이지로 리디렉션되었습니다.

1. 다음 페이지에는 액세스를 요청하는 데 사용되는 이름과 이메일 ID가 표시됩니다. 관리자에게 댓글을 남겨 주고 **[!UICONTROL 제출]**&#x200B;을 클릭하세요.

   ![](assets/bplogin-request-access.png)

## 제품 관리자 액세스 권한 부여 {#grant-access-to-brand-portal}

Brand Portal 제품 관리자는 자신의 Brand Portal 알림 영역과 받은 편지함의 이메일을 통해 액세스 요청을 받습니다.

![요청된 알림에 액세스](assets/bplogin_request_access_7.png)

액세스 권한을 부여하려면 제품 관리자가 Brand Portal 알림 영역에서 관련 알림을 클릭한 다음 **[!UICONTROL 액세스 권한 부여]**&#x200B;를 클릭해야 합니다.
또는 제품 관리자는 액세스 요청 이메일에 제공된 링크를 따라 Adobe [!UICONTROL Admin Console]을(를) 방문하여 사용자를 관련 제품 구성에 추가할 수 있습니다.

[Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) 홈 페이지로 리디렉션되었습니다. Adobe [!UICONTROL Admin Console]을(를) 사용하여 사용자를 만들고 Brand Portal에 그룹으로 표시되는 제품 프로필(이전의 제품 구성)에 사용자를 할당합니다. [!UICONTROL Admin Console]에서 사용자를 추가하는 방법에 대한 자세한 내용은 [사용자 추가](brand-portal-adding-users.md#add-a-user)를 참조하십시오(사용자 추가 절차의 4-7단계).

## Brand Portal 언어 {#brand-portal-language}

Adobe [!UICONTROL Experience Cloud 설정]에서 Brand Portal 언어를 변경할 수 있습니다.

![요청된 알림에 액세스](assets/BPLang.png)

언어를 변경하려면:

1. 상단 메뉴에서 [!UICONTROL 사용자] > [!UICONTROL 프로필 편집]을 선택합니다.

   ![프로필 편집](assets/EditBPProfile.png)

1. [!UICONTROL Experience Cloud 설정] 페이지의 [!UICONTROL 언어] 드롭다운 메뉴에서 언어를 선택합니다.

## Brand Portal 유지 관리 알림 {#brand-portal-maintenance-notification}

Brand Portal이 유지 관리를 위해 다운되도록 예약되기 전에 Brand Portal에 로그인하면 알림이 배너로 표시됩니다. 샘플 알림:

![](assets/bp_maintenance_notification.png)

이 알림을 무시하고 Brand Portal을 계속 사용할 수 있습니다. 이 알림은 모든 새 세션에 표시됩니다.

## 릴리스 및 시스템 정보 {#release-and-system-information}

* [새로운 기능](whats-new.md)
* [릴리스 정보](brand-portal-release-notes.md)
* [지원되는 파일 형식](brand-portal-supported-formats.md)

## 관련 리소스 {#related-resources}

<!--
* [Adobe Customer Support]()
-->

* [AEM 포럼](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community?profile.language=ko)
