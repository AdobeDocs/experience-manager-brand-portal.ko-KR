---
title: 보고서를 사용한 작업
seo-title: 보고서를 사용한 작업
description: AEM Assets 브랜드 포털 관리자는 브랜드 포털 사용에 대한 보고서를 보고, 브랜드 포털을 통해 공유되는 다운로드, 만료, 게시 및 링크에 대한 보고서를 만들고, 관리하고, 볼 수 있습니다.
seo-description: AEM Assets 브랜드 포털 관리자는 브랜드 포털 사용에 대한 보고서를 보고, 브랜드 포털을 통해 공유되는 다운로드, 만료, 게시 및 링크에 대한 보고서를 만들고, 관리하고, 볼 수 있습니다.
uuid: dc4e5275-a614-4b95-8c70-2b7e470c50a7
content-type: 참조
topic-tags: 관리
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 7683074f-b6ea-42e0-a411-3b13eb88d1f2
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d

---


# 보고서를 사용한 작업 {#work-with-reports}

보고 기능은 브랜드 포털 사용을 평가하고 내부 및 외부 사용자가 승인된 자산과 어떻게 상호 작용하는지 파악하는 데 유용합니다. 관리자는 자산 보고서 페이지에서 항상 사용할 수 있는 브랜드 포털 사용량 보고서를 볼 수 있습니다. 그러나 사용자 로그인 및 링크를 통해 다운로드한 자산, 만료, 게시 및 링크를 통해 공유되는 자산에 대한 보고서를 생성하여 자산 보고서 페이지에서 볼 수 있습니다. 이러한 보고서는 조직 내외부에서 승인된 자산의 채택을 측정하는 데 주요 성공 지표를 도출할 수 있는 자산 배포를 분석하는 데 유용합니다.

보고서 관리 인터페이스는 직관적이고 세밀하게 정의된 옵션과 저장된 보고서에 액세스할 수 있는 컨트롤을 포함합니다. 이전에 생성된 모든 보고서가 나열된 자산 보고서 페이지에서 보고서를 보거나, 다운로드하거나, 삭제할 수 있습니다.

## 보고서 보기 {#view-reports}

보고서를 보려면 다음 단계를 수행합니다.

1. 맨 위의 도구 모음에서 AEM 로고를 탭/클릭하여 관리 도구에 액세스합니다.

   ![](assets/aemlogo.png)

1. 관리 도구 패널에서 보고서 만들기/ **[!UICONTROL 관리를 클릭하여]** 자산 **[!UICONTROL 보고서]** 페이지를 엽니다.

   ![](assets/access-asset-reports.png)

1. 자산 **[!UICONTROL 보고서]** 페이지에서 사용량 보고서와 기타 생성된 보고서에 액세스합니다.

   >[!NOTE]
   >
   >사용 보고서는 기본적으로 브랜드 포털에 있습니다. 만들거나 삭제할 수 없습니다. 그러나 다운로드, 만료, 게시, 링크 공유 및 사용자 로그인 보고서를 만들고, 다운로드하고, 삭제할 수 있습니다.

   보고서를 보려면 보고서 링크를 탭/클릭합니다. 또는 보고서를 선택하고 도구 모음에서 보기 아이콘을 탭/클릭합니다.

   [!UICONTROL 사용 보고서는] 현재 브랜드 포털 사용자 수, 모든 자산이 차지하는 저장소 공간 및 브랜드 포털의 총 자산 수에 대한 정보를 표시합니다. 이 보고서는 이러한 각 정보 지표에 대해 허용된 용량을 표시합니다.

   ![](assets/usage-report.png)

   [!UICONTROL 사용자 로그인] 보고서는 브랜드 포털에 로그인한 사용자에 대한 정보를 제공합니다. 보고서는 보고서 생성 시점까지 브랜드 포털 6.4.2 배포에서 각 사용자의 표시 이름, 이메일 ID, 개인(관리자, 뷰어, 편집기, 손님), 그룹, 마지막 로그인, 활동 상태 및 로그인 수를 보여줍니다.

   ![](assets/user-logins.png)

   [!UICONTROL Download] report lists and details about all the assets downloaded in a specific date and time range.

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >자산 다운로드 [!UICONTROL 보고서는] 개별적으로 선택되어 브랜드 포털에서 다운로드한 자산만 표시합니다. 사용자가 에셋이 포함된 폴더를 다운로드한 경우, 보고서는 폴더 또는 폴더 내의 에셋을 표시하지 않습니다.

   [!UICONTROL Expiration] report lists and details all the assets that expired in a specific time frame.

   ![](assets/expiration-report.png)

   [!UICONTROL Publish] report lists and gives information about all the assets that are published from AEM to Brand Portal in a specified time frame.

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >Publish Report does not display information about content fragments, as the content fragments cannot be published to the Brand Portal.

   [!UICONTROL Link Share report lists all the assets shared through links from Brand Portal interface in a specific time frame. ] The report also informs when was the asset shared via link, by which user, when does the link expire, and the number of shared links for the tenant (and users with whom the asset link was shared). The columns of Link Share Report are not customizable.

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >The Link Share Report does not display users who have access to the asset shared via the link or have downloaded the asset through the link.
   >
   >
   >For tracking downloads through the shared link, you need to generate download report after selecting Only Link Share Downloads option on Create Report page. ******** However, user (Downloaded by) is anonymous in this case.

