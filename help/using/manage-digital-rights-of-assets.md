---
title: 자산의 디지털 권한 관리
seo-title: 자산의 디지털 권한 관리
description: 자산 라이선스 및 자산 및 공유 링크에 대한 만료 설정을 통해 이러한 자산의 사용을 제어하고 안전하게 보호할 수 있습니다.
seo-description: 자산 라이선스 및 자산 및 공유 링크에 대한 만료 설정을 통해 이러한 자산의 사용을 제어하고 안전하게 보호할 수 있습니다.
uuid: ce30e398-0109-41bf-a4d2-2fcca476f499
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: f77003ba-31fe-4a9e-96c8-dbc4c2eba79e
role: Admin
exl-id: 86c31891-0627-41ca-b571-8dac3a074d55
source-git-commit: 26b009fec800d9b437bde5838009c71b1b3b7ac6
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 2%

---

# 자산의 디지털 권한 관리 {#manage-digital-rights-of-assets}

크리에이티브 자산과 브랜드 자료의 안전한 배포와 사용을 보장하는 것은 브랜드를 보호하는 데 중요합니다. 이 작업은 만료 날짜(및 시간)를 AEM에서 Brand Portal에 게시된 승인된 자산과 연결하거나, 조건부 사용을 위해 이러한 자산의 라이선스를 통해 조직 및 외부에서 적용할 수 있습니다. 또한 Brand Portal에서는 Brand Portal에서 공유된 자산에 대한 링크에 대한 만료 날짜를 지정할 수 있습니다.

Brand Portal에서 자산이 어떻게 보호되는지 그리고 관련 사용 권한을 이해하려면 를 참조하십시오.

## 자산 만료 {#asset-expiration}

자산 만료는 조직 전체에서 Brand Portal에서 승인된 자산의 사용을 제어하는 효과적인 방법입니다. AEM Assets에서 Brand Portal으로 게시되는 모든 자산에는 만료 날짜가 있으며, 이 날짜가 다른 사용자 역할별로 이러한 자산의 사용을 제한할 수 있습니다.

### 만료된 자산과 관련된 사용 권한 {#usage-permissions-expired-assets}

Brand Portal에서 관리자는 만료된 자산을 보고, 다운로드하고, 컬렉션에 추가할 수 있습니다. 반면에 편집자와 뷰어는 만료된 자산만 보고 컬렉션에 추가할 수 있습니다.

관리자는 AEM Assets에서 Brand Portal으로 만료된 자산을 게시할 수 있습니다. 그러나 만료된 자산은 Brand Portal의 잉크를 통해 공유할 수 없습니다. 만료된 자산과 만료되지 않은 자산을 모두 포함하는 폴더에서 만료된 자산을 선택하는 경우 **[!UICONTROL 링크 공유]** 작업을 사용할 수 없습니다. 그러나 만료되거나 만료되지 않은 자산이 포함된 폴더를 선택하면 [!UICONTROL 공유] 및 **[!UICONTROL 링크 공유]** 작업을 사용할 수 있습니다.

>[!NOTE]
>
>폴더는 만료된 자산이 포함되어 있어도 링크로 공유할 수 있습니다. 이 경우, 링크는 만료된 자산을 나열하지 않고, 만료되지 않은 자산만 공유됩니다.

다음 표에는 만료된 자산의 사용 권한이 표시됩니다.

|  | **[!UICONTROL 링크 공유]** | **[!UICONTROL 다운로드]** | **[!UICONTROL 속성]** | **[!UICONTROL 컬렉션에 추가]** | **[!UICONTROL 삭제]** |
|---|---|---|---|---|---|
| **[!UICONTROL 관리자]** | 사용할 수 없음 | 사용 가능 | 사용 가능 | 사용 가능 | 사용 가능 |
| **[!UICONTROL 편집자]** | 사용할 수 없음 | 사용할 수 없음 | 사용 가능 | 사용 가능 | 사용할 수 없음 |
| **[!UICONTROL 뷰어]** | 사용할 수 없음 | 사용할 수 없음 | 사용 가능 | 사용 가능 | 사용할 수 없음 |
| **[!UICONTROL 게스트 사용자]** | 사용할 수 없음 | 사용할 수 없음 | 사용 가능 | 사용 가능 | 사용할 수 없음 |

