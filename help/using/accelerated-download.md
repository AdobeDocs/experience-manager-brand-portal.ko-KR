---
title: 브랜드 포털 다운로드 시간 단축
seo-title: 브랜드 포털 다운로드 시간 단축
description: 브랜드 포털 및 공유 링크에서 다운로드 성능을 향상시킵니다.
seo-description: 브랜드 포털 및 공유 링크에서 다운로드 성능을 향상시킵니다.
uuid: 2871137e-6471-49a7-872a-841bd92543d1
contentOwner: mgulati
topic-tags: download-install
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 301f7a0b-5527-4aac-b731-bfc145fed0c0
translation-type: tm+mt
source-git-commit: 45664ffc0a5eb36e941d75a5773ef59cfa6b4646
workflow-type: tm+mt
source-wordcount: '1107'
ht-degree: 2%

---


# 브랜드 포털 다운로드 시간 단축 {#guide-to-accelerate-downloads-from-brand-portal}

브랜드 포털을 통해 IBM Aspera Connect와 통합하여 대용량 에셋 파일의 다운로드 성능을 향상시킬 수 있습니다. 이 애플리케이션은 독점적 기술을 사용하여 TCP 오버헤드를 제거하고 에셋 파일의 전송 속도를 향상시킵니다. 이러한 통합을 통해 다운로드 환경이 개선되었습니다.

>[!NOTE]
>
>다운로드 속도는 네트워크 대역폭, 서버 지연 및 클라이언트의 지리적 위치 등의 요인에 따라 다르므로 사용자에 따라 다릅니다.

빠른 **[!UICONTROL 다운로드]** 구성은 기본적으로 활성화되므로 브랜드 포털에서 원하는 에셋 파일을 다운로드하는 데 걸리는 시간이 크게 줄어듭니다.

![](assets/download-configuration.png)

## 파일 다운로드 속도를 높이기 위한 사전 요구 사항 {#prerequisites-to-accelerate-file-download}

파일을 더 빨리 다운로드하려면 다음을 확인하십시오.

