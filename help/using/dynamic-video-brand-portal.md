---
title: Brand Portal에서 동적 비디오 지원
seo-title: Dynamic video support on Brand Portal
description: Brand Portal에서 동적 비디오 지원
seo-description: Dynamic video support on Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
exl-id: 08d6a0fb-061e-4bef-b8e2-bb8522e7482e
source-git-commit: 8924ff9c78c065895dd0f8d1099a5488b34a34e2
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 4%

---

# Brand Portal에서 동적 비디오 지원 {#dynamic-video-support-on-brand-portal}

Dynamic Media 지원을 통해 Brand Portal에서 비디오를 적응적으로 미리 보고 재생할 수 있습니다. 또한 포털 및 공유 링크에서 동적 변환을 다운로드합니다.
Brand Portal 사용자는 다음 작업을 수행할 수 있습니다.

* 자산 세부 사항 페이지, 카드 보기 및 링크 공유 미리 보기 페이지에서 비디오를 미리 봅니다.
* 자산 세부 사항 페이지에서 비디오 인코딩 재생
* 에셋 세부 정보 페이지의 렌디션 탭에서 동적 렌디션을 봅니다.
* 비디오가 포함된 비디오 인코딩 및 폴더를 다운로드합니다.

>[!NOTE]
>
>비디오로 작업하고 Brand Portal에 게시하려면 Experience Manager 작성자 인스턴스가 Dynamic Media 하이브리드 모드 또는 Dynamic Media에서 설정되어 있는지 확인하십시오 **[!DNL Scene7]** 모드.

Brand Portal은 비디오를 미리 보고, 재생하고, 다운로드하기 위해 다음 두 가지 구성을 관리자에게 제공합니다.

