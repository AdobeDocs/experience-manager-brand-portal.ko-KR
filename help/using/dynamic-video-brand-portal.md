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
ht-degree: 3%

---

# Brand Portal에서 동적 비디오 지원 {#dynamic-video-support-on-brand-portal}

Dynamic Media 지원을 통해 Brand Portal에서 적응적으로 비디오를 미리 보고 재생할 수 있습니다. 포털과 공유 링크에서 동적 표현물을 다운로드합니다.
Brand Portal 사용자는

* 자산 세부 사항 페이지, 카드 보기 및 링크 공유 미리 보기 페이지에서 비디오를 미리 봅니다.
* 자산 세부 사항 페이지에서 비디오 인코딩을 재생합니다.
* 자산 세부 사항 페이지의 표현물 탭에서 동적 표현물을 봅니다.
* 비디오가 포함된 비디오 인코딩과 폴더를 다운로드합니다.

>[!NOTE]
>
>비디오를 사용하여 작업하고 Brand Portal에 게시하려면 Experience Manager 작성자 인스턴스가 Dynamic Media 하이브리드 모드 또는 Dynamic Media에 설정되어 있는지 확인하십시오 **[!DNL Scene7]** 모드.

비디오를 미리 보고 재생하고 다운로드하려면 Brand Portal이 관리자에게 다음 두 가지 구성을 표시합니다.

