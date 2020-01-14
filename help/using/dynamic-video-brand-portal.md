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
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# Brand Portal에서 동적 비디오 지원 {#dynamic-video-support-on-brand-portal}

다이내믹 미디어 지원을 통해 브랜드 포털에서 비디오를 미리 보고 재생할 수 있습니다. 포털과 공유 링크에서 동적 표현물을 다운로드할 수도 있습니다.
브랜드 포털 사용자는 다음을 수행할 수 있습니다.

* 자산 세부 사항 페이지, 카드 보기 및 링크 공유 미리 보기 페이지에서 비디오를 미리 볼 수 있습니다.
* 자산 세부 사항 페이지에서 비디오 인코딩을 재생합니다.
* 자산 세부 사항 페이지의 표현물 탭에서 동적 표현물을 봅니다.
* 비디오가 포함된 비디오 인코딩 및 폴더를 다운로드합니다.

>[!NOTE]
>
>비디오를 사용하여 작업하고 브랜드 포털에 게시하려면 AEM 작성자 인스턴스가 다이내믹 미디어 하이브리드 모드 또는 다이내믹 미디어 **[!DNL Scene 7]**모드에서 설정되어 있는지 확인하십시오.

비디오를 미리 보고 재생하고 다운로드하려면 브랜드 포털에서 관리자에게 다음 두 가지 구성을 표시합니다.

