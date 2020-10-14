---
title: 기여도 폴더 만들기
seo-title: 기여도 폴더 만들기
description: 'AEM Assets에서 기여도 폴더를 만드는 방법에 대한 통찰력을 얻을 수 있습니다. '
seo-description: AEM Assets에서 기여도 폴더를 만드는 방법에 대한 통찰력을 얻을 수 있습니다.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 2f6ec4ac56390b2243e1d1a2c2adb34eb9aad7b2
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 3%

---


# Create contribution folder {#create-contribution-folder}


AEM 관리자 및 새 폴더를 만들 권한이 있는 비관리 사용자는 AEM Assets에서 기여도 폴더를 만들 수 있습니다.
기여도 폴더를 만들려면 자산 기여도 유형의 새 폴더를 만듭니다. 이 폴더를 만들면 브랜드 포털 사용자의 자산 제출이 가능합니다.  이렇게 하면 기여도 폴더 내에 SHARED 및 NEW라는 두 개의 하위 폴더가 추가로 생성되는 워크플로우가 자동으로 트리거됩니다.

>[!NOTE]
>
>한 폴더 내에 여러 기여도 폴더를 만들 수는 있지만 다른 기여도 폴더 내에 기여도 폴더를 만들 수는 없습니다.

기여도 폴더를 만들려면:
1. AEM 작성자 인스턴스에 로그인합니다.

   기본 URL은 http:// localhost:4502/aem/start.html입니다.

1. 자산 **[!UICONTROL > 파일]** 으로 **[!UICONTROL 이동합니다]**. AEM Assets 저장소의 모든 기존 폴더가 나열됩니다.

1. Click **[!UICONTROL Create]** to create a new folder. **[!UICONTROL 폴더 만들기]** 대화 상자가 열립니다.

1. 폴더의 **[!UICONTROL 제목]****[!UICONTROL 및]** 이름을 **[!UICONTROL 입력하고 자산 기여도]** 확인란을선택합니다.
폴더 이름을 지정하려면 공백 없이 소문자를 사용하는 것이 좋습니다.

1. **[!UICONTROL 만들기]**&#x200B;를 클릭합니다. AEM Assets 저장소에 나열된 기여도 폴더를 볼 수 있습니다.

   >[!NOTE]
   >
   >관리자가 아닌 사용자는 자산 기여도 폴더를 만들고 공유할 수 있지만 수정하거나 삭제할 수 없습니다.


   ![](assets/create-contribution-folder.png)

1. 기여도 폴더를 열려면 아이콘을 클릭합니다. 두 개의 하위 폴더가 표시됩니다.**[!UICONTROL SHARED]** 및 **[!UICONTROL NEW]** 는 기여도 폴더 내에 자동으로만들어집니다.

   ![](assets/contribution-folder.png)

이제 기여도 폴더 속성을 [구성할 수 있습니다](brand-portal-configure-contribution-folder-properties.md).


