---
title: Brand Portal에서 동적 비디오 지원
seo-title: Brand Portal에서 동적 비디오 지원
description: Brand Portal에서 동적 비디오 지원
seo-description: Brand Portal에서 동적 비디오 지원
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
translation-type: tm+mt
source-git-commit: eab0a56cfe03d13485386ddc60400ed458198950
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 3%

---


# Brand Portal에서 동적 비디오 지원 {#dynamic-video-support-on-brand-portal}

Dynamic Media 지원을 통해 브랜드 포털에서 비디오를 미리 보고 재생할 수 있습니다. 또한 포털과 공유 링크에서 동적 변환을 다운로드합니다.
브랜드 포털 사용자는 다음을 수행할 수 있습니다.

* 자산 세부 사항 페이지, 카드 보기 및 링크 공유 미리 보기 페이지에서 비디오를 미리 볼 수 있습니다.
* 자산 세부 사항 페이지에서 비디오 인코딩을 재생합니다.
* 자산 세부 사항 페이지의 표현물 탭에서 동적 표현물을 봅니다.
* 비디오가 포함된 비디오 코드 및 폴더를 다운로드합니다.

>[!NOTE]
>
>비디오를 사용하여 작업하고 브랜드 포털에 게시하려면 Dynamic Media 하이브리드 모드 또는 Dynamic Media **[!DNL Scene 7]** 모드에서 AEM Author 인스턴스가 설정되어 있어야 합니다.

비디오를 미리 보고 재생하고 다운로드하려면 브랜드 포털에서 관리자에게 다음 두 가지 구성을 표시합니다.

