---
title: 자산의 디지털 권한 관리
seo-title: 자산의 디지털 권한 관리
description: 에셋 라이선스 및 에셋 및 공유 링크에 대한 만료 설정을 통해 이러한 에셋을 관리하고 안전하게 보호할 수 있습니다.
seo-description: 에셋 라이선스 및 에셋 및 공유 링크에 대한 만료 설정을 통해 이러한 에셋을 관리하고 안전하게 보호할 수 있습니다.
uuid: CE 30 E 398-0109-41 BF-A 4 D 2-2 FCCA 476 F 499
contentOwner: BDHAR
topic-tags: download-install
products: sg_ Experiencemanager/brand_ portal
content-type: 참조
discoiquuid: F 77003 BA -31 FE -4 A 9 E -96 C 8-DBC 4 C 2 EBA 79 E
translation-type: tm+mt
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# 자산의 디지털 권한 관리 {#manage-digital-rights-of-assets}

브랜드를 보호하기 위해서는 크리에이티브 에셋과 브랜드 자료를 안전하게 배포하고 사용해야 합니다. 만료 날짜 (및 시간) 를에 [!DNL AEM] 게시된 승인된 자산에 연관시키거나, 조건부 사용을 위해 이러한 자산에 라이선스를 부여함으로써 [!DNL Brand Portal]조직 및 외부에서 실시할 수 있습니다. 또한, 공유된 [!DNL Brand Portal] 자산에 대한 링크에 대한 만료 날짜를 지정할 [!DNL Brand Portal]수도 있습니다.

자산이 어떻게 보호되고 관련 사용 권한을 [!DNL Brand Portal] 이해하는지 알아보려면 읽어 보십시오.

## 자산 만료 {#asset-expiration}

자산 만료는 조직 전체에서 브랜드 포털에서 승인된 자산의 사용을 제어하는 효과적인 방법입니다. 자산에서 [!DNL AEM] 브랜드 포털에 게시된 모든 자산에 만료일을 지정하여 다른 사용자 역할별로 이러한 자산의 사용을 제한할 수 있습니다.

### 만료된 자산과 관련된 사용 권한 {#usage-permissions-expired-assets}

에서 [!DNL Brand Portal], 관리자는 만료된 자산을 보고, 다운로드하고, 컬렉션에 추가할 수 있습니다. 반면에 편집자와 뷰어는 만료된 에셋을 보고 컬렉션에 추가할 수만 있습니다.

관리자는 만료된 에셋을 자산에서 [!DNL AEM] 에 게시할 [!DNL Brand Portal]수 있습니다. 그러나 만료된 자산은 잉크를 통해 공유할 수 [!DNL Brand Portal]없습니다. 만료되거나 만료되지 않은 에셋을 모두 포함하는 폴더에서 만료된 에셋을 선택하면 링크 **[!UICONTROL 공유]** 작업을 사용할 수 없습니다. 그러나 만료되거나 만료되지 않은 에셋이 포함된 폴더를 선택하면 [!UICONTROL 공유] 및 **[!UICONTROL 공유 링크]** 작업을 사용할 수 있습니다.

>[!NOTE]
>
>폴더는 만료된 에셋이 포함되어 있어도 링크로 공유할 수 있습니다. 이 경우 링크가 만료된 에셋을 나열하지 않으며 만료된 에셋만 공유됩니다.

다음 표에는 만료된 자산의 사용 권한이 표시됩니다.

|  | **링크 공유** | **다운로드** | **속성** | **컬렉션에 추가** | **삭제** |
|---|---|---|---|---|---|
| **관리자** | 사용할 수 없음 | available | available | available | available |
| **편집자** | 사용할 수 없음 | 사용할 수 없음 | available | available | 사용할 수 없음 |
| **뷰어** | 사용할 수 없음 | 사용할 수 없음 | available | available | 사용할 수 없음 |
| **손님 사용자** | 사용할 수 없음 | 사용할 수 없음 | available | available | 사용할 수 없음 |

