---
title: 자산의 디지털 권한 관리
seo-title: 자산의 디지털 권한 관리
description: 에셋 라이선싱 및 에셋 및 공유 링크에 대한 만료 설정을 통해 이러한 에셋의 사용을 제어하고 안전하게 보호할 수 있습니다.
seo-description: 에셋 라이선싱 및 에셋 및 공유 링크에 대한 만료 설정을 통해 이러한 에셋의 사용을 제어하고 안전하게 보호할 수 있습니다.
uuid: ce30e398-0109-41bf-a4d2-2fcca476f499
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: f77003ba-31fe-4a9e-96c8-dbc4c2eba79e
role: 관리자
translation-type: tm+mt
source-git-commit: 263653916e4bc183827c197c3beb137c9e59ccb1
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 3%

---


# 자산의 디지털 권한 관리 {#manage-digital-rights-of-assets}

브랜드를 보호하기 위해 크리에이티브 에셋과 브랜드 자료의 안전한 배포와 사용을 보장하는 것이 중요합니다. 만료일(및 시간)을 AEM에서 브랜드 포털에 게시된 승인된 자산에 연결하거나, 조건부 사용을 위해 이러한 자산에 라이선스를 부여함으로써 조직 및 외부에서 적용할 수 있습니다. 또한 브랜드 포털에서는 브랜드 포털에서 공유된 에셋에 대한 링크에 대한 만료 날짜를 지정할 수 있습니다.

브랜드 포털에서 자산이 어떻게 보호되고 관련 사용 권한을 이해하는지 살펴보십시오.

## 자산 만료 {#asset-expiration}

에셋 만료는 조직 전체에서 브랜드 포털에서 승인된 에셋의 사용을 제어하는 효과적인 방법입니다. AEM Assets에서 브랜드 포털로 게시되는 모든 자산은 만료 날짜가 있으며, 이 날짜는 다른 사용자 역할별로 이러한 자산의 사용을 제한할 수 있습니다.

### 만료된 자산 {#usage-permissions-expired-assets} 관련 사용 권한

브랜드 포털에서 관리자는 만료된 자산을 보고 다운로드하고 컬렉션에 추가할 수 있습니다. 반면에 편집자와 뷰어는 만료된 자산만 보고 컬렉션에 추가할 수 있습니다.

관리자는 AEM Assets에서 만료된 자산을 브랜드 포털에 게시할 수 있습니다. 그러나 만료된 자산은 브랜드 포털의 링크를 통해 공유할 수 없습니다. 만료된 자산과 만료되지 않은 자산이 모두 포함된 폴더에서 만료된 자산을 선택하는 경우 **[!UICONTROL 링크 공유]** 작업을 사용할 수 없습니다. 그러나 만료되거나 만료되지 않은 에셋이 포함된 폴더를 선택하면 [!UICONTROL 공유] 및 **[!UICONTROL 링크 공유]** 작업을 사용할 수 있습니다.

>[!NOTE]
>
>폴더가 만료된 에셋이 포함되어 있더라도 여전히 링크로 공유할 수 있습니다. 이 경우 링크가 만료된 자산을 나열하지 않고 만료되지 않은 자산만 공유됩니다.

다음 표에는 만료된 자산의 사용 권한이 표시됩니다.

|  | **[!UICONTROL 링크 공유]** | **[!UICONTROL 다운로드]** | **[!UICONTROL 속성]** | **[!UICONTROL 컬렉션에 추가]** | **[!UICONTROL 삭제]** |
|---|---|---|---|---|---|
| **[!UICONTROL 관리자]** | 사용할 수 없음 | 사용 가능 | 사용 가능 | 사용 가능 | 사용 가능 |
| **[!UICONTROL 편집자]** | 사용할 수 없음 | 사용할 수 없음 | 사용 가능 | 사용 가능 | 사용할 수 없음 |
| **[!UICONTROL 뷰어]** | 사용할 수 없음 | 사용할 수 없음 | 사용 가능 | 사용 가능 | 사용할 수 없음 |
| **[!UICONTROL 손님 사용자]** | 사용할 수 없음 | 사용할 수 없음 | 사용 가능 | 사용 가능 | 사용할 수 없음 |

