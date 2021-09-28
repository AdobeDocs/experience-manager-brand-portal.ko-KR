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
source-git-commit: d7dbf9ae2d27dda2edb60d8f861e618fb6332ec7
workflow-type: tm+mt
source-wordcount: '1185'
ht-degree: 2%

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
>비디오를 사용하여 작업하고 Brand Portal에 게시하려면 AEM 작성자 인스턴스가 Dynamic Media 하이브리드 모드 또는 Dynamic Media **[!DNL Scene 7]** 모드에 설정되어 있는지 확인하십시오.

비디오를 미리 보고 재생하고 다운로드하려면 Brand Portal이 관리자에게 다음 두 가지 구성을 표시합니다.

* [Dynamic Media 하이브리드 ](#configure-dm-hybrid-settings)
구성AEM 작성자 인스턴스가 dynamic media 하이브리드 모드에서 실행 중인 경우.
* [Dynamic  [!DNL Scene 7] ](#configure-dm-scene7-settings)
Media 구성AEM 작성자 인스턴스가 다이내믹 미디어 모드에서 실행 중인 **[!DNL Scene 7]** 경우.
Brand Portal 테넌트가 복제되는 AEM 작성자 인스턴스에서 설정한 구성을 기반으로 이러한 구성 중 하나를 설정합니다.

>[!NOTE]
>
>**[!UICONTROL Scene7Connect]** 실행 모드에서 실행되는 AEM Author로 구성된 Brand Portal 테넌트에서 동적 비디오가 지원되지 않습니다.

## 다이내믹 비디오는 어떻게 재생됩니까? {#how-are-dynamic-videos-played}

![비디오 인코딩을 클라우드에서 가져옵니다](assets/VideoEncodes.png)

Dynamic Media 구성([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) 또는 [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) 구성)이 Brand Portal에 설정된 경우, 동적 변환은 **[!DNL Scene 7]** 서버에서 가져옵니다. 따라서 비디오 인코딩은 지연과 왜곡없이 미리 보고 재생됩니다.

비디오 인코딩은 Brand Portal 저장소에 저장되지 않고 **[!DNL Scene 7]** 서버에서 가져오므로 AEM 작성자 인스턴스 및 Brand Portal의 Dynamic Media 구성이 동일한지 확인하십시오.

>[!NOTE]
>
>Brand Portal에서는 비디오 뷰어 및 뷰어 사전 설정이 지원되지 않습니다. Brand Portal의 기본 뷰어에서 비디오를 미리 보고 재생합니다.

## 전제 조건 {#prerequisites}

Brand Portal에서 다이내믹 비디오를 사용하여 작업하려면 다음을 수행하십시오.

* **DM(Dynamic Media)**
모드에서 AEM 작성자 시작  [Dynamic Media Hybrid 모드 또는 ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) Dynamic  [Mediamode [!DNL Scene 7] 에서 AEM 작성자 인스턴스(Brand Portal이 구성된 ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode)인스턴스)를 시작합니다.
* **AEM 작성자에서 Dynamic Media 클라우드 서비스**
구성 AEM 작성자가 실행 중인 Dynamic Media 모드를 기반으로  [Dynamic Media 클라우드 ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) 서비스 또는  [[!DNL Scene 7] 도구](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) 의 AEM 작성자에 대한  **클라우드 서비스** |  **Cloud Services** |  **Dynamic Media**.
* **Brand Portal에서 Dynamic Media**
구성AEM 작성자의 Dynamic Media 클라우드 구성을 기반으로  [Dynamic Media ](#configure-dm-hybrid-settings) 설정 또는 Brand Portal 관리  [[!DNL Scene 7] ](#configure-dm-scene7-settings)  도구에서 설정을 구성합니다.
Dynamic Media Hybrid 및 Dynamic Media **[!UICONTROL S7]**&#x200B;의 기능을 사용하는 경우, Dynamic Media Hybrid 및 Dynamic Media **[!UICONTROL Scene7]** 모드로 구성된 AEM Author 인스턴스에 별도의 Brand Portal 테넌트](#separate-tenants)가 사용되는지 확인하십시오.[
* **Brand Portal에 비디오 인코딩이 적용된 폴더**
를 게시 [비디오 인코딩](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) 을 적용하고 AEM 작성자 인스턴스의 리치 미디어 자산이 포함된 폴더를 Brand Portal에 게시합니다.
* **보안 미리 보기가**
활성화된 경우 SPS에서 IP 가져오기**[!DNL Scene 7]** ( [회사](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) 에 대해  **[!DNL Scene 7]** 보안 미리 보기 사용)를 사용하는 경우  [회사 관리자가 SPS(](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) Scene 7 **[!UICONTROL Publishing System) 플래시 UI를 사용하여 각 지역]** 의 공용 송신IP를 관리하는 것이좋습니다.
송신 IP는 다음과 같습니다.

| **지역** | **송신 IP** |
|--- |--- |
| NA | 130.248.160.66, 52.151.32.108 |
| EMEA | 185.34.189.1 |
| APAC | 63.140.44.54 |

이러한 송신 IP 중 하나를 허용리스트 지정하려면 [보안 테스트 서비스를 위한 계정 준비](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)를 참조하십시오.

## 우수 사례

Brand Portal(및 공유 링크)에서 다이내믹 비디오 자산을 성공적으로 미리 보고, 재생하고 다운로드하도록 하려면 다음 방법을 따르십시오.

### Dynamic Media Hybrid 및 Dynamic Media Scene 7 모드에 대한 별도의 테넌트 {#separate-tenants}

Dynamic Media **[!DNL Scene 7]** 및 Dynamic Media Hybrid 기능을 모두 사용하는 경우 Dynamic Media Hybrid 및 Dynamic Media **[!DNL Scene 7]** 모드로 구성된 AEM Author 인스턴스용 서로 다른 Brand Portal 테넌트를 사용하는 것이 좋습니다.


![작성자 및 BP 1에서 1로의 매핑](assets/BPDynamicMedia.png)

### AEM 작성자 인스턴스 및 Brand Portal에서 동일한 구성 세부 정보

**[!UICONTROL 제목]**, **[!UICONTROL 등록 ID]**, **[!UICONTROL 비디오 서비스 URL]**(**[!UICONTROL Dynamic Media Hybrid]**&#x200B;에서) 및 **[!UICONTROL 제목]**, 자격 증명(**[!UICONTROL 이메일]** 및 암호), **[!UICONTROL 지역]**, **[!UICONTROL Dynamic Media의]** **[!DNL Scene 7]**)-은 Brand Portal 및 **[!UICONTROL AEM 클라우드 구성]**&#x200B;에서 동일합니다.

### Dynamic Media 허용 목록에 추가하다 Scene 7 모드에 대한 공개 송신 IP

Dynamic Media **[!UICONTROL 보안 미리 보기 활성화]**-with [비디오 자산을 Brand Portal에 제공하는 데 사용되는 경우, **[!UICONTROL Scene 7]**&#x200B;은 스테이징 환경 또는 내부 애플리케이션을 위한 전용 이미지 서버를 설정합니다. ](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) 이 서버에 대한 모든 요청은 원본 IP 주소를 확인합니다. 수신 요청이 승인된 IP 주소 목록에 없으면 오류 응답이 반환됩니다.
따라서 **[!UICONTROL Scene-7]** 회사 관리자는 **[!UICONTROL SPS]**(Scene-7 Publishing System) 플래시 UI를 통해 회사의 **[!UICONTROL 보안 테스트]** 환경에 대해 승인된 IP 주소 목록을 구성합니다. 해당 지역의 송신 IP(다음에서)가 해당 승인된 목록에 추가되어 있는지 확인합니다.
이러한 송신 IP 중 하나를 허용리스트 지정하려면 [보안 테스트 서비스를 위한 계정 준비](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)를 참조하십시오.
송신 IP는 다음과 같습니다.

| **지역** | **송신 IP** |
|--- |--- |
| NA | 130.248.160.66, 52.151.32.108 |
| EMEA | 185.34.189.1 |
| APAC | 63.140.44.54 |

## Dynamic Media(하이브리드) 설정 구성 {#configure-dm-hybrid-settings}

AEM 작성자 인스턴스가 Dynamic Media 하이브리드 모드에서 실행 중인 경우 관리 도구 패널의 **[!UICONTROL 비디오]** 타일을 사용하여 Dynamic Media 게이트웨이 설정을 구성합니다.

>[!NOTE]
>
>[비디오 인코딩 프로필](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html)은 Brand Portal에 게시되지 않고, 대신 **[!UICONTROL Scene 7]** 서버에서 가져옵니다. 따라서 비디오 인코딩이 Brand Portal에서 성공적으로 재생되도록 하려면 구성 세부 사항이 AEM 작성자 인스턴스의 [[!UICONTROL Scene7 클라우드 구성]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices)와 동일한지 확인하십시오.

Brand Portal 테넌트에 대해 Dynamic Media 구성을 설정하려면 다음을 수행하십시오.

1. Brand Portal의 맨 위에 있는 도구 모음에서 관리 도구에 액세스하려면 AEM 로고를 선택합니다.
1. 관리 도구 패널에서 **[!UICONTROL 비디오]** 타일을 선택합니다.

   ![Brand Portal의 Dynamic Media 하이브리드 구성](assets/DMHybrid-Video.png)

   **[!UICONTROL Dynamic Media 구성]** 편집 페이지가 열립니다.

   ![Brand Portal에서 Dynamic Media 하이브리드 구성](assets/edit-dynamic-media-config.png)

1. **[!UICONTROL 등록 ID]** 및 **[!UICONTROL 비디오 서비스 URL]**(DM-게이트웨이 URL)을 지정합니다. 이러한 세부 사항이 AEM 작성자 인스턴스의 **[!UICONTROL 도구 > Cloud Services]**&#x200B;에 있는 세부 정보와 동일한지 확인합니다.
1. **저장**&#x200B;을 선택하여 구성을 저장합니다.

## Dynamic Media Scene7 설정 구성 {#configure-dm-scene7-settings}

AEM 작성자 인스턴스가 Dynamic Media- **[!UICONTROL Scene 7]** 모드에서 실행 중인 경우 관리 도구 패널에서 **[!UICONTROL Dynamic Media 구성]** 타일을 사용하여 **[!UICONTROL Scene 7]** 서버 설정을 구성합니다.

Brand Portal 테넌트에서 Dynamic Media **[!UICONTROL Scene 7]** 구성을 설정하려면 다음을 수행하십시오.

1. Brand Portal의 맨 위에 있는 도구 모음에서 관리 도구에 액세스하려면 AEM 로고를 선택합니다.

2. 관리 도구 패널에서 **[!UICONTROL Dynamic Media 구성]** 타일을 선택합니다.

   ![Brand Portal의 DM  [!UICONTROL Scene 7]  구성](assets/DMS7-Tile.png)

   **[!UICONTROL Dynamic Media 구성]** 편집 페이지가 열립니다.

   ![Brand Portal의 Scene 7 구성](assets/S7Config.png)

3. 제공:

   * **[!UICONTROL 제목]**
   * Scene 7 서버에 액세스할 수 있는 자격 증명(**[!UICONTROL 이메일 ID]** 및 **[!UICONTROL 암호]**)
   * **[!UICONTROL 지역]**

   이러한 값이 AEM 작성자 인스턴스의 값과 동일한지 확인합니다.

4. **[!UICONTROL Dynamic Media에 연결]**&#x200B;을 선택합니다.

5. **[!UICONTROL 회사 이름]** 및 **[!UICONTROL Save]**&#x200B;구성을 제공합니다.
