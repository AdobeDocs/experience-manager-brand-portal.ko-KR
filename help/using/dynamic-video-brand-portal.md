---
title: 브랜드 포털에서 다이내믹한 비디오 지원
seo-title: 브랜드 포털에서 다이내믹한 비디오 지원
description: 브랜드 포털에서 다이내믹한 비디오 지원
seo-description: 브랜드 포털에서 다이내믹한 비디오 지원
uuid: A 3502 A 4 D -3971-4 EA 4-953 C -44 BA 04446269
contentOwner: Mgulati
products: sg_ Experiencemanager/brand_ portal
content-type: 참조
topic-tags: download-install
discoiquuid: E 18 D 992 A-A 3 B 5-45 F 2-9696-8161993213 EE
translation-type: tm+mt
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# 브랜드 포털에서 다이내믹한 비디오 지원 {#dynamic-video-support-on-brand-portal}

다이내믹 미디어 지원을 통해 적응형 동영상을 [!DNL Brand Portal] 미리 보고 재생할 수 있습니다. 또한 포털 및 공유 링크에서 동적 표현물을 다운로드하십시오.
[!DNL Brand Portal] 사용자는 다음을 수행할 수 있습니다.

* 자산 세부 사항 페이지, 카드 보기 및 링크 공유 미리 보기 페이지에서 비디오 미리 보기
* 자산 세부 사항 페이지에서 비디오 인코딩 재생을 참조하십시오.
* 자산 세부 사항 페이지의 표현물 탭에서 다이내믹 표현물을 봅니다.
* 비디오가 포함된 비디오 인코딩 및 폴더를 다운로드합니다.

>[!NOTE]
>
>비디오를 사용하여 작업하고 게시하려면 [!DNL Brand Portal][!DNL AEM] 작성자 인스턴스가 다이내믹 미디어 하이브리드 모드 또는 다이내믹 미디어 [!DNL Scene 7] 모드에서 설정되어 있는지 확인하십시오.

비디오를 미리 보거나 재생하고 다운로드하려면 다음 두 가지 구성을 관리자에게 [!DNL Brand Portal] 노출하십시오.

