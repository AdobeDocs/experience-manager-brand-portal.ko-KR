---
title: 자주 묻는 질문
description: Adobe Experience Manager Assets Brand Portal에서 자주 묻는 질문에 대한 통찰력을 얻으십시오.
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '1500'
ht-degree: 0%

---

# 자주 묻는 질문 {#frequently-asked-questions}

Brand Portal FAQ는 최종 사용자 쿼리와 최신 Experience Manager Assets Brand Portal 6.4.6 릴리스 또는 이전 버전을 사용하는 동안 발생할 수 있는 문제에 중점을 둡니다.


## Brand Portal 6.4.6 FAQ {#faqs-bp646}

**질문: 기존 OAuth 끝점(`https://legacy-oauth.cloud.adobe.io/login`)이 작동하지 않습니다. 가능한 이유는 무엇입니까?**

**답변:** 이전 OAuth 구성은 더 이상 사용되지 않습니다. Experience Manager Assets 작성자 인스턴스를 최신 서비스 팩으로 업그레이드하고 Adobe Developer Console을 통해 구성합니다. 자세한 내용은 [Brand Portal을 사용하여 Experience Manager Assets 구성](configure-aem-assets-with-brand-portal.md)을 참조하십시오. 그러나 업그레이드 전까지 레거시 OAuth 구성이 작동하려면 레거시 OAuth 끝점을 `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`(으)로 업데이트하십시오.

**질문: Adobe Developer Console으로 업그레이드한 후 기여 폴더의 자산을 Brand Portal에서 Experience Manager Assets으로 게시할 수 없습니다. 내 작성자 인스턴스는 Experience Manager Assets 6.5.4에 있습니다. 가능한 이유는 무엇입니까?**

**대답:** 예, Adobe Developer Console을 통해 기여 폴더의 자산을 Experience Manager Assets 6.5.4에 게시하는 동안 알려진 문제가 있습니다.

