---
title: 자산의 디지털 권한 관리
description: 에셋 및 공유 링크에 대한 라이센스 부여 및 만료 설정은 이러한 에셋의 제어된 사용을 보장하고 보호합니다.
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
role: Admin
exl-id: 86c31891-0627-41ca-b571-8dac3a074d55
source-git-commit: 10f89ded6febb1a024cbe181fa48a290d90223f0
workflow-type: tm+mt
source-wordcount: '887'
ht-degree: 3%

---

# 자산의 디지털 권한 관리 {#manage-digital-rights-of-assets}

크리에이티브 자산 및 브랜드 자료의 안전한 배포 및 사용은 브랜드를 보호하는 데 중요합니다. 이 프로세스는 만료 날짜(및 시간)를 AEM에서 Brand Portal으로 게시된 승인된 자산과 연결하거나, 이러한 자산에 조건부 사용을 위한 라이센스를 부여하여 강제 적용할 수 있습니다. 또한 Brand Portal을 사용하여 Brand Portal에서 공유한 에셋으로의 링크에 대한 만료 날짜를 지정할 수 있습니다.

Brand Portal에서 자산이 어떻게 보호되는지 알아보고 관련 사용 권한을 이해하려면 계속 읽어 보십시오.

## 에셋 만료 {#asset-expiration}

에셋 만료는 조직 전체에서 Brand Portal에서 승인된 에셋의 사용을 제어하는 효과적인 방법입니다. AEM Assets에서 Brand Portal으로 게시된 모든 에셋에는 만료 날짜가 있을 수 있으며, 이로 인해 다른 사용자 역할로 이러한 에셋 사용이 제한됩니다.

### 만료된 에셋 관련 사용 권한 {#usage-permissions-expired-assets}

Brand Portal에서 관리자는 만료된 에셋을 보고 다운로드하고 컬렉션에 추가할 수 있습니다. 그러나 편집자와 뷰어는 만료된 에셋을 보고 컬렉션에 추가할 수만 있습니다.

관리자는 만료된 에셋을 AEM Assets에서 Brand Portal에 게시할 수 있습니다. 그러나 만료된 에셋은 Brand Portal의 링크를 사용하여 공유할 수 없습니다. 만료된 에셋과 만료되지 않은 에셋이 모두 들어 있는 폴더에서 만료된 에셋을 선택하는 경우 **[!UICONTROL 링크 공유]** 작업을 사용할 수 없습니다. 그러나 만료된 에셋과 만료되지 않은 에셋이 포함된 폴더를 선택하면 [!UICONTROL 공유] 및 **[!UICONTROL 링크 공유]** 작업을 사용할 수 있습니다.

>[!NOTE]
>
>만료된 에셋이 포함된 폴더는 여전히 링크로 공유할 수 있습니다. 이 경우 링크는 만료된 에셋을 나열하지 않고 만료되지 않은 에셋만 공유합니다.

다음 표에는 만료된 에셋의 사용 권한이 표시됩니다.

|   | **[!UICONTROL 공유 연결]** | **[!UICONTROL 다운로드]** | **[!UICONTROL 속성]** | **[!UICONTROL 컬렉션에 추가]** | **[!UICONTROL 삭제]** |
|---|---|---|---|---|---|
| **[!UICONTROL 관리자]** | 사용할 수 없음 | 사용 가능 | 사용 가능 | 사용 가능 | 사용 가능 |
| **[!UICONTROL 편집기]** | 사용할 수 없음 | 사용할 수 없음 | 사용 가능 | 사용 가능 | 사용할 수 없음 |
| **[!UICONTROL 뷰어]** | 사용할 수 없음 | 사용할 수 없음 | 사용 가능 | 사용 가능 | 사용할 수 없음 |
| **[!UICONTROL 게스트 사용자]** | 사용할 수 없음 | 사용할 수 없음 | 사용 가능 | 사용 가능 | 사용할 수 없음 |

>[!NOTE]
>
>뷰어 및 편집기 가 만료된 에셋과 만료되지 않은 에셋이 포함된 폴더를 다운로드하는 경우 만료되지 않은 에셋만 다운로드됩니다. 폴더에 만료된 에셋만 포함된 경우 빈 폴더가 다운로드됩니다.

### 에셋의 만료 상태 {#expiration-status-of-assets}

자산의 만료 상태를 **[!UICONTROL 카드 보기]**&#x200B;에서 볼 수 있습니다. 카드의 빨간색 플래그는 자산이 만료되었음을 나타냅니다.

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>목록 및 열 보기에는 에셋의 만료 상태가 표시되지 않습니다.

## 자산 링크 만료 {#asset-link-expiration}