* [다이내믹 미디어 하이브리드 구성](#configure-dm-hybrid-settings)AEM 작성자 인스턴스가 다이내믹 미디어 하이브리드 모드에서 실행 중인 경우
* [다이내믹 미디어 [!DNL Scene 7] 구성](#configure-dm-scene7-settings)AEM 작성자 인스턴스가 다이내믹 미디어&#x200B;**[!DNL Scene 7]**모드에서 실행 중인 경우.
브랜드 포털 테넌트가 복제되는 AEM 작성자 인스턴스에서 설정한 구성을 기준으로 이러한 구성 중 하나를 설정합니다.

>[!NOTE]
>
>Scene7Connect 런타임 모드에서 실행 중인 AEM 작성자와 통합된 브랜드 포털 **[!UICONTROL 테넌트에서는 동적 비디오가]**지원되지 않습니다.

## 동적 비디오 재생 방법 {#how-are-dynamic-videos-played}

![클라우드에서 비디오 인코딩](assets/VideoEncodes.png)

Brand Portal에서 다이내믹 미디어 구성([하이브리드](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) 또는 [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) 구성)을 **[!DNL Scene 7]**설정하는 경우서버에서 동적 변환을 가져옵니다. 따라서 비디오 인코딩은 지연 없이 미리 보고 재생되며 품질은 왜곡됩니다.

비디오 인코딩은 브랜드 포털 저장소에 저장되지 않고 **[!DNL Scene 7]**서버에서 반입되므로 AEM 작성자 인스턴스 및 브랜드 포털의 다이내믹 미디어 구성이 동일한지 확인하십시오.

>[!NOTE]
>
>비디오 뷰어 및 뷰어 사전 설정은 브랜드 포털에서 지원되지 않습니다. 비디오는 브랜드 포털에서 기본 뷰어에서 미리 보고 재생됩니다.

## 전제 조건 {#prerequisites}

브랜드 포털에서 다이내믹한 비디오를 사용하여 작업하려면 다음을 확인하십시오.

* **DM(다이내믹 미디어) 모드에서** AEM 작성자 시작AEM 작성자 인스턴스(브랜드 포털이 통합된 AEM 작성자 인스턴스)를 다이내믹 미디어 [하이브리드 모드](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) 또는 [다이내믹 미디어 [!DNL Scene 7] 모드에서](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode)시작합니다.
* **AEM 작성자에서 Dynamic Media 클라우드 서비스**&#x200B;구성 AEM 작성자가 실행 중인 다이내믹 미디어 모드를 기반으로 Dynamic [Media 클라우드 서비스](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) 또는 [도구에서 AEM 작성자의 클라우드 서비스](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) [!DNL Scene 7] 클라우드 서비스를 **설정합니다** | **클라우드 서비스** | **Dynamic Media**.
* **브랜드 포털에서 다이내믹 미디어 구성** AEM 작성자의 다이내믹 미디어 클라우드 구성을 기반으로, 다이내믹 미디어 설정 [또는](#configure-dm-hybrid-settings) [!DNL Scene 7] 설정을 [](#configure-dm-scene7-settings) 브랜드 포털 관리 도구에서 구성합니다.
Dynamic Media Hybrid 및 Dynamic Media S7의 기능을 사용하는 경우, 다이내믹 미디어 하이브리드 및 다이내믹 미디어 [Scene7](#separate-tenants) 모드로 구성된 AEM 작성자 인스턴스에 **[!UICONTROL 별도의 브랜드 포털 테넌트가]**사용되는지**[!UICONTROL &#x200B;확인하십시오]**.
* **브랜드 포털에 비디오 인코딩이 적용된 폴더 게시**[비디오 인코딩을](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) 적용하고 AEM 작성자 인스턴스의 리치 미디어 에셋이 포함된 폴더를 브랜드 포털에 게시합니다.
* **보안 미리 보기를 활성화한**&#x200B;경우 SPS에서 화이트리스트 IP 가져오기&#x200B;**[!DNL Scene 7]**IP[를 사용하는](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)경우(회사에서**[!DNL Scene 7]** 보안 미리 보기가 활성화됨 [) 다이내믹 미디어를 사용하는](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) 경우, 해당&#x200B;**[!UICONTROL SPS(Scene7 Publishing System)를 사용하여 해당]**영역에 대해 화이트리스트 공개 IP를관리하는 것이 좋습니다.
송신 IP는 다음과 같습니다.

| **지역** | **송신 IP** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

이러한 송신 IP를 화이트리스트에 추가하려면 보안 테스트 서비스를 [위한 계정](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)준비를 참조하십시오.

## 우수 사례

다이내믹 비디오 에셋이 브랜드 포털(및 공유 링크)에서 성공적으로 미리 보고 재생되고 다운로드되었는지 확인하려면 다음 방법을 따르십시오.

### Dynamic Media Hybrid 및 Dynamic Media Scene 7 모드를 위한 개별 테넌트 {#separate-tenants}

다이내믹 미디어 **[!DNL Scene 7]**및 다이내믹 미디어 하이브리드 기능을 모두 사용하는 경우 다이내믹 미디어 하이브리드 및 다이내믹 미디어 모드로 구성된 AEM 작성자 인스턴스에 대해 다른 브랜드 포털 테넌트를 사용하는 것이**[!DNL Scene 7]** 좋습니다.<br />

![작성 및 BP 1-1 매핑](assets/BPDynamicMedia.png)

### AEM 작성자 인스턴스 및 브랜드 포털에서 동일한 구성 세부 사항

Registration ID, **[!UICONTROL Registration ID]**,****Registration Service URL **[!UICONTROL URL(]**비디오의 VideoMedia And VideoMedia의 Dynamic**[!UICONTROL  Credentials, EmailAnd Password]**Password와 Hybrid CompanyHybridMedia의 구성 세부 사항이 같은 ******** ******** **[!DNL Scene 7]******구성 세부 사항인지 확인합니다. 포털 및 AEM 클라우드 구성

### Dynamic Media Scene 7 모드에 대한 화이트리스트 공개 주소 IP

Dynamic Media **[!UICONTROL Scene 7]**의[보안 미리 보기가 활성화됨](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)-으로 비디오 자산을 Brand Portal에 제공하는**[!UICONTROL &#x200B;경우 Scene 7은]** 스테이징 환경 또는 내부 응용 프로그램을 위한 전용 이미지 서버를 만듭니다. 이 서버에 대한 모든 요청은 원본 IP 주소를 확인합니다. 수신 요청이 승인된 IP 주소 목록 내에 없으면 실패 응답이 반환됩니다.
따라서 **[!UICONTROL Scene-7]**Company 관리자는 SPS(Scene-7 Publishing System)**[!UICONTROL &#x200B;플래시]** UI를 통해 회사의 보안 테스트 환경에 대해 ****승인된 IP 주소 목록을 구성합니다. 각 지역의 송신 IP가 승인된 목록에 추가되어 있는지 확인하십시오.
이러한 송신 IP를 화이트리스트에 추가하려면 보안 테스트 서비스를[위한 계정](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)준비를 참조하십시오.
송신 IP는 다음과 같습니다.

| **지역** | **송신 IP** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## 다이내믹 미디어(하이브리드) 설정 구성 {#configure-dm-hybrid-settings}

AEM 작성자 인스턴스가 다이내믹 미디어 하이브리드 모드에서 실행 중인 경우 관리 **[!UICONTROL 도구]**패널의 비디오 타일을 사용하여 Dynamic Media 게이트웨이 설정을 구성합니다.
>[!NOTE]
>
>비디오 [인코딩 프로필은](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) 브랜드 포털에 게시되지 않고 대신 Scene 7 **[!UICONTROL 서버에서 가져옵니다]**. 따라서 비디오 인코딩이 브랜드 포털에서 성공적으로 재생되도록 하려면 구성 세부 사항이 AEM 작성자[[!UICONTROL 인스턴스의 Scene7 클라우드 구성과]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices)동일한지 확인합니다.
브랜드 포털 임차인에서 다이내믹 미디어 구성을 설정하려면

1. 브랜드 포털의 상단 도구 모음에서 관리 도구에 액세스하려면 AEM 로고를 선택합니다.

2. 관리 도구 패널에서 비디오 **[!UICONTROL 타일을 선택합니다]**.<br />   ![브랜드 포털의 다이내믹 미디어 하이브리드 구성](assets/DMHybrid-Video.png)
   **[!UICONTROL Dynamic Media 구성 편집]**페이지가 열립니다.<br />   ![브랜드 포털의 다이내믹 미디어 하이브리드 구성](assets/edit-dynamic-media-config.png)

3. 등록 **[!UICONTROL ID]**및**[!UICONTROL &#x200B;비디오 서비스 URL]** (DM-게이트웨이 URL)을 지정합니다. 이러한 세부 사항이 AEM 작성자 인스턴스의 도구 > **[!UICONTROL 클라우드]**서비스의 세부 사항과 동일한지 확인합니다.

4. 저장을 **선택하여** 구성을 저장합니다.

## Dynamic Media Scene7 설정 구성 {#configure-dm-scene7-settings}

AEM 작성자 인스턴스가 Dynamic Media - **[!UICONTROL Scene 7]**모드에서 실행 중인**[!UICONTROL &#x200B;경우]** 관리 도구 **[!UICONTROL 패널의]**Dynamic Media 구성 타일을 사용하여Scene7서버 설정을 구성할수 있습니다.

브랜드 포털 임차인에서 **[!UICONTROL 다이내믹 미디어]**Scene 7 구성을 설정하려면

1. 브랜드 포털의 상단 도구 모음에서 관리 도구에 액세스하려면 AEM 로고를 선택합니다.

2. 관리 도구 패널에서 Dynamic Media **[!UICONTROL 구성 타일을]**선택합니다.<br />   ![브랜드 [!UICONTROL 포털의 DM] Scene 7 구성](assets/DMS7-Tile.png)
   **[!UICONTROL Dynamic Media 구성 편집]**페이지가 열립니다.<br />   ![브랜드 포털의 Scene 7 구성](assets/S7Config.png)

3. 제공:
   * **[!UICONTROL 제목]**
   * Scene 7 **[!UICONTROL 서버에]**액세스하기 위한 자격 증명(이메일 ID**[!UICONTROL &#x200B;및]**암호)
   * **[!UICONTROL 영역]**이러한 값이 AEM 작성자 인스턴스의 값과 동일한지 확인합니다.

4. Select **[!UICONTROL Connect to Dynamic Media]**.

5. 회사 이름을 **[!UICONTROL 입력하고]**구성을**[!UICONTROL &#x200B;저장합니다]** .