## Generate reports {#generate-reports}

Administrators can generate and manage the following standard reports, once generated, they are saved to be accessed later:[](../using/brand-portal-reports.md#main-pars-header)

* 사용자 로그인
* 다운로드
* 만료
* 게시
* 공유 링크

The columns in the Download, Expiration, and Publish report can be customized for viewing. To generate a report, follow these steps:

1. From toolbar at the top, tap/click the AEM logo to access administrative tools.

   ![](assets/aemlogo.png)

1. 관리 도구 패널에서 보고서 만들기/관리를 탭/클릭하여 **[!UICONTROL 자산]** 보고서 **[!UICONTROL 페이지를 엽니다]** .

   ![](assets/asset-reports.png)

1. 자산 보고서 페이지에서 만들기를 탭/ **[!UICONTROL 클릭합니다]**.
1. 보고서 **[!UICONTROL 만들기]** 페이지에서 만들 보고서를 선택하고 다음을 탭/ **[!UICONTROL 클릭합니다]**.

   ![](assets/crete-report.png)

1. 보고서 세부 사항을 구성합니다. 제목, 설명, 폴더 구조(보고서를 실행 및 생성해야 하는 위치), 다운로드, 만료 및 [!UICONTROL 게시]보고서의 날짜 [!UICONTROL 범위를] 지정합니다.

   ![](assets/create-report-page.png)

   반면에 [!UICONTROL 링크 공유 보고서는] 제목, 설명 및 날짜 범위 매개 변수만 있으면 됩니다.

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >보고서 제목의 특수 문자 번호 및 비율은 보고서 생성 시 하이픈(-)으로 대체됩니다.

1. 다음을 탭/ **[!UICONTROL 클릭하여]**&#x200B;다운로드, 만료 및 게시 보고서의 열을 구성합니다.
1. 필요에 따라 해당 확인란을 선택하거나 선택 취소합니다. 예를 들어 다운로드 보고서에서 사용자(자산을 다운로드한 사용자)의 이름을 보려면 [!UICONTROL 다운로드자] ( **[!UICONTROL 다운로드한 사람)를]**&#x200B;선택합니다. 다음 이미지는 다운로드 보고서에서 기본 열을 선택하는 방법을 보여줍니다.

   ![](assets/createdownloadreport.png)

   이러한 보고서에 사용자 지정 열을 추가하여 사용자 지정 요구 사항에 대한 데이터를 더 많이 표시할 수도 있습니다.

   다운로드, 게시 또는 만료 보고서에 사용자 지정 열을 추가하려면 다음 단계를 따르십시오.

   1. 사용자 지정 열을 표시하려면 사용자 지정 열 **[!UICONTROL 내에서 추가를]** 탭/ [!UICONTROL 클릭합니다].
   1. 열 이름 필드에 열 이름을 **[!UICONTROL 지정합니다]** .
   1. 속성 선택기를 사용하여 열을 매핑해야 하는 속성을 선택합니다.

      ![](assets/property-picker.png)
또는 속성 경로 필드에 경로를 입력합니다.

      ![](assets/property-path.png)

      사용자 정의 열을 더 추가하려면 추가를 탭/클릭하고 **2단계와 3단계를** 반복합니다.

1. **[!UICONTROL 만들기를 탭/클릭합니다]**. 보고서 생성이 시작되었음을 알리는 메시지가 표시됩니다.

## 보고서 다운로드 {#download-reports}

보고서를 .csv 파일로 저장하고 다운로드하려면 다음 중 하나를 수행합니다.

* 자산 보고서 페이지에서 보고서를 선택하고 맨 위의 도구 **[!UICONTROL 모음에서]** 다운로드를 탭/클릭합니다.

![](assets/download-asset-report.png)

* 자산 보고서 페이지에서 보고서를 엽니다. 보고서 **[!UICONTROL 페이지]** 맨 위에서 다운로드 옵션을 선택합니다.

![](assets/download-report-fromwithin.png)

## 보고서 삭제 {#delete-reports}

기존 보고서를 삭제하려면 자산 보고서 **[!UICONTROL 페이지에서]** 보고서를 선택하고 맨 **[!UICONTROL 위의 도구 모음에서]** 삭제를 탭/클릭합니다.

>[!NOTE]
>
>[!UICONTROL 사용] 보고서는 삭제할 수 없습니다.