>[!NOTE]
>
>뷰어 및 편집자가 만료된 자산과 만료되지 않은 자산이 들어 있는 폴더를 다운로드하는 경우 만료되지 않은 자산만 다운로드됩니다. 폴더에 만료된 자산만 포함된 경우 빈 폴더가 다운로드됩니다.

### 자산의 만료 상태 {#expiration-status-of-assets}

**[!UICONTROL 카드 보기에서 자산의 만료 상태를 볼 수 있습니다]**. 카드의 빨간색 플래그는 자산이 만료되었음을 나타냅니다.

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>목록 및 열 보기에는 자산의 만료 상태가 표시되지 않습니다.

## 자산 링크 만료 {#asset-link-expiration}

링크를 통해 자산을 공유하는 동안 관리자 및 편집자는 **[!UICONTROL 링크 공유]** 대화 상자의 **[!UICONTROL 만료]** 필드를 사용하여 만료 날짜와 시간을 설정할 수 있습니다. 링크의 기본 만료는 링크가 공유된 날짜부터 7일입니다.

![](assets/asset-link-sharing.png)

이렇게 하면 링크로 공유된 자산이 Brand Portal 관리자 및 편집자가 설정한 날짜 및 시간에 만료되며, 만료 날짜 이후에 더 이상 보고 다운로드할 수 없게 됩니다. 링크를 통해 공유되는 자산은 조직에 속하지 않는 외부 사용자도 볼 수 있으므로 만료를 지정하면 승인된 자산이 보호되고 지정된 시간 이후에 알 수 없는 엔티티에 노출되지 않았는지 확인할 수 있습니다.

링크 공유에 대한 자세한 내용은 [링크로 자산 공유](../using/brand-portal-link-share.md)를 참조하십시오.

## 라이선스가 있는 자산 {#licensed-assets}

라이선스가 있는 자산은 Brand Portal에서 다운로드하기 전에 라이선스 계약을 수락해야 합니다. 라이선스가 있는 자산에 대한 이 계약은 Brand Portal에서 자산을 직접 다운로드하거나 공유 링크를 통해 다운로드할 때 제공됩니다. 만료되었거나 만료되지 않았더라도 라이선스로 보호된 자산은 모든 사용자가 볼 수 있습니다. 그러나 라이선스가 만료된 자산의 다운로드 및 사용은 제한됩니다. 만료된 라이선스가 있는 자산의 동작 및 사용자 역할에 따른 허용 활동에 대해 알아보려면 [만료된 자산의 사용 권한](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets)을 참조하십시오.

라이선스로 보호된 자산에는 [사용권 계약이 첨부되어 있습니다. 이 계약서는 AEM Assets에서 자산의 [메타데이터 속성](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets)을 설정하여 수행됩니다.](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets)

라이선스로 보호된 자산을 다운로드하도록 선택하면 **[!UICONTROL Copyright Management]** 페이지로 리디렉션됩니다.

![](assets/asset-copyright-mgmt.png)

여기서 관련 사용권 계약을 다운로드하여 수락하려면 자산을 선택해야 합니다. 사용권 계약에 동의하지 않으면 **[!UICONTROL 다운로드]** 단추가 활성화되지 않습니다.

![](assets/licensed-asset-download-2.png)

선택한 항목에 여러 개의 보호된 자산이 포함되어 있는 경우 한 번에 한 개의 자산을 선택하고 사용권 계약에 동의한 다음 자산 다운로드를 계속 진행합니다.

## 만료된 자산에 대한 보고서 생성 {#generate-report-about-expired-assets}

관리자는 특정 기간 내에 만료된 모든 자산을 나열하는 보고서를 생성하고 다운로드할 수 있습니다. 이 보고서에는 자산 계층 구조에서 자산 위치를 지정하는 경로, 크기, 유형, 자산 만료 시기, 자산이 게시된 시기 등 만료된 자산에 대한 자세한 정보가 포함되어 있습니다. 이 보고서의 열을 사용자 지정하여 사용자 요구 사항에 따라 더 많은 데이터를 표시할 수 있습니다.

![](assets/assets-expired.png)

보고서 기능에 대한 자세한 내용은 [보고서를 사용한 작업](../using/brand-portal-reports.md#work-with-reports)을 참조하십시오.