* [다이내믹 미디어 하이브리드 모드에서](#configure-dm-hybrid-settings)[!DNL AEM] 작성자 인스턴스가 실행 중인 경우의 다이내믹 미디어 하이브리드 구성입니다.
* [다이내믹 미디어 [! DNL Scene 7] 작성자 인스턴스가 다이내믹 미디어 모드에서 실행되는](#configure-dm-scene7-settings)경우의 [!DNL AEM] 구성을[!DNL Scene 7] 
참조하십시오.
테넌트가 복제되는 [!DNL AEM] 작성자 인스턴스에서 설정한 구성에 따라 이러한 구성 중 [!DNL Brand Portal] 하나를 설정합니다.

>[!NOTE]
>
>Scene 7 Connect runmode에서 실행되는 [!DNL Brand Portal] 작성자와 [!DNL AEM] 통합된 테넌트에서 동적 비디오는 [!UICONTROL 지원되지] 않습니다.

## 동적 비디오는 어떻게 재생됩니까? {#how-are-dynamic-videos-played}

![클라우드에서 비디오 인코딩 가져오기](assets/VideoEncodes.png)

Dynamic Media 구성 ([하이브리드](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) 또는 [[! DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) 구성을 설정하고 [!DNL Brand Portal][!DNL Scene 7] 서버에서 동적 표현물을 가져옵니다. 따라서 비디오 인코딩은 품질 왜곡과 왜곡 없이 미리 보고 재생할 수 있습니다.

비디오 인코딩이 [!DNL Brand Portal] 보관소에 저장되지 않고 [!DNL Scene 7] 서버에서 가져오는 경우 [!DNL AEM] , 작성자 인스턴스의 다이내믹 미디어 구성이 동일한지 및 [!DNL Brand Portal] 동일한지 확인하십시오.

>[!NOTE]
>
>비디오 뷰어 및 뷰어 사전 설정은에서 지원되지 [!DNL Brand Portal]않습니다. 기본 뷰어에서 비디오를 미리 보고 [!DNL Brand Portal]재생합니다.

## 전제 조건 {#prerequisites}

다이내믹 비디오를 사용한 [!DNL Brand Portal]작업을 하려면 다음을 수행해야 합니다.

* **DM (Dynamic Media) 모드에서[!DNL AEM]작성**[!DNL AEM] 시작 [!DNL Brand Portal][Dynamic Media 하이브리드 모드](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) 또는 [Dynamic Media [! DNL Scene 7 모드](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **다이내믹 미디어 모드 작성자를 기반으로[!DNL AEM]작성자에서**
Dynamic Media 클라우드 [!DNL AEM] 서비스를 구성하려면 [Dynamic Media 클라우드 서비스](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) 또는 [[! Tools from](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) [!DNL AEM] Author의 **Dnl Scene 7] 클라우드 서비스** | **클라우드 서비스** | **다이내믹 미디어.**
* **Author Dynamic Media on Brand Portal**
based on the Dynamic Media Cloud configurations on [!DNL AEM] author, configure [dynamic media settings](#configure-dm-hybrid-settings) or [[! DNL Scene 7의](#configure-dm-scene7-settings) [!DNL Brand Portal] 설정을 참조하십시오.
[[! DNL 브랜드 포털] 테넌트는](#separate-tenants) 다이내믹 [!DNL AEM] 미디어 하이브리드 및 다이내믹 미디어 S 7의 기능을 사용하는 경우 다이내믹 미디어 하이브리드 및 Dynamic Media [!UICONTROL Scene 7] 모드로 구성된 작성자 인스턴스에 [!UICONTROL 사용됩니다].
* **브랜드 포털에**
적용된 비디오 인코딩이 있는 폴더를 게시하면 [비디오 인코딩을](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) 적용하고 리치 미디어 에셋이 포함된 폴더를 [!DNL AEM] 작성자 인스턴스에서 [!DNL Brand Portal]에 게시합니다.
* **SPS에서 허용 목록 활성화 - 동적 미디어**([!DNL Scene 7] 회사에 [대해 보안 미리 보기가 활성화된](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) 경우)
를 사용하는 경우 SPS에서 IPS가 활성화된 경우 [!DNL Scene 7] 회사 관리자가 [SPS](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) ([!UICONTROL Scene 7] Publishing System) Flash UI를 사용하여 각 지역에 대한 공개 종료 IP를 화이트리스트에 추가하는 것을 권장합니다.
수신 IP는 다음과 같습니다.

| **지역** | **Egress IP** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

이러한 Egress IPS 중 하나를 허용 목록에 표시하려면 보안 테스트 서비스 계정을 [참조하십시오](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## 우수 사례

동적 비디오 에셋을 (및 공유 링크) 에서 [!DNL Brand Portal] 미리 보고, 재생하고, 다운로드했는지 확인하려면 다음 방법을 따르십시오.

### 다이내믹 미디어 하이브리드 및 Dynamic Media Scene 7 모드에 대한 테넌트 구분 {#separate-tenants}

다이내믹 미디어와 [!DNL Scene 7] 다이내믹 미디어 하이브리드 기능을 모두 사용하는 경우에는 다이내믹 미디어 하이브리드 및 [!DNL Brand Portal] 다이내믹 미디어 [!DNL AEM][!DNL Scene 7] 모드로 구성된 작성자 인스턴스에 대해 다른 임차인을 사용하는 것이 좋습니다.
![1 대 1 매핑 작성 및 BP](assets/BPDynamicMedia.png)

### AEM 작성자 인스턴스 및 브랜드 포털에서 동일한 구성 세부 정보

제목, 등록 ID, 비디오 서비스 URL (Dynamic Media 하이브리드) 및 제목, 자격 증명 (이메일 및 암호), 지역, 회사 (다이내믹 미디어 [!DNL Scene 7]) 와 같은 구성 세부 사항이 [!DNL Brand Portal] 동일한 [!DNL AEM] 클라우드 구성인지 확인합니다.

### 다이내믹 미디어 Scene 7 모드에 대한 화이트 리스트 공개 egress IPS

비디오 자산을 제공하는 Dynamic Media Scene 7 이 [](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)활성화된 경우 Scene 7 에서는 [!DNL Brand Portal]스테이징 환경 또는 내부 애플리케이션을 위한 전용 이미지 서버를 설정합니다. 이 서버에 대한 모든 요청은 원본 IP 주소를 확인합니다. 수신 요청이 승인된 IP 주소 목록에 없으면 실패 응답이 반환됩니다.
따라서 Scene -7 회사 관리자는 SPS (Scene -7 Publishing System) Flash UI를 통해 회사의 보안 테스트 환경에 대한 승인된 IP 주소 목록을 구성합니다. 해당 지역 (다음 사항에서) 에 대한 수신 IP가 승인된 목록에 추가되어 있는지 확인합니다.
이러한 Egress IPS 중 하나를 허용 목록에 표시하려면 보안 테스트 서비스 계정을 [참조하십시오](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
수신 IP는 다음과 같습니다.

| **지역** | **Egress IP** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Dynamic Media (하이브리드) 설정 구성 {#configure-dm-hybrid-settings}

[!DNL AEM] 작성자 인스턴스가 다이내믹 미디어 하이브리드 모드에서 실행 중인 경우, 관리 도구 패널의 비디오 타일을 사용하여 Dynamic Media Gateway 설정을 구성하십시오.
>[!NOTE]
>
>[비디오 인코딩 프로필은](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) 에 게시되지 [!DNL Brand Portal]않고 대신 Scene 7 서버에서 가져옵니다. 따라서 비디오 인코딩이 성공적으로 [!DNL Brand Portal]재생되도록 하려면 구성 세부 사항이 작성자 인스턴스의 [Scene 7 클라우드 구성과](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) [!DNL AEM] 같은지 확인하십시오.
임차인에 [!DNL Brand Portal] 대한 다이내믹 미디어 구성을 설정하려면:

1. 맨 위의 도구 모음에서 관리 도구에 액세스하려면 [!DNL AEM] 로고를 선택합니다 [!DNL Brand Portal].

2. 관리 도구 패널에서 **비디오** 타일을 선택합니다.
   ![브랜드 포털에서 다이내믹 미디어 하이브리드 구성](assets/DMHybrid-Video.png)
   **Edit Dynamic Media Configuration** 페이지가 열립니다.
   ![브랜드 포털에서 다이내믹한 미디어 하이브리드 구성](assets/edit-dynamic-media-config.png)

3. **등록 ID** 및 **비디오 서비스 URL** (DM-게이트웨이 URL) 를 지정합니다. 이러한 세부 사항이 작성자 인스턴스의 **도구** &gt; **클라우드 서비스에** 있는 것과 동일한지 [!DNL AEM] 확인하십시오.

4. **저장을** 선택하여 구성을 저장합니다.

## Dynamic Media Scene 7 설정 구성 {#configure-dm-scene7-settings}

[!DNL AEM] 작성자 인스턴스가 다이내믹 미디어- [!UICONTROL Scene 7] 모드에서 실행 중인 경우, 관리 도구 패널의 **Dynamic Media 구성** 타일을 사용하여 [!UICONTROL Scene 7] 서버 설정을 구성합니다.

임차인에 Dynamic Media [!UICONTROL Scene 7] 구성을 [!DNL Brand Portal] 설정하려면:

1. 맨 위의 도구 모음에서 관리 도구에 액세스하려면 [!DNL AEM] 로고를 선택합니다 [!DNL Brand Portal].

2. 관리 도구 패널에서 **다이내믹 미디어 구성** 타일을 선택합니다.
   ![[Dynamic Media 구성 편집] [!DNL Brand Portal]](assets/DMS7-Tile.png)페이지에서 [DM Scene 7 구성] 페이지가 열립니다.
   ![Scene 7 구성 [!DNL Brand Portal]](assets/S7Config.png)

3. 제공:
   * 제목
   * Scene 7 서버에 액세스하기 위한 자격 증명 (이메일 ID 및 암호)
   * 영역
이 값이 [!DNL AEM] 작성자 인스턴스의 값과 동일한지 확인합니다.

4. Select **Connect to Dynamic Media**.

5. **회사 이름을**&#x200B;입력하고 구성을 **저장합니다** .
