---
title: 링크로 자산 공유
seo-title: Share assets as a link
description: Adobe Experience Manager Assets Brand Portal 관리자는 승인된 내부 사용자 및 외부 엔터티(파트너 및 공급업체 포함)와 여러 에셋의 링크를 공유할 수 있습니다. 편집자는 공유된 에셋만 보고 공유할 수 있습니다.
seo-description: Adobe Experience Manager Assets Brand Portal Administrators can share links of multiple assets with authorized internal users and external entities, including partners and vendors. Editors can view and share only the assets shared with them.
uuid: 8889ac24-c56d-4a47-b792-80c34ffb5c3f
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f3573219-3c58-47ba-90db-62b003d8b9aa
exl-id: 9d254e95-a4fc-468d-ae1f-9690ddd3b4a1
source-git-commit: e3e35ad4be5c082ad7bac7bed8ea20a186d245ad
workflow-type: tm+mt
source-wordcount: '969'
ht-degree: 5%

---

# 링크로 자산 공유 {#share-assets-as-a-link}

Adobe Experience Manager Assets Brand Portal 관리자는 승인된 내부 사용자 및 외부 엔터티(파트너 및 공급업체 포함)와 여러 에셋의 링크를 공유할 수 있습니다. 편집자는 공유된 에셋만 보고 공유할 수 있습니다.

링크를 통해 에셋을 공유하면 수신자가 에셋에 액세스하기 위해 Brand Portal에 로그인할 필요가 없기 때문에 외부 당사자가 에셋을 사용할 수 있는 편리한 방법입니다.

<!-- Link sharing access is restricted to editors and administrators. 
-->