* [Dynamic Media 하이브리드 구성](#configure-dm-hybrid-settings)
Experience Manager 작성자 인스턴스가 Dynamic Media 하이브리드 모드에서 실행 중인 경우.
* [Dynamic Media [!DNL Scene7] 구성](#configure-dm-scene7-settings)
Experience Manager 작성자 인스턴스가 Dynamic Media에서 실행 중인 경우 -**[!DNL Scene7]** 모드.
Brand Portal 테넌트가 복제되는 Experience Manager 작성자 인스턴스에 설정한 구성을 기반으로 이러한 구성 중 하나를 설정합니다.

>[!NOTE]
>
>에서 실행 중인 Experience Manager 작성자로 구성된 Brand Portal 테넌트에서는 동적 비디오가 지원되지 않습니다. **[!UICONTROL Scene7 연결]** 실행 모드.

## 다이내믹 비디오는 어떻게 재생됩니까? {#how-are-dynamic-videos-played}

![클라우드에서 비디오 인코딩을 가져옵니다.](assets/VideoEncodes.png)

Dynamic Media 구성인 경우([하이브리드](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) 또는 [[!DNL Scene7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) configurations)가 Brand Portal에 설정되어 있을 때 동적 변환을 가져올 수 있습니다. **[!DNL Scene7]** 서버입니다. 따라서 비디오 인코딩은 품질에서 지연 및 왜곡 없이 미리 보고 재생됩니다.

비디오 인코딩은 Brand Portal 저장소에 저장되지 않고에서 가져옵니다. **[!DNL Scene7]** 서버: Adobe Experience Manager 작성자 인스턴스와 Brand Portal의 Dynamic Media 구성이 동일한지 확인합니다.

>[!NOTE]
>
>비디오 뷰어 및 뷰어 사전 설정은 Brand Portal에서 지원되지 않습니다. 비디오는 Brand Portal의 기본 뷰어에서 미리 보고 재생됩니다.

## 사전 요구 사항 {#prerequisites}

Brand Portal에서 동적 비디오로 작업하려면 다음을 확인하십시오.

* **Dynamic Media 모드에서 Experience Manager 작성자 시작**
다음 위치에서 Experience Manager 작성자 인스턴스(Brand Portal 구성 시) 시작 [DYNAMIC MEDIA - [!DNL Scene7] 모드](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=en#enabling-dynamic-media-in-scene-mode) 또는 [Dynamic Media - 하이브리드 모드](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) 또는
* **Experience Manager 작성자에 대한 Dynamic Media Cloud Services 구성**
Experience Manager 작성자가 실행 중인 Dynamic Media 모드(Scene7 모드 또는 하이브리드 모드)에 따라 다음 중 하나를 설정합니다. [DYNAMIC MEDIA CLOUD SERVICES ([!DNL Scene7] mode)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=ko#configuring-dynamic-media-cloud-services) 또는 [Dynamic Media Cloud Services(하이브리드 모드)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html?lang=en#configuring-dynamic-media-cloud-services) Experience Manager 작성자 위치 **도구** | **Cloud Services** | **Dynamic Media**.
* **Brand Portal에서 Dynamic Media 구성**
Experience Manager 작성자의 Dynamic Media 클라우드 구성을 기반으로 다음을 구성하십시오. [Dynamic Media 설정](#configure-dm-hybrid-settings) 또는 [[!DNL Scene7] 설정](#configure-dm-scene7-settings) Brand Portal 관리 도구에서.
다음을 확인합니다. [Brand Portal 테넌트 구분](#separate-tenants) Dynamic Media에 구성된 Experience Manager 작성자 인스턴스에 사용됩니다. **[!UICONTROL Scene7]** mode 및 Dynamic Media - 하이브리드 모드. 특히 Dynamic Media의 기능을 사용하는 경우 **[!UICONTROL S7]** 및 Dynamic Media Hybrid.
* **Brand Portal에 비디오 인코딩이 적용된 폴더 게시**
적용 [비디오 인코딩](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) Experience Manager 작성자 인스턴스의 리치 미디어 자산이 포함된 폴더를 Brand Portal에 게시합니다.
* **허용 목록에 추가하다 보안 미리 보기가 활성화된 경우 SPS의 이그레스 IP**
Dynamic Media을 사용하는 경우-**[!DNL Scene7]** (와) [보안 미리 보기 활성화됨](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) (회사의 경우), 다음 사항을 권장합니다. **[!DNL Scene7]** 회사 관리자 [허용 목록에 추가하다 공개 이그레스 IP](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) SPS를 사용하는 각 지역의 경우(**[!UICONTROL Scene7]** Publishing System) 플래시 UI.
이그레스 IP는 다음과 같습니다.

| **지역** | **이그레스 IP** |
|--- |--- |
| NA | 130.248.160.68,  20.94.203.130 |
| EMEA | 185.34.189.3,  51.132.146.75 |
| APAC | 63.140.44.54 |

이러한 이그레스 IP 중 하나를 허용 목록에 추가하려면 [보안 테스트 서비스를 위한 계정 준비](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## 모범 사례

Brand Portal(및 공유 링크)에서 다이내믹 비디오 자산을 성공적으로 미리 보고, 재생하고, 다운로드하려면 다음 사례를 따르십시오.

### Dynamic Media - Scene7 및 Dynamic Media - 하이브리드 모드에 대한 별도의 테넌트 {#separate-tenants}

Dynamic Media을 모두 사용하는 경우 - **[!DNL Scene7]** 모드 및 Dynamic Media - 하이브리드 모드 기능, Dynamic Media으로 구성된 Experience Manager 작성자 인스턴스용 다양한 Brand Portal 테넌트 사용 - **[!DNL Scene7]** 및 Dynamic Media - 하이브리드 모드.


![작성자 및 BP 일대일 매핑](assets/BPDynamicMedia.png)

### Experience Manager 작성자 인스턴스 및 Brand Portal의 동일한 구성 세부 정보

Brand Portal 및 의 구성 세부 정보가 동일한지 확인합니다. **[!UICONTROL Experience Manager 클라우드 구성]**. 동일한 구성 세부 사항에는 다음이 포함됩니다.

* **[!UICONTROL 제목]**
* **[!UICONTROL 등록 ID]**
* **[!UICONTROL 비디오 서비스 URL]** 위치: **[!UICONTROL Dynamic Media - 하이브리드 모드]**
* **[!UICONTROL 제목]**
* 자격 증명(**[!UICONTROL 이메일]** 및 암호)
* **[!UICONTROL 지역]**
* **[!UICONTROL 회사]** DYNAMIC MEDIA - **[!DNL Scene7]** 모드

### 허용 목록에 추가하다 Dynamic Media Scene7 모드용 공개 이그레스

If Dynamic Media **[!UICONTROL Scene7]**-having [보안 미리 보기 활성화됨](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)- Brand Portal에 비디오 자산을 제공하는 데 사용됩니다. **[!UICONTROL Scene7]** 스테이징 환경 또는 내부 애플리케이션을 위한 전용 이미지 서버를 설정합니다. 이 서버에 대한 모든 요청은 원본 IP 주소를 확인합니다. 수신 요청이 승인된 IP 주소 목록 내에 없는 경우 실패 응답이 반환됩니다.
다음 **[!UICONTROL Scene7]** 따라서 회사 관리자는 해당 회사의 승인된 IP 주소 목록을 구성합니다 **[!UICONTROL 보안 테스트]** 환경, 다음을 통해 **[!UICONTROL SPS]** (Scene7 Publishing System) flash UI. 각 지역의 이그레스 IP가 해당 승인 목록에 추가되었는지 확인합니다(다음에서).
이러한 이그레스 IP 중 하나를 허용 목록에 추가하려면 [보안 테스트 서비스를 위한 계정 준비](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
이그레스 IP는 다음과 같습니다.

| **지역** | **이그레스 IP** |
|--- |--- |
| NA | 130.248.160.66,  52.151.32.108 |
| EMEA | 185.34.189.1 |
| APAC | 63.140.44.54 |

## Dynamic Media(하이브리드) 설정 구성 {#configure-dm-hybrid-settings}

Experience Manager 작성자 인스턴스가 Dynamic Media 하이브리드 모드에서 실행 중인 경우 다음을 사용합니다 **[!UICONTROL 비디오]** 관리 도구 패널의 타일을 사용하여 Dynamic Media 게이트웨이 설정을 구성합니다.

>[!NOTE]
>
>다음 [비디오 인코딩 프로필](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) Brand Portal에 게시되지 않고 대신 **[!UICONTROL Scene7]** 서버입니다. 따라서 비디오 인코딩이 Brand Portal에서 성공적으로 재생되도록 하려면 구성 세부 사항이 와 동일한지 확인합니다. [DYNAMIC MEDIA CLOUD SERVICES ([!DNL Scene7] mode)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=ko#configuring-dynamic-media-cloud-services) Experience Manager 작성자 인스턴스에서 확인할 수 있습니다.

Brand Portal 테넌트에 대해 Dynamic Media 구성을 설정하려면 다음을 수행하십시오.

1. Brand Portal의 맨 위에 있는 도구 모음에서 관리 도구에 액세스할 수 있도록 Experience Manager 로고를 선택합니다.
1. 관리 도구 패널에서 **[!UICONTROL 비디오]** 타일.

   ![Brand Portal의 Dynamic Media 하이브리드 구성](assets/DMHybrid-Video.png)

   **[!UICONTROL Dynamic Media 구성 편집]** 페이지가 열립니다.

   ![Brand Portal의 Dynamic Media 하이브리드 구성](assets/edit-dynamic-media-config.png)

1. 지정 **[!UICONTROL 등록 ID]** 및 **[!UICONTROL 비디오 서비스 URL]** (DM-Gateway URL). 이러한 세부 사항이 의 세부 사항과 동일한지 확인합니다. **[!UICONTROL 도구 > Cloud Services]** Experience Manager 작성자 인스턴스에서 확인할 수 있습니다.
1. 선택 **저장** 구성을 저장합니다.

## Dynamic Media Scene7 설정 구성 {#configure-dm-scene7-settings}

Experience Manager 작성자 인스턴스가 Dynamic Media에서 실행 중인 경우 - **[!UICONTROL Scene7]** 모드, 사용 **[!UICONTROL Dynamic Media 구성]** 을 구성하려면 관리 도구 패널에서 타일을 수행합니다. **[!UICONTROL Scene7]** 서버 설정.

Dynamic Media을 설정하려면 **[!UICONTROL Scene7]** Brand Portal 테넌트에 대한 구성:

1. Brand Portal의 맨 위에 있는 도구 모음에서 관리 도구에 액세스할 수 있도록 Experience Manager 로고를 선택합니다.

2. 관리 도구 패널에서 **[!UICONTROL Dynamic Media 구성]** 타일.

   ![DM [!UICONTROL 장면 7] Brand Portal에서 구성](assets/DMS7-Tile.png)

   **[!UICONTROL Dynamic Media 구성 편집]** 페이지가 열립니다.

   ![Brand Portal의 Scene 7 구성](assets/S7Config.png)

3. 제공:

   * **[!UICONTROL 제목]**
   * 자격 증명(**[!UICONTROL 이메일 ID]** 및 **[!UICONTROL 암호]**) Scene7 서버에 액세스하기 위해
   * **[!UICONTROL 지역]**

   이러한 값이 Experience Manager 작성자 인스턴스에 있는 값과 동일한지 확인합니다.

4. 선택 **[!UICONTROL Dynamic Media에 연결]**.

5. 다음을 제공합니다 **[!UICONTROL 회사 이름]**, 및 **[!UICONTROL 저장]** 구성.
