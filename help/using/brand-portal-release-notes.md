---
title: 릴리스 노트
seo-title: 릴리스 노트
description: Adobe Experience Manager Assets Brand Portal 6.4.6 릴리스의 기능, 개선 사항, 주요 문제 및 알려진 문제에 대한 통찰력을 얻을 수 있습니다.
seo-description: Adobe Experience Manager Assets Brand Portal 6.4.6 릴리스의 개선 사항, 중요 문제 및 알려진 문제에 대한 통찰력을 얻을 수 있습니다.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: e0aeb9a69c81add2d87463fc87d6d08ae57722b9

---


# 릴리스 노트 {#release-notes}

Adobe Experience Manager Assets Brand Portal 6.4.6 릴리스의 새로운 기능, 개선 사항, 주요 문제 및 알려진 문제에 대한 통찰력을 얻을 수 있습니다.

## 릴리스 정보 {#release-information}

| 제품 | Adobe Experience Manager Assets 브랜드 포털 |
|---|---|
| 버전 | 6.4.6 |
| 날짜 | 2020년 3월 |

## 개요 {#overview}

AEM(Adobe Experience Manager) 자산 브랜드 포털을 통해 승인된 크리에이티브 자산을 손쉽게 확보, 제어 및 장치 간 외부 사용자와 내부 비즈니스 사용자에게 안전하게 배포할 수 있습니다. 자산 공유의 효율성을 향상시키고 자산 출시 시간을 단축하며 규정 준수 및 무단 액세스 위험을 줄일 수 있습니다. 브랜드 포털을 통해 사용자는 언제 어디에서나 회사에서 승인한 포맷으로 에셋을 검색, 검색, 미리 보기, 다운로드 및 내보낼 수 있습니다.

## 6.4.6의 새로운 기능 {#what-s-new-in-646}

### 새로운 기능 {#new-feature}

이 릴리스에는 다음과 같은 새로운 기능이 포함됩니다.

* Captcha - Brand Portal에 게스트 로그인을 위한 것입니다. 자세한 내용은 [브랜드 포털 게스트 액세스를](../using/guest-access.md) 참조하십시오.

### 향상된 기능 {#enhancements-646}

이 브랜드 포털 릴리스에는 다음 개선 사항이 포함됩니다.

* 이제 AEM Assets는 Adobe I/O를 통해 브랜드 포털로 구성되며, 브랜드 포털 임차인의 승인을 위해 IMS 토큰을 조달합니다.

   >[!NOTE]
   >
   >기존 OAuth를 통한 구성은 2020년 4월 6일부터 더 이상 지원되지 않으며, Adobe I/O를 통해 구성으로 변경되었습니다.


>[!TIP]
>
>***기존 고객만 해당***
>
>기존 레거시 OAuth 게이트웨이 구성을 계속 사용하는 것이 좋습니다. 이전 OAuth 게이트웨이 구성에 문제가 있는 경우 기존 구성을 삭제하고 Adobe I/O를 통해 새 구성을 만드십시오.


자세한 내용은 브랜드 포털에서 [AEM 자산 구성을 참조하십시오.](configure-aem-assets-with-brand-portal.md)

### 해결된 중요한 문제 {#critical-issues-fixed}

이 릴리스에는 다음과 같은 중요한 문제가 수정되었습니다.

* 메타데이터 스키마 드롭다운 값은 자산 속성에 표시되지 않습니다.

* 메타데이터 하위 스키마는 자산 속성의 MIMETYPE에 따라 탭을 표시하지 않습니다.

* 백엔드에서 스키마가 제거되더라도 메타데이터 스키마 게시 취소는 오류 메시지를 채웁니다.

* 게시된 자산에 대해 미리 보기 이미지가 표시되지 않습니다.

* 사용자가 이름에 작은 따옴표가 포함된 자산을 게시하거나 게시 취소할 수 없습니다.

* 여러 자산을 다운로드하는 동안 약관이 표시되지 않습니다.

* 사소한 보안 취약점이 해결되었습니다.

### 알려진 문제 {#known-issues}

이 릴리스에는 다음과 같은 알려진 문제가 포함됩니다.

* 브랜드 포털 사용자는 AEM 6.5.4에서 Adobe I/O로 업그레이드할 때 기여도 폴더 자산을 AEM 자산에 게시할 수 없습니다.

   이 문제는 다음 서비스 팩 6.5.5에서 해결됩니다.

   AEM 6.5.4에 대한 즉각적인 수정 사항은 핫픽스를 [다운로드하고](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) 작성자 인스턴스에 설치하는 것이 좋습니다.

* 자산을 다운로드하는 동안 시스템 표현물 제외 옵션이 제대로 작동하지 않습니다.


## 언어 {#languages}

브랜드 포털 사용자 인터페이스는 다음 언어로 사용할 수 있습니다.

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

이 브랜드 포털 릴리스에서 실행하도록 인증된 플랫폼을 확인하려면 기술 요구 사항의 **작성** 지원 **사용자 인터페이스** 섹션에 있는 표의 터치에 적합한 UI [지원](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html)열을참조하십시오.

## 링크 {#links}

* [adobe.com의 Adobe Experience Manager 제품 페이지](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [자산 브랜드 포털 설명서](https://helpx.adobe.com/experience-manager/brand-portal/user-guide.html)

## 제품 액세스 및 지원(제한된 사이트) {#product-access-and-support-restricted-sites}

다음 사이트는 고객만 사용할 수 있습니다. 고객으로서 액세스 권한이 필요한 경우 Adobe 계정 관리자에게 문의하십시오.

* [](https://daycare.day.com) 제품 [액세스](https://login.marketing.adobe.com)

* [Adobe 고객 지원 센터](https://helpx.adobe.com/contact.html)