* [Dynamic Media 하이브리드 구성](#configure-dm-hybrid-settings)AEM Author 인스턴스가 다이내믹 미디어 하이브리드 모드에서 실행 중인 경우
* [동적 [!DNL Scene 7] 미디어 구성](#configure-dm-scene7-settings)AEM Author 인스턴스가 다이내믹 미디어 모드에서 실행 중인&#x200B;**[!DNL Scene 7]** 경우
이 구성 중 하나를 AEM Author 인스턴스에서 브랜드 포털 테넌트가 복제되는 구성에 따라 설정합니다.

>[!NOTE]
>
>동적 비디오는 **[!UICONTROL Scene7Connect 런타임 모드에서 실행되는 AEM Author으로 구성된 브랜드 포털 테넌트에서]** 지원되지 않습니다.

## 동적 비디오는 어떻게 재생됩니까? {#how-are-dynamic-videos-played}

![클라우드에서 비디오 인코딩](assets/VideoEncodes.png)

Dynamic Media 구성([하이브리드](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings)[또는](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) [!DNL Scene 7] **[!DNL Scene 7]** 구성)이 브랜드 포털에 설정되어 있는 경우, 동적 변환은서버에서 가져옵니다. 비디오 인코딩은 지연 없이 미리 보고 재생되며 품질은 왜곡되지 않습니다.

비디오 인코딩은 브랜드 포털 리포지토리에 저장되지 않으며 **[!DNL Scene 7]** 서버에서 반입되므로 AEM Author 인스턴스 및 브랜드 포털의 Dynamic Media 구성이 동일한지 확인합니다.

>[!NOTE]
>
>비디오 뷰어 및 뷰어 사전 설정은 브랜드 포털에서 지원되지 않습니다. 비디오가 미리 보고 브랜드 포털의 기본 뷰어에서 재생됩니다.

## 전제 조건 {#prerequisites}

브랜드 포털에서 다이내믹 비디오를 사용하려면 다음을 확인하십시오.

* **DM(Dynamic Media) 모드에서 AEM Author 시작** Dynamic Media [하이브리드 모드](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) 또는 [동적 [!DNL Scene 7] 미디어 모드에서 AEM Author 인스턴스(브랜드 포털이 구성된)를 시작합니다](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **AEM Author에서 Dynamic Media 클라우드 서비스 구성** Dynamic Media 모드 AEM Author이 실행 중인에 따라 [도구](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) 에서 AEM Author에 있는 [[!DNL Scene 7] Dynamic Media 클라우드 서비스](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) 또는 **클라우드 서비스중 하나를설정합니다** | **Cloud Service** | **Dynamic Media**.
* **AEM Author의 Dynamic Media 클라우드 구성을**&#x200B;기반으로 브랜드 포털의 Dynamic Media을 구성하고, 브랜드 포털 관리 도구에서 [Dynamic Media 설정](#configure-dm-hybrid-settings) 또는 [[!DNL Scene 7] 설정을](#configure-dm-scene7-settings) 구성합니다.
Dynamic Media Hybrid 및 Dynamic Media [S7](#separate-tenants)**[!UICONTROL 의 기능을 사용하는 경우 Dynamic Media Hybrid 및 Scene7]** 모드로 구성된 AEM Author 인스턴스에 **[!UICONTROL 별도의 브랜드 포털 테넌트가 사용되는지]**&#x200B;확인하십시오.
* **브랜드 포털에 비디오 인코딩이 적용된 폴더 게시**[비디오 인코딩](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) 을 적용하고 AEM Author 인스턴스의 리치 미디어 에셋이 포함된 폴더를 브랜드 포털에 게시합니다.
* **보안 미리 보기가 활성화된**&#x200B;경우 SPS의 허용 목록 주소 IP **[!DNL Scene 7]** 를 Dynamic Media- [(회사에서](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) 보안 미리 보기가 **[!DNL Scene 7]** 활성화된 [경우)를 사용하는](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) 경우 회사는 관리자가 SPS(SceneScene7 Flash Publishing System)을 사용하여 해당 영역에 대해&#x200B;**[!UICONTROL IP 목록 공개]** 를 SPS(Scene7 Flash Publishing System)를 사용하여 각각의 영역에 대해외부로 보내는 것을 허용하는 것이 좋습니다.
송신 IP는 다음과 같습니다.

| **지역** | **송신 IP** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

이러한 송신 IP 중 하나를 허용하려면 보안 테스트 서비스를 [위한 계정 준비를 참조하십시오](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## 우수 사례

브랜드 포털(및 공유 링크)에서 다이내믹 비디오 자산을 성공적으로 미리 보고, 재생하고 다운로드하려면 다음 방법을 따르십시오.

### Dynamic Media 하이브리드 및 Dynamic Media 장면 7 모드를 위한 세입자 분리 {#separate-tenants}

Dynamic Media **[!DNL Scene 7]** 및 Dynamic Media 하이브리드 기능을 모두 사용하는 경우 Dynamic Media 하이브리드 및 Dynamic Media 모드로 구성된 AEM Author 인스턴스에 대해 다른 브랜드 포털 테넌트를 사용하는 것이 **[!DNL Scene 7]** 좋습니다.<br />

![작성 및 BP를 1대1 매핑](assets/BPDynamicMedia.png)

### AEM Author 인스턴스 및 브랜드 포털에서 동일한 구성 세부 사항

[ **[!UICONTROL 제목]**], [등록 ID **, []** Dynamic Media 및Video **[!UICONTROL URL]과 같은 구성 세부 사항(]** 에서)과 [비디오] URL **, [비디오 자격 증명], [전자 메일 및 암호], [전자 메일] 및 []********** ******** **[!DNL Scene 7]******&#x200B;전자 메일], [전자 메일] 및 [전자 메일], [지역], [Dynamic Media이]과 같은이 같은 구성 세부 사항이 [브랜드에 있습니다. AEM 클라우드 구성.

### Dynamic Media Scene 7 모드에 대한 허용 목록 공개 주소 IP

Dynamic Media **[!UICONTROL Scene 7]**&#x200B;의 [보안 미리 보기 활성화](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)-를 사용하여 브랜드 포털에 비디오 자산을 제공하는 경우 **[!UICONTROL Scene 7은]** 스테이징 환경 또는 내부 애플리케이션에 대한 전용 이미지 서버를 설정합니다. 이 서버에 대한 모든 요청은 원본 IP 주소를 확인합니다. 수신 요청이 승인된 IP 주소 목록 내에 없으면 실패 응답이 반환됩니다.
따라서 **[!UICONTROL Scene-7]** Company 관리자는 **[!UICONTROL SPS]** (Scene-7 Publishing System) Flash UI를 통해 회사의 **[!UICONTROL 보안 테스트]** 환경에 대해 승인된 IP 주소 목록을구성합니다. 해당 지역의 송신 IP가 승인된 목록에 추가되어 있는지 확인합니다(다음 항목부터).
이러한 송신 IP 중 하나를 허용하려면 보안 테스트 서비스를 [위한 계정 준비를 참조하십시오](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
송신 IP는 다음과 같습니다.

| **지역** | **송신 IP** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Dynamic Media(하이브리드) 설정 구성 {#configure-dm-hybrid-settings}

AEM Author 인스턴스가 다이내믹 미디어 하이브리드 모드에서 실행 중인 경우 관리 도구 패널의 **[!UICONTROL 비디오]** 타일을 사용하여 Dynamic Media 게이트웨이 설정을 구성합니다.
>[!NOTE]
>
>[비디오 인코딩 프로필은](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) 브랜드 포털에 게시되지 않고 대신 **[!UICONTROL Scene 7]** 서버에서 반입됩니다. 따라서 비디오 인코딩이 브랜드 포털에서 성공적으로 재생되도록 하려면 구성 세부 사항이 AEM Author 인스턴스의 [[!UICONTROL Scene7 클라우드 구성과]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) 동일한지 확인합니다.
브랜드 포털 테넌트에 Dynamic Media 구성을 설정하려면

1. 브랜드 포털의 상단 도구 모음에서 관리 도구에 액세스하려면 AEM 로고를 선택합니다.

2. 관리 도구 패널에서 **[!UICONTROL 비디오]** 타일을 선택합니다.<br />

   ![브랜드 포털의 Dynamic Media 하이브리드 구성](assets/DMHybrid-Video.png)
   **[!UICONTROL Dynamic Media 편집 구성]** 페이지가 열립니다.<br />
   ![브랜드 포털의 Dynamic Media 하이브리드 구성](assets/edit-dynamic-media-config.png)

3. 등록 **[!UICONTROL ID]** 및 **[!UICONTROL 비디오 서비스 URL]** (DM-게이트웨이 URL)을 지정합니다. 이러한 세부 사항이 AEM Author 인스턴스의 **[!UICONTROL [도구] > [Cloud Service]** ]와 동일한지 확인합니다.

4. 저장을 **선택하여** 구성을 저장합니다.

## Dynamic Media Scene7 설정 구성 {#configure-dm-scene7-settings}

AEM Author 인스턴스가 Dynamic Media- **[!UICONTROL Scene 7]** 모드에서 실행 중인 경우 관리 도구 패널의 **[!UICONTROL Dynamic Media 구성]** 타일을 사용하여 **[!UICONTROL Scene 7]** 서버 설정을 구성합니다.

브랜드 포털 테넌트에 **[!UICONTROL Dynamic Media Scene 7]** 구성을 설정하려면

1. 브랜드 포털의 상단 도구 모음에서 관리 도구에 액세스하려면 AEM 로고를 선택합니다.

2. 관리 도구 패널에서 **[!UICONTROL Dynamic Media 구성]** 타일을 선택합니다.<br />
   ![브랜드 [!UICONTROL 포털의 DM Scene 7] 구성](assets/DMS7-Tile.png)
   **[!UICONTROL Dynamic Media 편집 구성]** 페이지가 열립니다.<br />
   ![브랜드 포털의 Scene 7 구성](assets/S7Config.png)

3. 제공:
   * **[!UICONTROL 제목]**
   * Scene 7 서버에 액세스하기 위한 자격 증명(**[!UICONTROL 이메일 ID]** 및 **[!UICONTROL 암호]**)
   * **[!UICONTROL 영역]**&#x200B;이 값이 AEM Author 인스턴스의 값과 동일한지 확인합니다.

4. Select **[!UICONTROL Connect to Dynamic Media]**.

5. 회사 **[!UICONTROL 이름을]**&#x200B;입력하고 **[!UICONTROL 구성을]** 저장합니다.