링크를 통해 자산을 공유하는 동안 관리자 및 편집자는 **[!UICONTROL 링크 공유]** 대화 상자의 **[!UICONTROL 만료]** 필드를 사용하여 만료 날짜와 시간을 설정할 수 있습니다. 링크의 기본 만료일은 링크가 공유된 날로부터 7일입니다.

![](assets/asset-link-sharing.png)

링크로 공유되는 에셋이 Brand Portal 관리자 및 편집자가 설정한 날짜 및 시간에 만료되도록 합니다. 또한 에셋은 만료 날짜 이후에 더 이상 보고 다운로드할 수 없습니다. 외부 사용자로부터 승인된 에셋을 보호하려면 공유 링크에 만료 날짜를 설정하여 지정된 시간 이후에 알 수 없는 엔티티에 노출되지 않도록 합니다.

링크 공유에 대한 자세한 내용은 [링크로 자산 공유](../using/brand-portal-link-share.md)를 참조하세요.

## 라이선스가 있는 Assets {#licensed-assets}

라이센스가 부여된 자산은 Brand Portal에서 다운로드하기 전에 라이센스 계약의 동의가 필요합니다. 라이센스가 부여된 에셋에 대한 이 계약은 Brand Portal에서 또는 공유 링크를 통해 에셋을 직접 다운로드할 때 제공됩니다. 만료되었거나 만료되지 않았더라도 모든 사용자는 라이선스로 보호된 에셋을 볼 수 있습니다. 그러나 만료된 라이선스 자산의 다운로드와 사용은 제한됩니다. 사용자 역할에 따라 만료된 라이선스 에셋 및 허용되는 활동의 동작에 대해 알아보려면 [만료된 에셋의 사용 권한](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets)을 참조하세요.

라이선스로 보호된 자산에는 [!DNL Experience Manager Assets]에서 자산의 메타데이터 속성을 설정하여 [라이선스 계약](https://experienceleague.adobe.com/ko/docs/experience-manager-65/content/assets/administer/drm)이 첨부되어 있습니다.

자산에 다음(또는 두 가지 모두) 메타데이터 속성 중 하나가 포함되어 있으면 자산이 보호되는 것으로 간주됩니다.

* `xmpRights:WebStatement`: 이 속성은 자산에 대한 사용권 계약이 포함된 페이지의 경로를 참조합니다. `xmpRights:WebStatement`은(는) 저장소의 올바른 경로여야 합니다.
* `adobe_dam:restrictions`: 이 HTML의 값은 사용권 계약을 지정하는 원시 속성입니다.


라이선스로 보호된 자산을 다운로드하도록 선택한 경우 메타데이터 속성에 따라 **[!UICONTROL 저작권 관리]** 페이지로 리디렉션됩니다.

| `adobe_dam:restrictions` | `xmpRights:WebStatement` | 저작권 관리 |
| --- | --- | --- |
| 예 | - | 인터페이스는 Assets 및 Brand Portal 모두에 표시됩니다 |
| - | 예(잘못된 경로) | 인터페이스 없음 |
| 예 | 예(잘못된 경로) | 인터페이스 없음 |
| 예 | 예(유효한 경로) | 인터페이스가 Assets 또는 Brand Portal에 나타납니다</br>경로가 Assets에 유효한지 Brand Portal에 유효한지 또는 둘 다에 따라 다릅니다. |

![](assets/asset-copyright-mgmt.png)

여기에서 다운로드할 자산을 선택하고 관련 라이선스 계약에 동의해야 합니다. 사용권 계약에 동의하지 않으면 **[!UICONTROL 다운로드]** 단추가 활성화되지 않습니다.

![](assets/licensed-asset-download-2.png)

선택 항목에 여러 개의 보호된 자산이 포함된 경우 한 번에 하나의 자산을 선택하고 라이선스 계약에 동의한 다음 자산 다운로드를 진행합니다.

## 만료된 에셋에 대한 보고서 생성 {#generate-report-about-expired-assets}

관리자는 특정 기간 내에 만료된 모든 에셋을 나열하는 보고서를 생성하고 다운로드할 수 있습니다. 이 보고서에는 만료된 에셋에 대한 크기, 유형, 에셋 계층 구조에서 에셋 위치를 지정하는 경로, 에셋이 만료되는 시기 및 에셋이 게시된 시기와 같은 자세한 정보가 포함됩니다. 사용자 요구 사항에 따라 더 많은 데이터를 표시하도록 이 보고서의 열을 사용자 지정할 수 있습니다.

![](assets/assets-expired.png)

보고서 기능에 대한 자세한 내용을 보려면 [보고서 작업](../using/brand-portal-reports.md#work-with-reports)(으)로 이동하십시오.
