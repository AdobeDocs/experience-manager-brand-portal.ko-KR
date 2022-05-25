---
title: 자산을 업로드하고 Brand Portal의 기여도 폴더를 Experience Manager Assets에 게시합니다
seo-title: Upload assets and publish the Contribution folder from Brand Portal to Experience Manager Assets
description: 새 자산을 업로드하고 Brand Portal에서 Experience Manager Assets으로 기여도 폴더를 게시하는 방법에 대한 통찰력을 얻을 수 있습니다.
seo-description: Get an insight into uploading new assets and publishing the contribution folder from Brand Portal to Experience Manager Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 7dcf445d-97ed-4fa5-959c-c4c48e325766
source-git-commit: 606f4389780025f5cf92b11bf8cac464e36be44a
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 0%

---

# Experience Manager Assets에 기여도 폴더 게시 {#using-asset-souring-in-bp}

적절한 권한이 있는 Brand Portal 사용자는 여러 자산 또는 여러 자산이 들어 있는 폴더를 기여도 폴더에 업로드할 수 있습니다. 그러나 Brand Portal 사용자는 자산을 **신규** 폴더를 입력합니다. 다음 **공유** 폴더는 기여도에 대한 새 자산을 만드는 동안 Brand Portal 사용자가 사용할 수 있는 기준 자산(참조 컨텐츠)의 배포를 위한 것입니다.

기여도 폴더에 액세스할 수 있는 권한이 있는 Brand Portal 사용자는 다음 활동을 수행할 수 있습니다.