자세한 내용은 [사용자, 그룹 및 사용자 역할 관리](../using/brand-portal-adding-users.md#manage-user-roles).


다음은 링크로 자산을 공유하는 절차입니다.

1. Brand Portal 테넌트에 로그인합니다. 기본적으로 **[!UICONTROL 파일]** 보기는 게시된 모든 에셋과 폴더를 포함하는 열립니다.

1. 공유할 에셋 또는 폴더를 선택하거나 **[!UICONTROL 컬렉션]** 을(를) 보고 생성한 컬렉션을 공유할 수 있습니다.

   ![여러 자산 선택](assets/select-assets-new.png)

1. 맨 위에 있는 도구 모음에서 **[!UICONTROL 링크 공유]** 아이콘.

   다음 **[!UICONTROL 링크 공유]** 대화 상자가 나타납니다.

   ![](assets/link-sharing.png)

   * 이메일 주소 상자에 링크를 공유할 사용자의 이메일 ID를 입력합니다. You can share the link with multiple users. 사용자가 조직의 멤버인 경우 드롭다운 목록에 표시되는 제안 사항에서 이메일 ID를 선택합니다. 사용자가 외부 사용자인 경우 전체 이메일 ID를 입력하고 키를 누릅니다 **[!UICONTROL 입력]**; 이메일 ID가 사용자 목록에 추가됩니다.

      ![](assets/link-sharing-text.png)

   * 다음에서 **[!UICONTROL 제목]** 상자에 공유할 에셋의 제목을 입력합니다.
   * 다음에서 **[!UICONTROL 메시지]** 필요한 경우 상자에 메시지를 입력합니다.
   * 다음에서 **[!UICONTROL 만료]** 필드에서 날짜 선택기를 사용하여 링크의 만료 날짜 및 시간을 지정합니다. 기본적으로 만료일은 링크를 공유한 날로부터 7일로 설정됩니다.
   * 활성화 **[!UICONTROL 원본 파일 다운로드 허용]** 수신자가 원본 렌디션을 다운로드할 수 있도록 하려면 확인란을 선택합니다.

   링크를 통해 공유된 에셋은에 지정된 날짜 및 시간을 지나면 만료됩니다. **[!UICONTROL 만료]** 필드. Brand Portal에서 사용자 역할에 따라 허용되는 활동의 만료 에셋 동작 및 변경 사항에 대한 자세한 내용은 을 참조하십시오. [자산의 디지털 권한 관리](../using/manage-digital-rights-of-assets.md#asset-expiration).

   >[!NOTE]
   >
   >링크의 기본 만료 시간은 7일입니다. 링크는 를 사용하여 사용자에게 이메일로 전송해야 합니다. **[!UICONTROL 링크 공유]** 대화 상자에서 링크를 별도로 복사하고 공유하지 마십시오.

1. 클릭 **[!UICONTROL 공유]**. 링크가 사용자와 공유되었음을 확인하는 메시지가 표시됩니다. 사용자는 공유 링크가 포함된 이메일을 받습니다.

   ![](assets/link-share-email.png)

   >[!NOTE]
   >
   >관리자는 을 사용하여 로고, 설명 및 바닥글 사용자 지정이 포함된 이메일 메시지를 사용자 지정할 수 있습니다 [브랜딩](../using/brand-portal-branding.md) 기능.

## 공유 링크에서 에셋 다운로드 {#download-assets-from-shared-links}

이메일의 링크를 클릭하여 공유 에셋에 액세스합니다. AEM Link 공유 페이지가 열립니다.

공유 에셋을 다운로드하려면 다음 작업을 수행하십시오.

1. 에셋 또는 폴더를 클릭한 다음 **[!UICONTROL 다운로드]** 아이콘을 클릭합니다.

   ![](assets/download-share-link.png)

   >[!NOTE]
   >
   >현재 파일 형식에 따라 특정 에셋에 대해서만 미리 보기 및 썸네일을 생성할 수 있습니다. 지원되는 파일 형식에 대한 자세한 내용은 [자산 형식에 대한 미리보기 및 썸네일 지원](#preview-thumbnail-support).

1. 다음 **[!UICONTROL 다운로드]** 대화 상자가 나타납니다.

   ![download-dialog](assets/download-dialog-box-new.png)

1. 기본적으로 **[!UICONTROL 빠른 다운로드]** 설정은 다음에서 활성화됩니다. **[!UICONTROL 다운로드 설정]**. 따라서 IBM Aspera Connect를 사용하여 다운로드를 계속하는 확인 상자가 나타납니다.

   을(를) 계속하려면 **[!UICONTROL 빠른 다운로드]**, 클릭 **[!UICONTROL 허용]**.

   선택한 모든 렌디션은 각 에셋에 대해 별도의 폴더가 포함된 zip 폴더로 다운로드됩니다.

   >[!NOTE]
   >
   >공유 링크에서 에셋을 다운로드하는 동안 각 에셋에 대해 별도의 폴더가 만들어집니다.
   >
   >폴더, 컬렉션 또는 20개가 넘는 자산을 다운로드하도록 선택한 경우 **[!UICONTROL 다운로드]** 대화 상자를 건너뛰고 동적 렌디션을 제외한 사용자가 액세스할 수 있는 모든 에셋 렌디션은 각 에셋에 대한 별도의 폴더가 포함된 zip 폴더로 다운로드됩니다.

   >[!NOTE]
   >
   >자산을 링크로 공유한 사용자가 이 링크를 사용하지 않으면 원본 렌디션이 공유 링크를 사용하여 다운로드되지 않습니다 [관리자가 원본 렌디션에 대한 액세스 권한을 부여함](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges).


>[!NOTE]
>
>Brand Portal은 링크 공유를 사용하여 크기가 5GB보다 큰 폴더 또는 에셋의 다운로드를 제한합니다.

<!--
1. The **[!UICONTROL Download]** dialog box appears.

   ![](assets/download-linkshare.png)

    * To speed up the download of asset files shared as the link, select **[!UICONTROL Enable download acceleration]** option and [follow the wizard](../using/accelerated-download.md#download-workflow-using-file-accelerator). To know more about the fast download of assets on Brand Portal refer [Guide to accelerate downloads from Brand Portal](../using/accelerated-download.md).
    
1. To download the renditions of assets in addition to the assets from the shared link, select **[!UICONTROL Rendition(s)]** option. When you do so, **[!UICONTROL Exclude System Renditions]** option appears that is selected by default. This prevents the download of out-of-the-box renditions along with approved assets or their custom renditions.

   However, to allow auto-generated renditions to download along with custom renditions, deselect the **[!UICONTROL Exclude System Renditions]** option.

   >[!NOTE]
   >
   >Original renditions are not downloaded using the shared link if the user who shared the assets as a link is not [authorized by the administrator to have access to the original renditions](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges).

   ![](assets/download-linkshare-autoren.png)

1. Click **[!UICONTROL Download]**. The assets (and renditions if selected) are downloaded as a ZIP file to your local folder. However, no zip file is created if a single asset is downloaded without any of the renditions, thereby ensuring speedy download.

-->

## 자산 형식에 대한 미리보기 및 썸네일 지원 {#preview-thumbnail-support}

다음 매트릭스에는 Brand Portal이 썸네일 및 미리보기를 지원하는 자산 형식이 나와 있습니다.

| 자산 형식 | 썸네일 지원 | 미리보기 지원 |
|--------------|-------------------|-----------------|
| PNG | ✓ | ✓ |
| GIF | ✓ | ✓ |
| TIFF | ✓ | ✕ 덧신 |
| JPEG | ✓ | ✓ |
| BMP | ✓ | ✕ |
| PNM* | NA | NA |
| PGM* | NA | NA |
| PBM* | NA | NA |
| PPM* | NA | NA |
| PSD | ✓ | ✕ |
| EPS | NA | ✕ |
| DNG | ✓ | ✕ |
| PICT | ✓ | ✕ |
| PSB* | ✓ | ✕ |
| JPG | ✓ | ✓ |
| AI | ✓ | ✕ |
| DOC | ✕ | ✕ |
| DOCX | ✕ | ✕ |
| ODT* | ✕ | ✕ |
| PDF | ✓ | ✕ |
| HTML | ✕ | ✕ |
| RTF | ✕ | ✕ |
| TXT | ✓ | ✕ |
| XLS | ✕ | ✕ |
| XLSX | ✕ | ✕ |
| ODS | ✕ | ✕ |
| PPT | ✓ | ✕ |
| PPTX | ✕ | ✕ |
| ODP | ✕ | ✕ |
| INDD | ✓ | ✕ |
| PS | ✕ | ✕ |
| QXP | ✕ | ✕ |
| EPUB | ✓ | ✕ |
| AAC | ✕ | ✕ |
| MIDI | ✕ | ✕ |
| 3GP | ✕ | ✕ |
| MP3 | ✕ | ✕ |
| MP4 | ✕ | ✕ |
| OGA | ✕ | ✕ |
| OGG | ✕ | ✕ |
| RA | ✕ | ✕ |
| WAV | ✕ | ✕ |
| WMA | ✕ | ✕ |
| DVI | ✕ | ✕ |
| FLV | ✕ | ✕ |
| M4V | ✕ | ✕ |
| 마일 | ✕ | ✕ |
| OGV | ✕ | ✕ |
| MOV | ✕ | ✕ |
| WMV | ✕ | ✕ |
| SWF | ✕ | ✕ |
| TGZ | NA | ✕ |
| JAR | ✓ | ✕ |
| RAR | NA | ✕ |
| TAR | NA | ✕ |
| ZIP | ✓ | ✕ |

다음 범례에서는 행렬에 사용되는 기호에 대해 설명합니다.

| 기호 | 의미 |
|---|---|
| ✓ | 이 파일 형식은 이 기능을 지원합니다. |
| ✕ | 이 파일 형식은 이 기능을 지원하지 않습니다. |
| NA | 이 기능은 이 파일 형식에 적용할 수 없습니다. |
| &#42; | 이 기능을 사용하려면 AEM 작성자 인스턴스에서 이 파일 형식에 대한 추가 기능이 지원되어야 하지만 자산이 Brand Portal에 게시된 후 Brand Portal에서는 지원되지 않습니다 |

## 링크로 공유된 에셋 공유 해제 {#unshare-assets-shared-as-a-link}

링크로 이전에 공유한 에셋의 공유를 해제하려면 다음을 수행하십시오.

1. Brand Portal에 로그인하면 **[!UICONTROL 파일]** 기본적으로 보기가 열립니다. 링크로 공유한 자산을 보려면 **[!UICONTROL 공유 링크]** 보기.

1. 표시된 목록에서 공유한 링크를 검토합니다.

   ![](assets/shared-links.png)

1. 목록에서 링크 공유를 취소하려면 링크를 선택하고 **[!UICONTROL 공유 안 함]** 아이콘을 클릭합니다.

   ![](assets/unshare-asset.png)

   >[!NOTE]
   >
   >공유 링크는 사용자별로 표시됩니다. 이 기능은 테넌트의 모든 사용자가 공유하는 모든 링크를 표시하지 않습니다.

1. 경고 메시지 상자에서 **[!UICONTROL 계속]** 공유 취소를 확인합니다. 링크 항목이 공유 링크 목록에서 제거됩니다.