* [ **[!UICONTROL 도구]** ] > [ **[!UICONTROL 다운로드]** ]로 이동하여 **[!UICONTROL [다운로드 설정]** ]에서 **[!UICONTROL 빠른 다운로드]**&#x200B;구성이활성화되었는지 확인합니다.
* 포트 33001(TCP 및 UDP 모두)이 방화벽에서 열려 있는지 확인합니다. 사전 요구 사항에 대한 자세한 내용은 [IBM Aspera Connect Client 설명서를 참조하십시오](https://downloads.asperasoft.com/en/documentation/8).
* [관리자 권한을 사용하여 브라우저의 익스텐션에 IBM Aspera Connect 3.9.9를](https://www.ibm.com/support/knowledgecenter/SSXMX3_3.9.9/kc/connect_welcome.html) 설치합니다.
* Aspera 전송 클라이언트 플랫폼에 대한 지원은 [IBM Aspera Connect 플랫폼 지원 매트릭스를 참조하십시오](https://www.asperasoft.com/company/support/transfer-clients/).

## 도메인 다운로드 {#download-domains}

다른 지역에 대한 다운로드 도메인은 다음과 같습니다.

| 지역 코드 | 도메인 |
|---|---|
| NA OR1 | downloads-na1.brand-portal.adobe.com |
| NA VA5 | downloads-na2.brand-portal.adobe.com |
| EMEA LON5 | downloads-emea1.brand-portal.adobe.com |
| APAC SIN2 | downloads-apac1.brand-portal.adobe.com |

## 파일 가속기를 사용한 다운로드 성능 샘플 {#expected-download-performance-using-file-accelerator}

다음 표는 Aspera Connect 파일 다운로드 가속기를 사용한 2GB 파일의 다운로드 성능을 보여줍니다.

*Brand Portal 서버가 오레곤(미국)에 있는 것을 고려하여 관찰된 결과는 네트워크 대역폭, 서버 지연, 클라이언트 위치 등의 요인에 따라 달라집니다.*

| 클라이언트 위치 | 클라이언트와 서버 간의 지연(밀리초) | Aspera Connect 파일 전송 가속기를 사용한 속도 | Aspera File Transfer Accelerator를 사용하여 2GB 파일을 다운로드하는 데 걸린 시간(초) |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| 미국 서부(캘리포니아 주) | 18 | 36 | 57 |
| 미국 서부(오레곤) | 42 | 36 | 57 |
| 미국 동부(버지니아 주) | 85 | 35 | 58 |
| APAC(도쿄) | 124 | 36 | 57 |
| 노이다(인도) | 275 | 13.36 | 153 |
| 시드니 | 175 | 29 | 70 |
| 런던 | 179 | 35 | 58 |
| 싱가포르 | 196 | 34 | 60 |

## 파일 가속기를 사용하여 워크플로우 다운로드 {#download-workflow-using-file-accelerator}

브랜드 포털에서 에셋을 보다 빠르게 다운로드하려면

1. 지원되는 브라우저를 사용하여 브랜드 포털에 로그인합니다.
1. 다운로드할 폴더 또는 자산을 찾아보고 선택합니다. 상단에 있는 도구 모음에서 **[!UICONTROL 다운로드]** 아이콘을 클릭합니다. 자산 **[!UICONTROL 및 다운로드 가속]** **[!UICONTROL 활성화]** 확인란은 기본적으로 선택되어 **[!UICONTROL 있는]** 상태로 나타납니다.

   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >자산 다운로드 링크가 포함된 이메일 알림을 전송하는 기능은 현재 더 빠른 다운로드가 활성화된 상태에서 지원되지 않습니다.

   ![](assets/fast-download-emailchk.png)

1. 다운로드를 **[!UICONTROL 클릭합니다]**.

   브랜드 포털 테넌트 계정에서 다운로드 경험을 가속화하려면 브라우저 익스텐션에 Aspera Connect 클라이언트 응용 프로그램을 설치해야 합니다.

1. **Aspera Connect 클라이언트 다운로드**

   시스템에 Aspera Connect 클라이언트가 설치되어 있지 않거나 기존 Aspera Connect 클라이언트가 오래된 경우 [최신 버전 **[!UICONTROL 다운로드]를 선택하여 시스템별 Aspera Connect 클라이언트를 다운로드할 수 있는 브라우저 페이지에 메시지가 표시됩니다]**.

   ![](assets/aspera-not-launched.png)

   https://downloads.asperasoft.com/connect2/에서 최신 버전의 Aspera Connect를 [다운로드하려면 [지금](https://downloads.asperasoft.com/connect2/)**** 다운로드]를 선택하고 지침을 따릅니다.

1. **Aspera Connect 클라이언트 설치**

   IBM Aspera Connect 클라이언트 설정을 설치하려면 IBM Aspera Connect 클라이언트 응용 프로그램의 .msi 파일에서 설치 프로그램을 실행하고 설치 마법사를 따릅니다.

1. 클라이언트가 성공적으로 설치되면 브라우저 페이지를 새로 고친 후 다운로드 단계를 다시 시작합니다.

   Aspera Connect를 처음 사용하는 경우 브라우저에서 **[!UICONTROL IBM Aspera Connect를 사용하여 링크를 열라는 메시지가 표시됩니다]**. 나중에 이 대화 상자를 건너뛰려면 FASP 링크 **[!UICONTROL 에 대해 내 선택 사항을 기억하기를 활성화합니다]**.

   >[!NOTE]
   >
   >이 메시지는 브라우저마다 다릅니다.

1. 전송을 진행할지 여부를 확인하는 대화 상자가 나타납니다. 시작 **[!UICONTROL 허용을]** 선택합니다.
나중에 이 대화 상자를 건너뛰려면 이 호스트 **[!UICONTROL 와의 모든 연결에 내 선택 사항을 사용하십시오]**.
다운로드가 시작됩니다. 다운로드 진행 상황을 대화 상자에 표시합니다. 대화 상자를 사용하여 다운로드를 **[!UICONTROL 일시]**&#x200B;중지하거나 **[!UICONTROL 다시]**&#x200B;시작하거나 **[!UICONTROL 취소할]** 수있습니다.
Aspera Connect 응용 프로그램은 사용자가 모든 전송 세션을 보고 관리할 수 있는 시스템의 활동 창을 제공합니다. 자세한 내용은 [Aspera Connect 클라이언트 설명서를 참조하십시오](https://downloads.asperasoft.com/en/documentation/8).

![](assets/aspera-activity-window.png)

다운로드가 성공적으로 완료되면 사용자 시스템에 자산이 다운로드되는 위치가 대화 상자에 표시됩니다. 오류가 있으면 오류가 표시됩니다.

>[!NOTE]
>
>Aspera Connect 클라이언트 응용 프로그램에서는 [환경 설정] 내의 [탭 **[!UICONTROL 전송]에서 다운로드한 파일을]** 저장할 위치를 항상 묻는 메시지가 나타날 때 다운로드 위치를 선택하라는 메시지가 표시되지 않는 알려진 제한 사항이 **[!UICONTROL 있습니다]** ****. 다운로드가 시작되기 전에 다운로드한 파일을 저장할 위치 텍스트 상자 **[!UICONTROL 의 위치를 입력하십시오]**.

## Microsoft Edge 브라우저에서 파일 가속기 사용 {#using-file-accelerator-on-microsoft-edge-browser}

Microsoft Edge는 EPM(Enhanced Protected Mode)에서 실행되므로 동일한 개인 네트워크 또는 신뢰할 수 있는 사이트와의 통신을 방지할 수 있습니다. 따라서 서버와의 연결이 설정될 때마다 팝업이 표시됩니다.

![](assets/switchapps-msedge.png)

Microsoft Edge에서 가속화된 다운로드 기능을 사용하려면 신뢰할 수 있는 사이트 목록에서 브랜드 포털 사이트를 제거하십시오.

1. Campaign 컨트롤 패널을 엽니다(**[!UICONTROL 창 키 + X]**, **[!UICONTROL Campaign 컨트롤 패널]**&#x200B;선택).
1. [ **[!UICONTROL 네트워크 및 인터넷]** ] > [ **[!UICONTROL 인터넷 옵션]으로 이동합니다]**. Click the **[!UICONTROL Security]** tab.
1. 신뢰할 수 **[!UICONTROL 있는 사이트 영역을]**&#x200B;클릭한 다음 **[!UICONTROL 사이트를 클릭합니다]**.
1. 목록에서 브랜드 포털 사이트를 제거합니다.

## Aspera Connect 클라이언트 환경 설정 {#aspera-connect-client-preferences}

IBM Aspera Connect Client 환경 설정에서 아이콘을 마우스 오른쪽 단추로 클릭하고 [환경 설정]을 선택하여 설정할 수 있는 몇 가지 유용한 기본 설정이 **[!UICONTROL 있습니다]**.

![](assets/download_assets_frombrandportalimg19.png)

기본 다운로드 위치를 설정할 수 있습니다.

![](assets/aspera-preferences.png)

또한 Aspera Connect 클라이언트는 시스템 시작 시 자동으로 시작되도록 표시되므로 Connect 클라이언트가 실행 중이며 다운로드를 빠르게 시작할 수 있습니다.

![](assets/aspera-automaticallylaunch.png)

## 다운로드 가속화 문제 해결 {#troubleshoot-issues-with-download-acceleration}

다운로드 가속이 작동하지 않는 경우 다음 단계에 따라 문제를 해결하십시오.

1. 시스템에서 https://test-connect.asperasoft.com을 방문하여 포트가 [차단되어](https://test-connect.asperasoft.com/) 있는지 확인하십시오.

   포트가 OK되지 않으면 네트워크 팀에 연락하여 포트 33001(TCP 및 UDP 모두)이 방화벽에서 차단되지 않았는지 확인합니다.

1. 포트가 정상 상태인 경우 https://www.speedtest.net/을 사용하여 사용 가능한 대역폭을 측정하여 네트워크 속도가 느려지지 않은지 [확인하십시오](https://www.speedtest.net/).

   대역폭이 몇 가지(1-10Mbps) 또는 Kbps인 경우 Aspera 환경 설정을 사용하고 사용 가능한 대역폭과 동일한 대역폭을 제한하십시오.

1. Aspera 데모 서버의 다운로드 작동 여부를 확인하려면 https://demo.asperasoft.com/aspera/user을 [사용하십시오](https://demo.asperasoft.com/aspera/user).\
   (로그인: 아스퍼웹, 암호: 데모스페르타 )

1. 위의 문제 해결 단계 중 아무 것도 작동하지 않으면 [다운로드 가속 사용] 옵션을 선택 취소하고 일반 다운로드를 사용하십시오.
