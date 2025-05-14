---
title: 자주 묻는 질문
description: Adobe Experience Manager Assets Brand Portal에서 자주 묻는 질문에 대한 인사이트를 얻으십시오.
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: ht
source-wordcount: '1500'
ht-degree: 100%

---

# 자주 묻는 질문 {#frequently-asked-questions}

Brand Portal FAQ는 최종 사용자가 최신 Experience Manager Assets Brand Portal 6.4.6 릴리스 또는 이전 버전을 사용할 때 겪을 수 있는 질문과 문제에 초점을 맞춥니다.


## Brand Portal 6.4.6 FAQ {#faqs-bp646}

**질문: 기존의 Legacy OAuth 엔드포인트(`https://legacy-oauth.cloud.adobe.io/login`)가 작동하지 않습니다. 가능한 이유는 무엇입니까?**

**답변:** Legacy OAuth 구성은 더 이상 사용되지 않습니다. Experience Manager Assets 작성자 인스턴스를 최신 서비스 팩으로 업그레이드하고 Adobe Developer Console을 통해 구성하십시오. 자세한 내용은 [Brand Portal로 Experience Manager Assets 구성](configure-aem-assets-with-brand-portal.md)을 참조하십시오. 그러나 업그레이드 전까지 Legacy OAuth 구성이 작동하도록 하려면 Legacy OAuth 엔드포인트를 `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`으로 업데이트해야 합니다.

**질문: Adobe Developer Console로 업그레이드한 후 Brand Portal의 기여 폴더 자산을 Experience Manager Assets로 게시할 수 없습니다. 내 작성자 인스턴스는 Experience Manager Assets 6.5.4에 있습니다. 가능한 이유는 무엇입니까?**

**답변:** 예. Adobe Developer Console을 통해 기여 폴더의 자산을 Experience Manager Assets 6.5.4에 게시할 때 알려진 문제가 있습니다.