* [Dynamic Media 하이브리드 구성](#configure-dm-hybrid-settings)
Experience Manager 작성자 인스턴스가 dynamic media 하이브리드 모드에서 실행 중인 경우.
* [Dynamic Media [!DNL Scene7] 구성](#configure-dm-scene7-settings)
Dynamic Media에서 Experience Manager 작성자 인스턴스가 실행 중인 경우 -**[!DNL Scene7]** 모드.
Brand Portal 테넌트가 복제되는 Experience Manager 작성자 인스턴스에서 설정한 구성을 기반으로 이러한 구성 중 하나를 설정합니다.

>[!NOTE]
>
>에서 실행되는 Experience Manager 작성자로 구성된 Brand Portal 테넌트에서 동적 비디오가 지원되지 않습니다 **[!UICONTROL Scene7Connect]** 실행 모드.

## 다이내믹 비디오는 어떻게 재생됩니까? {#how-are-dynamic-videos-played}

![비디오 인코딩을 클라우드에서 가져옵니다](assets/VideoEncodes.png)

Dynamic Media 구성([하이브리드](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) 또는 [[!DNL Scene7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) 구성)을 Brand Portal에서 설정하고, 동적 변환을 **[!DNL Scene7]** server. 따라서 비디오 인코딩은 지연과 왜곡없이 미리 보고 재생됩니다.

비디오 인코딩은 Brand Portal 저장소에 저장되지 않고 **[!DNL Scene7]** 서버에서, Adobe Experience Manager 작성자 인스턴스 및 Brand Portal의 Dynamic Media 구성이 동일한지 확인합니다.

>[!NOTE]
>
>Brand Portal에서는 비디오 뷰어 및 뷰어 사전 설정이 지원되지 않습니다. Brand Portal의 기본 뷰어에서 비디오를 미리 보고 재생합니다.

## 전제 조건 {#prerequisites}

Brand Portal에서 다이내믹 비디오를 사용하여 작업하려면 다음을 수행하십시오.

* **Dynamic Media 모드에서 Experience Manager 작성자 시작**
의 Experience Manager 작성자 인스턴스(Brand Portal이 구성된 인스턴스)를 시작합니다. [Dynamic Media - [!DNL Scene7] 모드](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=en#enabling-dynamic-media-in-scene-mode) 또는 [Dynamic Media - 하이브리드 모드](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) 또는
* **Experience Manager 작성자에 대한 Dynamic Media Cloud Services 구성**
Dynamic Media 모드(Scene7 모드 또는 하이브리드 모드) Experience Manager 작성자가 실행 중인를 기반으로 다음 중 하나를 설정합니다 [Dynamic Media Cloud Services ([!DNL Scene7] mode)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=en#configuring-dynamic-media-cloud-services) 또는 [Dynamic Media Cloud Services(하이브리드 모드)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html?lang=en#configuring-dynamic-media-cloud-services) 작성자 Experience Manager 시 **도구** | **Cloud Services** | **Dynamic Media**.
* **Brand Portal에서 Dynamic Media 구성**
Experience Manager 작성자의 Dynamic Media 클라우드 구성에 따라 다음을 구성합니다 [Dynamic Media 설정](#configure-dm-hybrid-settings) 또는 [[!DNL Scene7] 설정](#configure-dm-scene7-settings) Brand Portal 관리 도구 사용.
확인 [별도의 Brand Portal 테넌트](#separate-tenants) Dynamic Media에 구성된 Experience Manager 작성자 인스턴스에 사용됩니다. **[!UICONTROL Scene7]** 모드 및 Dynamic Media - 하이브리드 모드. 특히 Dynamic Media의 기능을 사용하는 경우 **[!UICONTROL S7]** 및 Dynamic Media Hybrid입니다.
* **Brand Portal에 적용된 비디오 인코딩을 사용하여 폴더 게시**
적용 [비디오 인코딩](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) 및 Experience Manager 작성자 인스턴스의 리치 미디어 자산이 포함된 폴더를 Brand Portal에 게시합니다.
* **보안 미리 허용 목록에 추가하다 보기가 활성화된 경우 SPS에서 IP 송신**
Dynamic Media을 사용하는 경우**[!DNL Scene7]** (다음 포함) [보안 미리 보기 사용](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) 회사)의 경우 **[!DNL Scene7]** 회사 관리자 [공용 송신 허용 목록에 추가하다 IP](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) SPS를 사용하는 각 지역(**[!UICONTROL Scene7]** Publishing System) 플래시 UI입니다.
송신 IP는 다음과 같습니다.

| **지역** | **송신 IP** |
|--- |--- |
| NA | 130.248.160.68, 20.94.203.130 |
| EMEA | 185.34.189.3, 51.132.146.75 |
| APAC | 63.140.44.54 |

이러한 송신 IP 중 하나를 허용하려면 다음을 참조하십시오 [보안 테스트 서비스를 위한 계정 준비](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## 우수 사례

Brand Portal(및 공유 링크)에서 다이내믹 비디오 자산을 성공적으로 미리 보고, 재생하고 다운로드하도록 하려면 다음 방법을 따르십시오.

### Dynamic Media - Scene7 및 Dynamic Media - 하이브리드 모드에 대한 별도의 테넌트 {#separate-tenants}

Dynamic Media을 모두 사용하는 경우 - **[!DNL Scene7]** 모드 및 Dynamic Media - 하이브리드 모드 기능은 Dynamic Media으로 구성된 Experience Manager 작성자 인스턴스에 대해 다른 Brand Portal 테넌트를 사용합니다. **[!DNL Scene7]** 및 Dynamic Media - 하이브리드 모드.


![작성자 및 BP 1에서 1로의 매핑](assets/BPDynamicMedia.png)

### Experience Manager 작성자 인스턴스 및 Brand Portal에서 동일한 구성 세부 사항

구성 세부 사항이 Brand Portal 및 **[!UICONTROL Experience Manager 클라우드 구성]**. 동일한 구성 세부 사항에는 다음이 포함됩니다.

* **[!UICONTROL 제목]**
* **[!UICONTROL 등록 ID]**
* **[!UICONTROL 비디오 서비스 URL]** in **[!UICONTROL Dynamic Media - 하이브리드 모드]**
* **[!UICONTROL 제목]**
* 자격 증명 (**[!UICONTROL 이메일]** 및 암호)
* **[!UICONTROL 지역]**
* **[!UICONTROL 회사]** Dynamic Media - **[!DNL Scene7]** 모드

### Dynamic Media Scene7허용 목록에 추가하다 모드에 대한 공개 송신 IP

Dynamic Media **[!UICONTROL Scene7]**-having [보안 미리 보기 사용](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)Brand Portal에 비디오 자산을 제공하는 데 -이 사용됩니다. **[!UICONTROL Scene7]** 스테이징 환경 또는 내부 응용 프로그램을 위한 전용 이미지 서버를 설정합니다. 이 서버에 대한 모든 요청은 원본 IP 주소를 확인합니다. 수신 요청이 승인된 IP 주소 목록에 없으면 오류 응답이 반환됩니다.
다음 **[!UICONTROL Scene7]** 따라서 회사 관리자는 회사의 승인된 IP 주소 목록을 구성합니다 **[!UICONTROL 보안 테스트]** 환경, **[!UICONTROL SPS]** (Scene7 Publishing System) flash UI. 해당 지역의 송신 IP(다음에서)가 해당 승인된 목록에 추가되어 있는지 확인합니다.
이러한 송신 IP 중 하나를 허용하려면 다음을 참조하십시오 [보안 테스트 서비스를 위한 계정 준비](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
송신 IP는 다음과 같습니다.

| **지역** | **송신 IP** |
|--- |--- |
| NA | 130.248.160.66, 52.151.32.108 |
| EMEA | 185.34.189.1 |
| APAC | 63.140.44.54 |

## Dynamic Media(하이브리드) 설정 구성 {#configure-dm-hybrid-settings}

Experience Manager 작성자 인스턴스가 dynamic media 하이브리드 모드에서 실행 중인 경우 **[!UICONTROL 비디오]** 관리 도구 패널에서 Dynamic Media 게이트웨이 설정을 구성할 수 있습니다.

>[!NOTE]
>
>다음 [비디오 인코딩 프로필](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) 가 Brand Portal에 게시되지 않고 대신 **[!UICONTROL Scene7]** server. 따라서 Brand Portal에서 비디오 인코딩이 성공적으로 재생되도록 하려면 구성 세부 사항이 와 동일한지 확인하십시오 [Dynamic Media Cloud Services ([!DNL Scene7] mode)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=en#configuring-dynamic-media-cloud-services) Experience Manager 작성자 인스턴스에서 사용됩니다.

Brand Portal 테넌트에 대해 Dynamic Media 구성을 설정하려면 다음을 수행하십시오.

1. Brand Portal의 맨 위에 있는 도구 모음에서 관리 도구에 액세스할 수 있도록 Experience Manager 로고를 선택합니다.
1. 관리 도구 패널에서 **[!UICONTROL 비디오]** 타일.

   ![Brand Portal의 Dynamic Media 하이브리드 구성](assets/DMHybrid-Video.png)

   **[!UICONTROL Dynamic Media 구성 편집]** 페이지가 열립니다.

   ![Brand Portal에서 Dynamic Media 하이브리드 구성](assets/edit-dynamic-media-config.png)

1. 지정 **[!UICONTROL 등록 ID]** 및 **[!UICONTROL 비디오 서비스 URL]** (DM-게이트웨이 URL). 이러한 세부 사항이 **[!UICONTROL 도구 > Cloud Services]** Experience Manager 작성자 인스턴스에서 사용됩니다.
1. 선택 **저장** 구성을 저장합니다.

## Dynamic Media Scene7 설정 구성 {#configure-dm-scene7-settings}

Dynamic Media에서 Experience Manager 작성자 인스턴스가 실행 중인 경우 - **[!UICONTROL Scene7]** 모드를 설정한 후 **[!UICONTROL Dynamic Media 구성]** 관리 도구 패널의 타일을 사용하여 구성 **[!UICONTROL Scene7]** 서버 설정.

Dynamic Media을 설정하려면 **[!UICONTROL Scene7]** Brand Portal 테넌트의 구성:

1. Brand Portal의 맨 위에 있는 도구 모음에서 관리 도구에 액세스할 수 있도록 Experience Manager 로고를 선택합니다.

2. 관리 도구 패널에서 **[!UICONTROL Dynamic Media 구성]** 타일.

   ![DM [!UICONTROL Scene 7] Brand Portal에서 구성](assets/DMS7-Tile.png)

   **[!UICONTROL Dynamic Media 구성 편집]** 페이지가 열립니다.

   ![Brand Portal의 Scene 7 구성](assets/S7Config.png)

3. 제공:

   * **[!UICONTROL 제목]**
   * 자격 증명 (**[!UICONTROL 이메일 ID]** 및 **[!UICONTROL 암호]**) Scene7 서버에 액세스하려면
   * **[!UICONTROL 지역]**

   이러한 값이 Experience Manager 작성자 인스턴스에 있는 값과 동일한지 확인합니다.

4. 선택 **[!UICONTROL Dynamic Media에 연결]**.

5. 다음을 제공합니다. **[!UICONTROL 회사 이름]**, 및 **[!UICONTROL 저장]** 구성.