>[!NOTE]
>
>뷰어와 편집자가 만료되거나 만료된 에셋이 포함된 폴더를 다운로드하는 경우 만료되지 않은 에셋만 다운로드됩니다. 폴더에 만료된 에셋만 포함된 경우 빈 폴더가 다운로드됩니다.

### 자산의 만료 상태 {#expiration-status-of-assets}

카드 보기에서 자산의 만료 상태를 볼 수 있습니다. 카드에 빨간색 플래그가 있으면 자산이 만료되었음을 나타냅니다.

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>목록 및 열 보기에는 자산의 만료 상태가 표시되지 않습니다.

## 자산 링크 만료 {#asset-link-expiration}

링크를 통해 자산을 공유하는 동안 관리자와 편집자는 링크 공유 대화 상자의 **[!UICONTROL 만료]** 필드를 사용하여 만료 날짜와 시간을 **[!UICONTROL 설정할]** 수 있습니다. 링크의 기본 만료는 링크가 공유된 날짜로부터 7 일입니다.

![](assets/asset-link-sharing.png)

링크를 통해 공유한 에셋은 [!DNL Brand Portal] 관리자 및 편집자가 설정한 날짜와 시간에 만료되며 만료 날짜 이후에 더 이상 보고 다운로드할 수 없습니다. 링크를 통해 공유된 에셋은 조직의 일부가 아닌 외부 사용자가 볼 수도 있으므로, 만료를 지정하여 승인된 자산이 보호되고 지정된 시간 이상으로 알 수 없는 엔티티에 노출되지 않도록 할 수 있습니다.

링크 공유에 대한 자세한 내용은 자산 [공유를 링크로 참조하십시오](../using/brand-portal-link-share.md).

## 라이선스가 부여된 에셋 {#licensed-assets}

라이선스가 부여된 에셋은 브랜드 포털에서 다운로드하기 전에 라이선스 계약을 수락할 수 있습니다. 라이센스 에셋에 대한 본 계약은 공유 링크를 통해 [!DNL Brand Portal] 또는 공유 링크를 통해 직접 에셋을 다운로드할 때 제공됩니다. 만료되었거나 만료되지 않은 경우, 라이센스가 보호된 자산은 모든 사용자가 볼 수 있습니다. 그러나 만료된 라이센스 에셋의 다운로드 및 사용은 제한됩니다. 만료된 라이센스 에셋의 비헤이비어와 사용자 역할을 기반으로 허용되는 활동의 영향에 대해 알려면, 만료된 에셋의 [사용 권한을 참조하십시오](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets).

라이센스 보호된 자산은 자산에 [연결된 라이센스 계약을](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) 가지며, 이는 자산에 자산의 [메타데이터 속성을](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) 설정하여 [!DNL AEM] 수행됩니다.

라이센스 보호된 에셋을 다운로드하도록 선택하면 [!UICONTROL 저작권 관리] 페이지로 리디렉션됩니다.

![](assets/asset-copyright-mgmt.png)

여기에서 에셋을 선택하여 관련 라이선스 계약을 다운로드하고 수락해야 합니다. 사용권 계약에 동의하지 않으면 **[!UICONTROL 다운로드]** 단추가 활성화되지 않습니다.

![](assets/licensed-asset-download-2.png)

선택한 항목에 보호된 자산이 여러 개 포함되어 있는 경우 한 번에 하나의 자산을 선택하고 사용권 계약에 동의하며 계속해서 에셋을 다운로드하십시오.

## 만료된 자산에 대한 보고서 생성 {#generate-report-about-expired-assets}

관리자는 특정 기간 내에 만료되는 모든 자산이 나열된 보고서를 생성하고 다운로드할 수 있습니다. 이 보고서에는 크기, 유형, 자산 계층 내의 자산 위치 지정, 자산이 만료되는 시기, 자산이 게시된 시기 (만료된 자산) 등과 같은 세부 정보가 포함됩니다. 사용자 요구 사항을 기반으로 더 많은 데이터를 표시하도록 이 보고서의 열을 사용자 지정할 수 있습니다.

![](assets/assets-expired.png)

보고서 기능에 대한 자세한 내용은 보고서 [작업을 참조하십시오](../using/brand-portal-reports.md#work-with-reports).