이 문제는 Experience Manager Assets 6.5.5에서 해결되었습니다. Experience Manager Assets 인스턴스를 최신 서비스 팩으로 업그레이드하고 Adobe Developer Console에서 [구성을 업그레이드](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal#upgrade-integration-65)할 수 있습니다.


**질문: Experience Manager Assets의 Brand Portal에서 게시된 기여도 폴더의 컨텐츠가 표시되지 않습니다. 가능한 이유는 무엇입니까?**

**답변:** Experience Manager Assets 관리자에게 문의하여 구성을 확인하고 Brand Portal 테넌트가 Experience Manager Assets 작성자 인스턴스를 하나만 사용하여 구성되었는지 확인하십시오.

이 문제는 여러 Experience Manager Assets 작성자 인스턴스에 Brand Portal 테넌트를 구성한 경우 발생할 수 있습니다. 예를 들어 관리자는 스테이징 및 프로덕션 환경의 Experience Manager Assets 작성자 인스턴스에서 동일한 Brand Portal 테넌트를 구성합니다. 이 경우 에셋 게시는 Brand Portal에서 트리거되지만, 복제 에이전트가 요청 토큰을 받지 못하기 때문에 Experience Manager Assets 작성자 인스턴스가 에셋을 가져올 수 없습니다.


**질문: Experience Manager Assets에서 Brand Portal으로 자산을 게시할 수 없습니다. 복제 로그 상태는 연결 시간이 초과되었음을 나타냅니다. 빠른 해결 방법이 있습니까?**

**대답:** 복제 큐에 대기 중인 요청이 여러 개 있는 경우 대개 시간 초과 오류가 발생하여 게시가 실패합니다. 이 문제를 해결하려면 복제 에이전트가 시간 초과를 방지하도록 구성되었는지 확인합니다.

복제 에이전트를 구성하려면 다음 단계를 수행하십시오.

1. Experience Manager Assets 작성자 인스턴스에 로그인합니다.
1. **도구** 패널에서 **[!UICONTROL 배포]** > **[!UICONTROL 복제]**(으)로 이동합니다.
1. 복제 페이지에서 **[!UICONTROL `Agents on author`]**&#x200B;을(를) 클릭합니다. Brand Portal 테넌트에 대한 4개의 복제 에이전트를 볼 수 있습니다.
1. 복제 에이전트 URL을 클릭하여 에이전트 세부 정보를 엽니다.
1. 복제 에이전트 설정을 편집하려면 **[!UICONTROL 편집]**&#x200B;을 클릭하세요.
1. 에이전트 설정에서 **[!UICONTROL 확장]** 탭을 클릭합니다.
1. **[!UICONTROL 연결 끊기]** 확인란을 선택하십시오.
1. 4단계부터 7단계까지 반복하여 4개의 복제 에이전트를 모두 구성합니다.
1. 서버를 다시 시작하고 연결을 확인합니다.


## Brand Portal 6.4.5 FAQ {#faqs-bp645}

**질문: Brand Portal 6.4.5 릴리스의 주요 변경 사항은 무엇입니까?**

**대답:** Experience Manager Assets Brand Portal 6.4.5를 사용하면 관리자 권한 없이 사용자가 콘텐츠를 업로드하고 기여도 폴더를 Brand Portal에서 직접 Experience Manager Assets에 다시 게시할 수 있습니다. 자세한 내용은 [Brand Portal의 자산 소싱](brand-portal-asset-sourcing.md)을 참조하십시오.



**질문: 기존 에셋, 기능 또는 만든 구성에 대한 액세스 권한을 상실했습니까?**

**대답:** 기존의 모든 기능과 구성이 그대로 유지됩니다. 최종 사용자는 영향을 받지 않으며 콘텐츠는 그대로 유지됩니다.



**질문: 새 버전의 Brand Portal으로 전환하는 경우는 언제입니까?**

**대답:** Brand Portal 6.4.5는 2019년 10월에 프로덕션에 출시되었습니다. 그리고 다음 Brand Portal 버전은 2020년 3월이 될 예정입니다.
Adobe 업데이트 및 버전 변경의 경우 [릴리스 정보](brand-portal-release-notes.md) 및 [Brand Portal의 새로운 기능](whats-new.md)을 추적하는 것이 좋습니다.



**질문: 내 사용자가 영향을 받습니까?**

**답변:** Brand Portal 6.4.5 릴리스는 전적으로 Brand Portal 내에 있으므로 최종 사용자에게 영향을 주지 않습니다.



**질문: Brand Portal 사용자로서 내 작업에 필요한 작업이 있습니까?**

**대답:** Brand Portal 6.4.5 릴리스에는 Asset Sourcing이라는 새로운 기능이 포함되어 있습니다. 관리자는 Experience Manager Assets 사용자가 이 기능을 사용할 수 있도록 Brand Portal에서 에셋 소싱 기능을 구성해야 합니다. 자세한 내용은 [자산 소싱 사용](brand-portal-asset-sourcing.md)을 참조하세요.



**질문: 기여도 폴더를 만들 수 있는 사용자는 누구입니까?**

**답변:** Experience Manager Assets에서 폴더를 만들 수 있는 권한이 있는 모든 Experience Manager Assets 사용자는 **기여도** 폴더를 만들 수 있습니다. **기여도** 폴더를 만들려면 **자산 기여도** 유형의 폴더를 만드십시오.
이 폴더는 기여를 위해 활성 Brand Portal 사용자와 공유됩니다.



**질문: 기여 폴더에 포함된 항목은 무엇입니까?**

**답변:** **기여도** 폴더에 하위 폴더 **NEW** 및 **공유**가 두 개 있습니다. 처음에는 NEW 폴더가 비어 있고 SHARED 폴더에 Brand Portal 사용자에 대한 참조 콘텐츠(재사용 가능한 에셋)가 포함되어 있습니다.
Brand Portal 사용자는 **기여도** 폴더에 액세스하여 **NEW** 폴더에 있는 콘텐츠를 업로드합니다.



**질문: 기존 기여도 폴더의 이름을 수정할 수 있습니까?**

**답변:** **아니요**, 기존 **기여도** 폴더의 이름을 수정할 수 없습니다.



**질문: 기여도를 제외한 자산 요구 사항은 무엇입니까?**

**대답:** **기여도** 폴더의 **개요** 문서와 **공유** 폴더의 참조 콘텐츠는 Brand Portal 사용자가 기여도 요구 사항과 기대를 이해하는 데 도움이 됩니다. 이를 함께 자산 요구 사항이라고 합니다.

**질문: 에셋을 허용된 폴더에 업로드할 수 있습니까?**

**대답:** 허용된 폴더 중 일부가 아닙니다. Brand Portal 사용자는 Experience Manager Assets 또는 Brand Portal 관리자가 공유하는 **기여도** 폴더에만 콘텐츠를 업로드할 수 있습니다.



**질문: 기여 폴더에 액세스하려면 어떻게 해야 합니까?**

**답변:** **기여도** 폴더는 사용자와 공유된 경우에만 액세스할 수 있습니다. 기여도 폴더가 공유될 때마다 이메일/펄스 알림을 받습니다. 이메일에 공유된 링크를 통해 기여도 폴더에 액세스할 수 있습니다. 또는 Brand Portal 인스턴스에 로그인하고 알림 벨 아이콘으로 이동하여 기여도 폴더에 액세스할 수 있습니다.

>[!NOTE]
>
>Brand Portal 사용자가 아닌 경우 Experience Manager Assets 관리자에게 요청하여 Admin Console에서 사용자를 만듭니다. 그런 다음 Brand Portal 사용자 목록의 사용자 구성 파일에 프로필을 추가합니다.


**질문: 사용자 가져오기에 사용할 CSV 파일의 형식은 무엇입니까?**

**대답:** 형식이 대량 사용자 가져오기에 대해 Admin Console이 지원하는 형식과 일치합니다. 이메일, 이름 및 성은 필수입니다.



**질문: 자산 기여 사용자 드롭다운에서 사용자(Brand Portal 기여자) 목록을 채우는 것은 무엇입니까?**

**답변:** 드롭다운의 사용자는 Experience Manager Assets에 업로드된 Brand Portal 사용자 구성(.csv) 파일에서 채워집니다.



**질문: 가져오기 및 게시 작업의 상태는 어디에서 확인할 수 있습니까?**

**답변:** Experience Manager Assets의 **비동기** 작업 페이지에서 가져오기 상태를 확인할 수 있습니다. Brand Portal에서는 **[!UICONTROL 도구 > 자산 기여도 상태]**&#x200B;에서 게시 작업의 상태를 볼 수 있습니다.



**질문: Experience Manager에서 주기적으로 실행되는 가져오기 작업의 빈도는 얼마입니까?**

**대답:** Experience Manager Assets에서는 5분마다 폴링을 실행합니다.



**질문: 폴더를 Brand Portal에서 Experience Manager Assets으로 게시할 수 있는 횟수에 임계값이 있습니까?**

**대답:** 아니요, **NEW** 폴더의 모든 자산은 이전에 게시한 사실과 관계없이 Experience Manager Assets에 게시됩니다. **기여도** 폴더가 Brand Portal에서 Experience Manager Assets으로 게시될 때마다 **NEW** 폴더의 콘텐츠가 바뀝니다.



**질문: 기여 폴더에 새 자산을 업로드하는 방법**

**대답:** [기여 폴더에 자산 업로드](brand-portal-publish-contribution-folder-to-brand-portal.md)에 대한 자세한 설명서를 참조하세요.



**질문: NEW 폴더에 업로드된 자산의 미리 보기나 썸네일을 볼 수 없습니다.**

**대답:** Brand Portal 끝에는 워크플로우가 실행되지 않으므로 설계된 방식입니다.



**질문: 폴더를 Experience Manager Assets에서 Brand Portal으로 게시하면 어떻게 됩니까?**

**답변:** Experience Manager Assets에서는 폴더를 Brand Portal에 게시할 때마다 로그가 유지됩니다. 게시할 때 Brand Portal에 게시되지 않은 모든 자산이 복제 큐에 추가됩니다. 게시 작업이 트리거된 후 폴더에 추가된 모든 자산은 Brand Portal에 게시되지 않습니다. Experience Manager Assets 사용자가 폴더를 다시 게시하면 이전에 게시되지 않은(복제 큐에 있는) 자산만 Brand Portal에 게시됩니다. 이 프로세스는 Experience Manager Assets에서 Brand Portal으로 게시된 모든 폴더와 기여도 폴더 내의 공유 폴더에 대해 적용됩니다.

**질문: 누구에게 문의해야 합니까?**

**답변:** Adobe 계정 관리자 또는 고객 지원 센터에 문의하십시오.

>[!NOTE]
>
>출시 일정은 잠정적이며 변경될 수 있습니다. 업데이트된 릴리스 일정을 얻으려면 Adobe 계정 관리자 또는 고객 지원 센터에 문의하십시오.


## 제품 액세스 및 지원(제한된 사이트) {#product-access-and-support-restricted-sites}

이러한 사이트는 고객만 사용할 수 있습니다. 고객이고 액세스 권한이 필요한 경우 Adobe 계정 관리자에게 문의하십시오.

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Support]()
-->