>[!NOTE]
>
>뷰어 및 편집기가 만료되거나 만료되지 않은 에셋이 포함된 폴더를 다운로드하는 경우 만료되지 않은 에셋만 다운로드됩니다. 폴더에 만료된 에셋만 포함된 경우 빈 폴더가 다운로드됩니다.

### 에셋의 만료 상태 {#expiration-status-of-assets}

**[!UICONTROL 카드 보기]**&#x200B;에서 자산의 만료 상태를 볼 수 있습니다. 카드의 빨간색 플래그는 자산이 만료되었음을 나타냅니다.

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>목록 및 열 보기에는 자산의 만료 상태가 표시되지 않습니다.

## 자산 링크 만료 {#asset-link-expiration}

링크를 통해 자산을 공유하는 동안 관리자와 편집자는 **[!UICONTROL 링크 공유]** 대화 상자의 **[!UICONTROL 만료]** 필드를 사용하여 만료 날짜 및 시간을 설정할 수 있습니다. 링크의 기본 만료는 링크가 공유된 날짜로부터 7일입니다.

![](assets/asset-link-sharing.png)

이렇게 하면 링크로 공유된 에셋이 브랜드 포털 관리자 및 편집자가 설정한 날짜 및 시간에 만료되며, 만료 날짜 이후에 더 이상 보고 다운로드할 수 없게 됩니다. 링크를 통해 공유되는 자산은 조직에 속하지 않는 외부 사용자가 볼 수도 있으므로 만료일을 지정하여 승인된 자산이 보호되고 지정된 시간이 지나면 알 수 없는 개체에 노출되지 않도록 할 수 있습니다.

링크 공유에 대한 자세한 내용은 [에셋을 링크로 공유](../using/brand-portal-link-share.md)를 참조하십시오.

## 라이센스 자산 {#licensed-assets}

라이선스 자산은 브랜드 포털에서 다운로드하기 전에 사용권 계약에 동의해야 합니다. 라이선스가 부여된 에셋에 대한 본 계약은 브랜드 포털에서 직접 또는 공유 링크를 통해 에셋을 다운로드할 때 제공됩니다. 만료되거나 만료되지 않은 경우 라이선스를 보호된 자산을 모든 사용자가 볼 수 있습니다. 그러나 라이선스가 만료된 에셋의 다운로드 및 사용은 제한됩니다. 사용자 역할에 따라 만료된 라이선스가 부여된 에셋의 동작 및 허용되는 활동에 대해 알려면 [만료된 에셋 사용 권한](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets)을 참조하십시오.

라이선스로 보호된 자산은 AEM Assets에서 자산의 [메타데이터 속성](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets)을 설정하여](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets)에 첨부된 [사용권 계약을 가집니다.

라이선스로 보호된 에셋을 다운로드하도록 선택하면 **[!UICONTROL 저작권 관리]** 페이지로 리디렉션됩니다.

![](assets/asset-copyright-mgmt.png)

여기에서 다운로드할 에셋을 선택하고 관련 사용권 계약에 동의해야 합니다. 라이센스 계약에 동의하지 않으면 **[!UICONTROL 다운로드]** 단추가 활성화되지 않습니다.

![](assets/licensed-asset-download-2.png)

선택 항목에 여러 개의 보호된 에셋이 포함되어 있는 경우 한 번에 하나의 에셋을 선택하고 라이선스 계약에 동의한 다음 에셋 다운로드를 계속 진행합니다.

## 만료된 자산 {#generate-report-about-expired-assets}에 대한 보고서 생성

관리자는 특정 기간 내에 만료된 모든 에셋을 나열하는 보고서를 생성하고 다운로드할 수 있습니다. 이 보고서에는 크기, 유형, 자산 계층 구조에서 자산 위치를 지정하는 경로, 자산이 만료된 시기, 자산이 게시된 시기 등 만료된 자산에 대한 자세한 정보가 포함되어 있습니다. 이 보고서의 열을 사용자 요구 사항에 따라 더 많은 데이터를 표시하도록 사용자 지정할 수 있습니다.

![](assets/assets-expired.png)

보고서 기능에 대한 자세한 내용은 [보고서 작업](../using/brand-portal-reports.md#work-with-reports)을 참조하십시오.