* [자산 요구 사항 다운로드](#download-asset-requirements)
* [기여도 폴더에 새 자산 업로드](#uplad-new-assets-to-contribution-folder)
* [Experience Manager Assets에 기여도 폴더 게시](#publish-contribution-folder-to-aem)

## 자산 요구 사항 다운로드 {#download-asset-requirements}

Brand Portal 사용자는 기여 폴더가 Experience Manager Assets 사용자가 공유될 때마다 자동으로 이메일/펄스 알림을 수신하여, 사용자로부터 간단한(자산 요구 사항) 문서를 다운로드하거나 기준 자산(참조 컨텐츠)을 다운로드할 수 있습니다 **공유** 폴더를 삭제하여 자산 요구 사항을 파악합니다.

Brand Portal 사용자는 다음 활동을 수행하여 자산 요구 사항을 다운로드합니다.

* **개요 다운로드**: 자산 유형, 목적, 지원되는 형식, 최대 자산 크기 등과 같은 자산 관련 정보가 있는 기여도 폴더에 첨부된 간략한(자산 요구 문서)을 다운로드합니다.
* **기준 자산 다운로드**: 필요한 자산 유형을 이해하는 데 사용할 수 있는 기준 자산을 다운로드합니다. Brand Portal 사용자는 이러한 자산을 참조로 사용하여 기여할 새 자산을 만들 수 있습니다.

Brand Portal 대시보드는 새 공유 기여도 폴더와 함께 Brand Portal 사용자에게 허용된 모든 기존 폴더를 반영합니다. 이 예에서 Brand Portal 사용자는 새로 만든 기여도 폴더에만 액세스할 수 있고, 다른 기존 폴더는 사용자와 공유되지 않습니다.

**자산 요구 사항을 다운로드하려면 다음을 수행하십시오.**

1. Brand Portal 인스턴스에 로그인합니다.
1. Brand Portal 대시보드에서 기여 폴더를 선택합니다.
1. 클릭 **[!UICONTROL 속성]**. 기여도 폴더 세부 사항이 포함된 속성 창이 열립니다.

   ![](assets/properties.png)

   ![](assets/download-asset-requirement2.png)

1. 을(를) 클릭합니다. **[!UICONTROL 개요 다운로드]** 로컬 시스템에서 자산 요구 사항 문서를 다운로드하는 옵션.

   ![](assets/download.png)

1. Brand Portal 대시보드로 돌아갑니다.
1. 기여도 폴더를 열려면 클릭합니다. 두 개의 하위 폴더가 표시됩니다.**[!UICONTROL 공유]** 및 **[!UICONTROL 신규]** 기여도 폴더 내에 있어야 합니다. 공유 폴더에는 관리자가 공유하는 모든 기준 자산(참조 컨텐츠)이 포함되어 있습니다.
1. 을 다운로드할 수 있습니다 **[!UICONTROL 공유]** 로컬 시스템의 모든 기준 자산을 포함하는 폴더입니다.
또는 **[!UICONTROL 공유]** 폴더를 클릭하고 **다운로드** 아이콘을 사용하여 개별 파일/폴더를 다운로드할 수 있습니다.

   ![](assets/download.png)

   ![](assets/download-asset-requirement5.png)

간략한(자산 요구 사항 문서)을 살펴보고 자산 요구 사항을 이해하려면 기준 자산을 참조하십시오. 이제 기여도를 위한 새 자산을 만들고 기여도 폴더에 업로드할 수 있습니다.


## 기여도 폴더에 자산 업로드 {#upload-new-assets-to-contribution-folder}

자산 요구 사항을 거친 후 Brand Portal 사용자는 기여할 새 자산을 만들고 기여도 폴더 내의 NEW 폴더에 업로드할 수 있습니다. 사용자는 여러 자산을 자산 기여 폴더에 업로드할 수 있습니다. 그러나 한 번에 하나의 폴더만 만들 수 있습니다.

>[!NOTE]
>
>Brand Portal 사용자는 자산을 업로드할 수 있습니다(최대 **2개** NEW 폴더에 GB(파일 크기당)를 추가합니다.
>
>모든 Brand Portal 테넌트에 대한 최대 업로드 제한은 다음과 같습니다 **10**&#x200B;모든 기여도 폴더에 누적 적용되는 GB입니다.
>
>Brand Portal에 업로드된 자산은 표현물에 대해 처리되지 않으며 미리 보기를 포함하지 않습니다.

>[!NOTE]
>
>기여도 폴더를 Experience Manager Assets에 게시한 후 업로드 공간을 해제하여 다른 Brand Portal 사용자가 기여하기 위해 사용할 수 있도록 하는 것이 좋습니다.
>
>Brand Portal 테넌트의 업로드 제한을 초과해야 하는 경우 **10** GB, 고객 지원 센터에 요구 사항을 알려주십시오.


**새 자산을 업로드하려면 다음을 수행하십시오.**

1. Brand Portal 인스턴스에 로그인합니다.
Brand Portal 대시보드는 새 공유 기여도 폴더와 함께 Brand Portal 사용자에게 허용된 모든 기존 폴더를 반영합니다.

1. 기여도 폴더를 선택하고 을(를) 클릭하여 엽니다. 기여도 폴더에는 두 개의 하위 폴더가 있습니다. **[!UICONTROL 공유]** 및 **[!UICONTROL 신규]**.

1. 을(를) 클릭합니다. **[!UICONTROL 신규]** 폴더를 입력합니다.

   ![](assets/upload-new-assets4.png)

1. 클릭 **[!UICONTROL 만들기]** > **[!UICONTROL 파일]** 여러 자산이 들어 있는 개별 파일 또는 폴더(.zip)를 업로드합니다.

   ![](assets/upload-new-assets5.png)

1. 자산(파일 또는 폴더)을 **[!UICONTROL 신규]** 폴더를 입력합니다.

   ![](assets/upload-asset4.png)

모든 자산 또는 폴더를 새 폴더에 업로드한 후 기여도 폴더를 Experience Manager Assets에 게시합니다.


## Experience Manager Assets에 기여도 폴더 게시 {#publish-contribution-folder-to-aem}

Brand Portal 사용자는 Experience Manager 작성자 인스턴스에 액세스하지 않아도 기여도 폴더를 Experience Manager Assets에 게시할 수 있습니다.

자산 요구 사항을 살펴보았는지 확인하고 새로 만든 자산을 업로드하십시오. **신규** 기여도 폴더 내에 있는 폴더입니다.

**기여도 폴더를 게시하려면 다음을 수행하십시오.**

1. Brand Portal 인스턴스에 로그인합니다.

1. Brand Portal 대시보드에서 기여 폴더를 선택합니다.
1. 클릭 **[!UICONTROL AEM에 게시]**.

   ![](assets/export.png)

   ![](assets/publish-contribution-folder-to-aem1.png)

게시 워크플로우의 여러 단계에서 Brand Portal 사용자 및 관리자에게 이메일/펄스 알림이 전송됩니다.

1. **큐에 있음** - Brand Portal에서 게시 작업 과정이 트리거될 때 Brand Portal 사용자 및 Brand Portal 관리자에게 알림이 전송됩니다.

1. **완료** - 기여도 폴더가 Experience Manager Assets에 성공적으로 게시되면 Brand Portal 사용자 및 Brand Portal 관리자에게 알림이 전송됩니다.

새로 만든 자산을 Experience Manager Assets에 게시하면 Brand Portal 사용자는 새 폴더에서 삭제할 수 있습니다. 반면에 Brand Portal 관리자는 NEW 및 SHARED 폴더 모두에서 자산을 삭제할 수 있습니다.

기여 폴더를 만드는 목적이 달성되면 Brand Portal 관리자는 기여 폴더를 삭제하여 다른 사용자의 업로드 공간을 해제할 수 있습니다.

## 게시 작업 상태 {#publishing-job-status}

관리자가 Brand Portal에서 Experience Manager Assets으로 게시된 자산 기여 폴더의 상태를 보는 데 사용할 수 있는 두 개의 보고서가 있습니다.

* Brand Portal에서 **[!UICONTROL 도구]** > **[!UICONTROL 자산 기여 상태]**. 이 보고서는 게시 작업 과정의 여러 단계에 있는 모든 게시 작업 상태를 반영합니다.

   ![](assets/contribution-folder-status-v2.png)

* Experience Manager Assets(온-프레미스 또는 관리 서비스)에서 **[!UICONTROL 자산]** > **[!UICONTROL 작업]**. 이 보고서는 모든 게시 작업의 최종 상태(성공 또는 오류)를 반영합니다.

   ![](assets/publishing-status.png)

* Experience Manager Assets as a Cloud Service에서 **[!UICONTROL 자산]** > **[!UICONTROL 작업]**.

   또는 로 바로 이동할 수 있습니다. **[!UICONTROL 작업]** 전역 탐색에서 를 클릭합니다.

   이 보고서는 Brand Portal에서 Experience Manager Assets으로 자산 가져오기를 포함하여 모든 게시 작업의 최종 상태(성공 또는 오류)를 반영합니다.

   ![](assets/cloud-service-job-status.png)

<!--
>[!NOTE]
>
>Currently, no report is generated in AEM Assets as a Cloud Service for the Asset Sourcing workflow. 
-->

## 기여도 폴더에서 Experience Manager Assets에 게시된 자산의 자동 삭제 {#automatically-delete-published-assets-from-contribution-folder}

이제 Brand Portal은 12시간마다 자동 작업을 실행하여 모든 기여도 폴더를 스캔하고 AEM에 게시된 모든 자산을 삭제합니다. 따라서 폴더 크기를 [임계값 제한](#upload-new-assets-to-contribution-folder). 지난 7일 동안 자동으로 실행된 삭제 작업의 상태를 모니터링할 수도 있습니다. 작업에 대한 보고서는 다음 세부 정보를 제공합니다.

* 작업 시작 시간
* 작업 종료 시간
* 작업 상태
* 작업에 포함된 총 자산
* 작업에서 성공적으로 삭제된 총 자산 수
* 작업 실행 결과로 사용할 수 있는 총 스토리지 수

   ![삭제 보고서](assets/deletion-reports.png)

추가로 드릴다운하여 삭제 작업에 포함된 각 자산의 세부 사항을 볼 수도 있습니다. 자산 제목, 크기, 작성자, 삭제 상태 및 삭제 시간과 같은 세부 정보가 보고서에 포함됩니다.

![삭제 보고서 세부 정보](assets/deletion-reports-detailed.png)

>[!NOTE]
>
> * 고객은 Adobe 고객 지원 센터에 자동 삭제 작업 기능을 비활성화하고 다시 활성화하거나 실행 빈도를 변경하도록 요청할 수 있습니다.
> * 이 기능은 Experience Manager 6.5.13.0 이상 릴리스에서 사용할 수 있습니다.


### 삭제 보고서 보기 및 다운로드 {#view-delete-jobs}

삭제 작업에 대한 보고서를 보고 다운로드하려면

1. Brand Portal에서 **[!UICONTROL 도구]**>**[!UICONTROL 자산 기여 상태]**>**[!UICONTROL 삭제 보고서]** 선택 사항입니다.

1. 작업을 선택하고 **[!UICONTROL 보기]** 보고서를 보려면

   삭제 작업에 포함된 각 자산의 세부 사항을 봅니다. 자산 제목, 크기, 작성자, 삭제 상태 및 삭제 시간과 같은 세부 정보가 보고서에 포함됩니다. 클릭 **[!UICONTROL 다운로드]** 작업에 대한 보고서를 CSV 형식으로 다운로드하려면 다음을 수행하십시오.

   보고서의 자산에 대한 삭제 상태는 다음 값을 가질 수 있습니다.

   * **삭제됨** - 기여도 폴더에서 자산이 삭제되었습니다.

   * **없음** - Brand Portal에서 기여도 폴더에서 자산을 찾을 수 없습니다. 자산이 이미 폴더에서 수동으로 삭제됩니다.

   * **건너뛴** - 기여도 폴더에 아직 Experience Manager에 게시되지 않은 자산에서 사용할 수 있는 새 버전이 있으므로 Brand Portal에서 자산 삭제를 건너뛰었습니다.

   * **실패** - Brand Portal에서 자산을 삭제하지 못했습니다. 가 있는 자산을 삭제하기 위해 세 번 다시 시도됩니다. `Failed` 삭제 상태. 자산이 세 번째 다시 삭제 시도에 실패하면 자산을 수동으로 삭제해야 합니다.

### 보고서 삭제

Brand Portal에서는 하나 이상의 보고서를 선택하고 수동으로 삭제할 수도 있습니다.

보고서를 삭제하려면

1. 다음으로 이동 **[!UICONTROL 도구]**>**[!UICONTROL 자산 기여 상태]**>**[!UICONTROL 삭제 보고서]** 선택 사항입니다.

1. 하나 이상의 보고서를 선택하고 **[!UICONTROL 삭제]**.