이 문제는 Experience Manager Assets 6.5.5에서 해결되었습니다. Experience Manager Assets 인스턴스를 최신 서비스 팩으로 업그레이드하고 Adobe Developer Console에서 [구성을 업그레이드](https://experienceleague.adobe.com/ko/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal#upgrade-integration-65)할 수 있습니다.


**질문: Brand Portal에서 게시한 기여 폴더의 콘텐츠가 Experience Manager Assets에서 보이지 않습니다. 가능한 이유는 무엇입니까?**

**답변:** Experience Manager Assets 관리자에게 문의하여 구성을 확인하고 Brand Portal 테넌트가 하나의 Experience Manager Assets 작성자 인스턴스에만 구성되었는지 확인하십시오.

이 문제는 여러 Experience Manager Assets 작성자 인스턴스에 Brand Portal 테넌트를 구성한 경우 발생할 수 있습니다. 예를 들어 관리자가 동일한 Brand Portal 테넌트를 스테이징 환경과 프로덕션 환경의 Experience Manager Assets 작성 인스턴스에 모두 구성한 경우입니다. 이 경우 Brand Portal에서 자산 게시가 트리거되더라도, 복제 에이전트가 요청 토큰을 수신하지 못해 Experience Manager Assets 작성자 인스턴스가 자산을 가져오지 못하게 됩니다.


**질문: Experience Manager Assets의 자산을 Brand Portal에 게시할 수 없습니다. 복제 로그에는 연결 시간이 초과되었다고 기재되어 있습니다. 빠른 해결책이 있습니까?**

**답변:** 일반적으로 복제 대기열에 보류 중인 요청이 여러 개 있는 경우 시간 초과 오류로 인해 게시가 실패합니다. 이 문제를 해결하려면 복제 에이전트가 시간 초과를 방지하도록 구성되어 있는지 확인해야 합니다.

다음 단계를 수행하여 복제 에이전트를 구성하십시오.

1. AEM Experience Manager Assets 작성자 인스턴스에 로그인합니다.
1. **도구** 패널에서 **[!UICONTROL 배포]** > **[!UICONTROL 복제]**&#x200B;로 이동합니다.
1. 복제 페이지에서 **[!UICONTROL `Agents on author`]**&#x200B;를 클릭합니다. Brand Portal 테넌트에 대한 4개의 복제 에이전트를 확인할 수 있습니다.
1. 복제 에이전트 URL을 클릭하면 에이전트 세부 정보가 열립니다.
1. **[!UICONTROL 편집]**&#x200B;을 클릭하여 복제 에이전트 설정을 편집합니다.
1. 에이전트 설정에서 **[!UICONTROL 확장]** 탭을 클릭합니다.
1. **[!UICONTROL 연결 종료]** 확인란을 선택합니다.
1. 4~7단계를 반복하여 4개의 복제 에이전트를 모두 구성합니다.
1. 서버를 다시 시작하고 연결을 확인합니다.


## Brand Portal 6.4.5 FAQ {#faqs-bp645}

**질문: Brand Portal 6.4.5 릴리스의 주요 변경 사항은 무엇입니까?**

**답변:** Experience Manager Assets Brand Portal 6.4.5를 사용하면 사용자가 관리자 권한 없이도 Brand Portal에서 직접 콘텐츠를 업로드하고 Experience Manager Assets에 기여 폴더를 다시 게시할 수 있습니다. 자세한 내용은 [Brand Portal의 자산 소싱](brand-portal-asset-sourcing.md)을 참조하십시오.



**질문: 내가 만든 기존 자산, 기능 또는 구성에 대한 액세스 권한을 잃은 것입니까?**

**답변:** 기존 기능과 구성은 모두 그대로 유지됩니다. 최종 사용자에게는 영향이 없으며, 콘텐츠는 그대로 유지됩니다.



**질문: 언제 새로운 버전의 Brand Portal로 전환할 수 있습니까?**

**답변:** Brand Portal 6.4.5는 2019년 10월에 출시되었습니다. 또한 다음 Brand Portal 버전은 2020년 3월에 출시될 예정입니다.
업데이트 및 버전 변경에 대해서는 [릴리스 정보](brand-portal-release-notes.md) 및 [Brand Portal의 새로운 기능](whats-new.md)을 참조할 것을 권장합니다.



**질문: 내 사용자에게 영향이 있습니까?**

**답변:** Brand Portal 6.4.5 릴리스는 Brand Portal에서만 제공되므로 최종 사용자에게 영향을 미치지 않습니다.



**질문: Brand Portal 사용자로서 취해야 할 조치가 있습니까?**

**답변:** Brand Portal 6.4.5 릴리스에는 자산 소싱이라는 새로운 기능이 추가되었습니다. 관리자는 Experience Manager Assets에서 자산 소싱 기능을 구성하여 Brand Portal 사용자에 대해 해당 기능을 활성화해야 합니다. 자세한 내용은 [자산 소싱 활성화](brand-portal-asset-sourcing.md)를 참조하십시오.



**질문: 누가 기여 폴더를 만들 수 있습니까?**

**답변:** Experience Manager Assets에서 폴더를 만들 수 있는 권한이 있는 모든 Experience Manager Assets 사용자는 **기여** 폴더를 만들 수 있습니다. **기여** 폴더를 만들려면 **자산 기여** 유형의 폴더를 만드십시오.
이 폴더는 기여를 위해 활성 Brand Portal 사용자와 공유됩니다.



**질문: 기여 폴더에는 무엇이 포함됩니까?**

**답변:** **기여** 폴더에는 **신규**&#x200B;와 **공유됨**이라는 두 개의 하위 폴더가 포함되어 있습니다. 처음에는 신규 폴더가 비어 있고 공유됨 폴더에는 Brand Portal 사용자를 위한 참조 콘텐츠(재사용 가능한 자산)가 포함되어 있습니다.
Brand Portal 사용자는 **기여** 폴더에 액세스하고 **신규** 폴더에 콘텐츠를 업로드합니다.



**질문: 기존 기여 폴더의 이름을 수정할 수 있습니까?**

**답변:** **아니요**. 기존 이름 **기여** 폴더 이름은 수정할 수 없습니다.



**질문: 기여와 관련된 자산 요구 사항은 무엇입니까?**

**답변:** **기여** 폴더의 **간략한** 문서와 **공유됨** 폴더의 참조 콘텐츠는 Brand Portal 사용자가 기여의 요구와 기대를 이해하도록 도와줍니다. 이러한 사항을 합쳐 자산 요구사항이라고 합니다.

**질문: 허용되는 폴더에는 자산을 업로드할 수 있습니까?**

**답변:** 허용되는 폴더 중 일부에는 불가합니다. Brand Portal 사용자는 Experience Manager Assets 또는 Brand Portal 관리자가 공유하는 **기여** 폴더에만 콘텐츠를 업로드할 수 있습니다.



**질문: 기여 폴더에 어떻게 액세스할 수 있습니까?**

**답변:** 사용자는 본인과 공유된 **기여** 폴더에만 액세스할 수 있습니다. 기여 폴더가 공유될 때마다 이메일/펄스 알림을 받게 됩니다. 이메일에서 공유된 링크를 통해 기여 폴더에 액세스할 수 있습니다. 또는 Brand Portal 인스턴스에 로그인하고 종 모양 알림 아이콘으로 이동하여 기여 폴더에 액세스할 수 있습니다.

>[!NOTE]
>
>Brand Portal 사용자가 아닌 경우에는 Experience Manager Assets 관리자에게 Admin Console에서 사용자를 생성해 달라고 요청하십시오. 그런 다음 Brand Portal 사용자 목록에 있는 사용자 구성 파일에 프로필을 추가합니다.


**질문: 사용자를 가져오기 위한 CSV 파일의 형식은 무엇입니까?**

**답변:** 형식은 Admin Console에서 대량 사용자 가져오기를 지원하는 형식과 일치합니다. 이메일, 이름, 성은 필수입니다.



**질문: 자산 기여 사용자 드롭다운에서 사용자(Brand Portal 기여자) 목록에 채워지는 내용은 무엇입니까?**

**답변:** 드롭다운의 사용자는 Experience Manager Assets에 업로드된 Brand Portal 사용자 구성(.csv) 파일에서 채워집니다.



**질문: 가져오기 및 게시 작업의 상태는 어디에서 볼 수 있습니까?**

**답변:** Experience Manager Assets의 **비동기** 작업 페이지에서 가져오기 상태를 확인할 수 있습니다. Brand Portal에서는 **[!UICONTROL 도구 > 자산 기여 상태]**&#x200B;에서 게시 작업의 상태를 확인할 수 있습니다.



**질문: Experience Manager에서 주기적으로 실행되는 가져오기 작업의 빈도는 얼마입니까?**

**답변:** Experience Manager Assets에서는 5분마다 폴링이 실행됩니다.



**질문: Brand Portal의 폴더를 Experience Manager Assets로 게시할 수 있는 횟수에 임계값이 있습니까?**

**답변:** 아니요. **신규** 폴더에 있는 모든 자산은 이전에 게시되었는지 여부와 관계없이 Experience Manager Assets에 게시됩니다. Brand Portal의 **기여** 폴더를 Experience Manager Assets로 게시할 때마다 **신규** 폴더의 콘텐츠가 대체됩니다.



**질문: 기여 폴더에 새로운 자산을 업로드하는 방법은 무엇입니까?**

**답변:** [자산을 기여 폴더에 업로드](brand-portal-publish-contribution-folder-to-brand-portal.md)하는 방법에 대한 자세한 설명서를 참조하십시오.



**질문: 신규 폴더에 업로드된 자산의 썸네일이나 미리보기가 표시되지 않습니다.**

**답변:** Brand Portal 측에서 워크플로가 실행되지 않으므로 이는 의도된 동작입니다.



**질문: 변동 중인 폴더를 Experience Manager Assets에서 Brand Portal로 게시하면 어떻게 됩니까?**

**답변:** Experience Manager Assets에서는 폴더가 Brand Portal에 게시될 때마다 로그가 유지됩니다. 게시 시점에 Brand Portal에 게시되지 않은 모든 자산은 복제 대기열에 추가됩니다. 게시 작업이 트리거된 후 폴더에 추가된 모든 자산은 Brand Portal에 게시되지 않습니다. Experience Manager Assets 사용자가 폴더를 다시 게시하면 이전에 게시되지 않았던 자산(복제 대기열에 있는 자산)만 Brand Portal에 게시됩니다. 이 프로세스는 Experience Manager Assets에서 Brand Portal에 게시된 모든 폴더와 기여 폴더 내의 공유됨 폴더에도 적용됩니다.

**질문: 질문이 있으면 누구에게 문의해야 합니까?**

**답변:** Adobe 계정 관리자 또는 고객 지원 센터에 문의하십시오.

>[!NOTE]
>
>릴리스 일정은 예정되어 있지 않으며 변경될 수 있습니다. 업데이트된 릴리스 일정을 알아보려면 Adobe 계정 관리자 또는 고객 지원 센터에 문의하십시오.


## 제품 액세스 및 지원(제한된 사이트) {#product-access-and-support-restricted-sites}

이들 사이트는 고객만 사용할 수 있습니다. 고객이시며 액세스 권한이 필요한 경우 Adobe 계정 관리자에게 문의하십시오.

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Support]()
-->
