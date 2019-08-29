---
title: 사용자, 그룹 및 사용자 역할 관리
seo-title: 사용자, 그룹 및 사용자 역할 관리
description: 관리자는 Adobe Admin Console를 사용하여 AEM Assets 브랜드 포털 사용자 및 제품 프로필을 만들고 브랜드 포털 사용자 인터페이스를 사용하여 자신의 역할을 관리할 수 있습니다. 이 권한은 뷰어 및 편집자는 사용할 수 없습니다.
seo-description: 관리자는 Adobe Admin Console를 사용하여 AEM Assets 브랜드 포털 사용자 및 제품 프로필을 만들고 브랜드 포털 사용자 인터페이스를 사용하여 자신의 역할을 관리할 수 있습니다. 이 권한은 뷰어 및 편집자는 사용할 수 없습니다.
uuid: 0 dc 1867 c -6 d 1 b -4 d 0 d-a 25 e -0 df 207 c 269 b 8
content-type: 참조
topic-tags: 관리
products: sg_ Experiencemanager/brand_ portal
discoiquuid: BA 468 E 80-D 077-4 AF 6-B 782-238 FC 557 E 22 B
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# 사용자, 그룹 및 사용자 역할 관리 {#manage-users-groups-and-user-roles}

관리자는 사용자 및 제품 [!DNL Adobe Admin Console] 프로필을 만들고 [!DNL AEM Assets Brand Portal] 브랜드 포털 사용자 인터페이스를 사용하여 자신의 역할을 관리할 수 있습니다. 이 권한은 뷰어 및 편집자는 사용할 수 없습니다.

[관리 콘솔에서](http://adminconsole.adobe.com/enterprise/overview)조직과 연계된 모든 제품을 볼 수 있습니다. 제품은, 또는과 같은 [!DNL Experience Cloud][!DNL Adobe Analytics]모든 솔루션이 될 [!DNL Adobe Target][!DNL AEM Brand Portal]수 있습니다. AEM 브랜드 포털 제품을 선택하고 제품 프로필을 만들어야 합니다.

<!--
Comment Type: draft

<note type="note">
<p>Product Profiles (formerly known as product configurations*). </p>
<p>* The nomenclature has changed from product configurations to product profiles in the new Adobe Admin Console.</p>
</note>
-->
![](assets/create-user-group.png)

이러한 제품 프로필은 8 시간마다 [!DNL Brand Portal] 사용자 인터페이스와 동기화되고 그룹으로 [!DNL Brand Portal]표시됩니다. 사용자를 추가하고 제품 프로필을 만들고 해당 제품 프로필에 사용자를 추가하면에서 사용자 및 그룹에 역할을 할당할 [!DNL Brand Portal]수 있습니다.

>[!NOTE]
>
>에서 그룹을 [!DNL Brand Portal]만들려면, 사용자 [!DNL Adobe Admin Console]페이지 &gt; 사용자 그룹 대신 **제품** 페이지 &gt; ****&#x200B;제품 **프로필을** **사용하십시오**. 의 [!DNL Adobe Admin Console] 제품 프로파일은 그룹을 만드는 데 사용됩니다 [!DNL Brand Portal].

## 사용자 추가 {#add-a-user}

제품 관리자인 경우 [[! DNL Adobe Admin Console를](http://adminconsole.adobe.com/enterprise/overview) 사용하여 사용자를 만들고 (*이전 제품 구성*) 에 그룹으로 표시되는 제품 프로필에 할당합니다 [!DNL Brand Portal]. 그룹을 사용하여 역할 관리 및 자산 공유와 같은 일괄 작업을 수행할 수 있습니다.

>[!NOTE]
액세스 권한이 없는 새 사용자는의 [!DNL Brand Portal] 로그인 화면에서 액세스 권한을 요청할 [!DNL Brand Portal]수 있습니다. 자세한 내용은 [[DNL 브랜드 포털]](../using/brand-portal.md#request-access-to-brand-portal)를 참조하십시오. 알림 영역에서 액세스 요청 알림을 받은 후 관련 알림을 클릭한 다음 액세스 **권한 부여를 클릭합니다**. 또는, 받은 액세스 요청 이메일의 링크를 따릅니다. 다음으로 사용자를 추가하려면 [[! DNL Adobe Admin Console]](http://adminconsole.adobe.com/enterprise/overview)아래 절차의 4-7 단계를 따르십시오.

>[!NOTE]
[ [! DNL Adobe Admin Console를](http://adminconsole.adobe.com/enterprise/overview) [!DNL Brand Portal]직접 또는에서 사용 직접 로그인하는 경우 아래 절차의 4-7 단계를 수행하여 사용자를 추가합니다.

1. 상단에 [!DNL AEM] 있는 도구 모음에서 Adobe 로고를 클릭하여 관리 도구에 액세스합니다.

   ![AEM 로고](assets/aemlogo.png)

2. [관리 도구] 패널에서 **[사용자**] 를 클릭합니다.

   ![관리 툴 패널](assets/admin-tools-panel-5.png)

3. **사용자 역할** 페이지에서 **관리** 탭을 클릭한 다음 관리 콘솔 **시작을**&#x200B;클릭합니다.

   ![Admin Console를 시작할 사용자 역할](assets/launch_admin_console.png)

4. 관리 콘솔에서 다음 중 하나를 수행하여 새 사용자를 만듭니다.

   * 상단에 있는 도구 모음에서 **개요를**&#x200B;클릭합니다. **개요** 페이지에서 제품 **카드에서 사용자** 할당을 **[!DNL AEM Brand Portal]** 클릭합니다.
   ![관리 콘솔 개요](assets/admin_console_overviewadduser.png)

   * 맨 위의 도구 모음에서 **사용자를 클릭합니다**. **사용자** 페이지에서 왼쪽 레일의 **사용자는** 기본적으로 선택됩니다. 사용자 **추가를**&#x200B;클릭합니다.
   ![Admin Console 사용자 추가](assets/admin_console_adduseruserpage.png)

5. 사용자 추가 대화 상자에서 사용자가 입력할 때 나타나는 제안 목록에서 사용자를 추가하거나 선택할 사용자의 이메일 ID를 입력합니다.

   ![브랜드 포털에 사용자 추가](assets/add_user_to_aem_bp.png)

6. 사용자가 브랜드 포털에 액세스할 수 있도록 하나 이상의 제품 프로필 (이전의 제품 구성) 에 사용자를 할당합니다. **해당 제품** 프로필에 대한 프로파일을 선택하십시오. 에서 해당 제품 프로필을 선택합니다.
7. **저장**&#x200B;을 클릭합니다. 추가된 사용자에게 환영 이메일이 전송됩니다. 초대받은 사용자는 환영 이메일의 링크를 클릭하고 Adobe ID를 사용하여 [!DNL Brand Portal] 로그인함으로써 액세스할 수 있습니다. 자세한 내용은 최초 로그인 환경을 참조하십시오 [](../using/brand-portal-onboarding.md).

   >[!NOTE]
   사용자가 로그인할 수 없는 [!DNL Brand Portal]경우 조직의 관리자가 Adobe [!UICONTROL Admin Console] 를 방문하여 사용자가 존재하는지와 하나 이상의 제품 프로필에 추가되었는지 확인해야 합니다.

   사용자에게 관리 권한을 부여하는 방법에 대한 자세한 내용은 사용자에게 관리자 권한 [제공을](../using/brand-portal-adding-users.md#provideadministratorprivilegestousers)참조하십시오.

## 제품 프로필 추가 {#add-a-product-profile}

[!UICONTROL 관리 콘솔에서 제품 프로필 (이전 제품 구성) 는 그룹을 만드는 데] 사용되므로 [!DNL Brand Portal] 역할 관리 및 자산 공유와 같은 일괄 작업을 수행할 수 [!DNL Brand Portal]있습니다. **[!DNL Brand Portal]** 는 사용 가능한 기본 제품 프로필입니다. 더 많은 제품 프로필을 만들고 새 제품 프로필에 사용자를 추가할 수 있습니다.

>[!NOTE]
[ [! Uicontrol Admin Console를](http://adminconsole.adobe.com/enterprise/overview) 직접 또는 [!DNL Brand Portal]에서 관리 [!UICONTROL Admin Console에] 직접 로그인하는 경우 아래 절차의 4-7 단계를 수행하여 제품 프로필을 추가합니다.

1. 상단에 [!DNL AEM] 있는 도구 모음에서 Adobe 로고를 클릭하여 관리 도구에 액세스합니다.

   ![[!DNL AEM] 로고](assets/aemlogo.png)

2. [관리 도구] 패널에서 **[사용자**] 를 클릭합니다.

   ![관리 툴 패널](assets/admin-tools-panel-6.png)

3. **사용자 역할** 페이지에서 **관리** 탭을 클릭한 다음 관리 콘솔 **시작을**&#x200B;클릭합니다.

   ![Admin Console 실행](assets/launch_admin_console.png)

4. 상단에 있는 도구 모음에서 **제품을**&#x200B;클릭합니다.
5. **제품** 페이지에서는 **기본적으로 제품 프로필이** 선택됩니다. 새 프로필을 ****&#x200B;클릭합니다.

   ![새 제품 프로필 추가](assets/admin_console_addproductprofile.png)

6. 새 프로필 **만들기** 페이지에서 프로필 이름, 표시 이름, 프로필 설명 및 프로필에 추가 또는 제거될 때 이메일로 사용자에게 알림을 제공할지 여부를 선택합니다.

   ![제품 프로필 만들기](assets/admin_console_addaproductprofilecreatenewprofile.png)

7. **완료를**&#x200B;클릭합니다. 제품 구성 그룹 (예: **영업 그룹**) 이 브랜드 포털에 추가됩니다.

   ![제품 프로필](assets/admin_console_productprofileadded.png)

## 제품 프로필에 사용자 추가 {#add-users-to-a-product-profile}

[!DNL Brand Portal] 그룹에 사용자를 추가하려면 [!UICONTROL 관리 콘솔에서 해당 제품 프로필 (이전 제품 구성) 에 추가합니다]. 사용자를 개별적으로 또는 일괄 추가할 수 있습니다.

>[!NOTE]
[ [! DNL Admin Console를](http://adminconsole.adobe.com/enterprise/overview) [!DNL Brand Portal]직접 또는에서 사용할 수 있습니다. Admin Console에 직접 로그인하는 경우 아래 절차의 4-7 단계를 수행하여 사용자를 제품 프로필에 추가합니다.

1. 상단에 [!DNL AEM] 있는 도구 모음에서 Adobe 로고를 클릭하여 관리 도구에 액세스합니다.

   ![[!DNL AEM] 로고](assets/aemlogo.png)

2. [관리 도구] 패널에서 **[사용자**] 를 클릭합니다.

   ![관리 툴 패널](assets/admin-tools-panel-7.png)

3. **사용자 역할** 페이지에서 **관리** 탭을 클릭한 다음 관리 콘솔 **시작을**&#x200B;클릭합니다.

   ![Launch [!DNL Admin Console]](assets/launch_admin_console.png)

4. 상단에 있는 도구 모음에서 **제품을**&#x200B;클릭합니다.
5. **제품** 페이지에서는 **기본적으로 제품 프로필이** 선택됩니다. 사용자 (예: **영업 그룹**) 를 추가할 제품 프로필을 엽니다.

   ![제품 프로필](assets/admin_console_productprofileadded.png)

6. 개별 사용자를 제품 프로필에 추가하려면 다음을 수행하십시오.

   * 사용자 **추가를**&#x200B;클릭합니다.
   ![제품 프로필을 매핑할 그룹 [!DNL Brand Portal]](assets/admin_console_productprofilesalesgroup.png)

   * 영업 그룹에 사용자 **추가** 페이지에 입력하는 동안 나타나는 제안 목록에서 사용자를 추가하거나 선택할 사용자의 이메일 ID를 입력합니다.
   ![그룹에 사용자 추가](assets/admin_console_addusertosalesgroup.png)

   * **저장**&#x200B;을 클릭합니다.



7. 제품 프로필에 벌크 사용자를 추가하려면 다음을 수행하십시오.

   * 줄임표(...)****&gt; CSV로 사용자 **추가를**&#x200B;선택합니다.
   ![일괄 사용자 추가](assets/admin_console_addbulkusers.png)

   * CSV로 사용자 **추가** 페이지에서 CSV 템플릿을 다운로드하거나 CSV 파일을 드래그하여 놓습니다.
   ![CSV로 사용자 추가](assets/admin_console_addbulkuserscsv.png)

   * **업로드를**&#x200B;클릭합니다.
   기본 제품 프로필에 사용자를 추가하면 시작 [!DNL Brand Portal]이메일이 추가한 사용자의 이메일 ID로 전송됩니다. 초대받은 사용자는 환영 [!DNL Brand Portal] 이메일의 링크를 클릭하고 [!UICONTROL Adobe ID를 사용하여 로그인하여 액세스할]수 있습니다. 자세한 내용은 최초 로그인 환경을 참조하십시오 [](../using/brand-portal-onboarding.md).

   사용자 지정 또는 새 제품 프로필에 추가된 사용자는 이메일 알림을 받지 않습니다.

## 사용자에게 관리자 권한 제공 {#provide-administrator-privileges-to-users}

사용자에게 시스템 관리자 또는 제품 관리자 권한을 제공할 [!DNL Brand Portal] 수 있습니다. [!UICONTROL 관리 콘솔에서]제품 프로필 관리자, 사용자 그룹 관리자 및 지원 관리자와 같은 다른 관리 권한을 제공하지 마십시오. 이러한 역할에 대한 자세한 내용은 [관리 역할을](https://helpx.adobe.com/enterprise/using/admin-roles.html)참조하십시오.

>[!NOTE]
[ [! Uicontrol Admin Console를](https://adminconsole.adobe.com/enterprise/overview) 직접 또는 [!DNL Brand Portal]에서 관리 [!UICONTROL Admin Console에] 직접 로그인하는 경우 아래 절차의 4-8 단계를 수행하여 사용자를 제품 프로필에 추가합니다.

1. 상단에 [!DNL AEM] 있는 도구 모음에서 Adobe 로고를 클릭하여 관리 도구에 액세스합니다.

   ![Aemlogo](assets/aemlogo.png)

2. [관리 도구] 패널에서 **[사용자**] 를 클릭합니다.

   ![관리 툴 패널](assets/admin-tools-panel-8.png)

3. **사용자 역할** 페이지에서 **관리** 탭을 클릭한 다음 관리 콘솔 **시작을**&#x200B;클릭합니다.

   ![Admin Console 실행](assets/launch_admin_console.png)

4. 맨 위의 도구 모음에서 **사용자를 클릭합니다**.
5. **사용자** 페이지에서 왼쪽 레일의 **사용자는** 기본적으로 선택됩니다. 관리자 권한을 제공할 사용자의 사용자 이름을 클릭합니다.

   ![Admin Console에서 사용자 추가](assets/admin_console_adduseruserpage.png)

6. [사용자 프로필] 페이지에서 아래쪽에 있는 **[관리 권한]** 섹션을 찾아 줄임표(...)****&gt; [관리자 권한 **편집**] 를 선택합니다.
   ![관리 콘솔의 관리자 권한](assets/admin_console_editadminrights.png)

7. 관리 **편집** 페이지에서 시스템 관리자 또는 제품 관리자를 선택합니다.

   ![관리 콘솔에서 관리자 권한 편집](assets/admin_console_editadminrightsselection.png)

   >[!NOTE]
   [!DNL Brand Portal] 시스템 관리자 및 제품 관리자 역할만 지원합니다.
   [!DNL Adobe] 조직의 모든 제품에 대한 조직 전체의 관리자 권한을 부여하므로 시스템 관리자 역할을 사용하지 않는 것이 좋습니다. 예를 들어 세 개의 Marketing Cloud 제품이 포함된 조직의 시스템 관리자는 세 가지 제품에 대한 전체 권한 세트를 갖습니다. 자산을 자산에서에 게시할 수 있도록 시스템 관리자만 [!DNL AEM] 자산을 구성할 수 [!DNL AEM][!DNL Brand Portal]있습니다. 자세한 내용은 [[DNL 브랜드 포털]](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html)를 참조하십시오.
   이와 반대로 제품 관리자 역할은 특정 제품에 대해서만 관리자 권한을 부여합니다. 보다 [!DNL Brand Portal]세부적인 액세스 제어를 실행하려면 제품 관리자 역할을 사용하고 해당 제품을 선택합니다 **[!DNL AEM Brand Portal]**.

   >[!NOTE]
   [!DNL Brand Portal] 는 제품 프로필 관리자 (이전의 구성 관리자) 권한을 지원하지 않습니다. 사용자에게 제품 프로필 관리자 권한을 할당하지 마십시오.

8. 관리 유형 선택 항목을 검토하고 **저장을 클릭합니다**.

   >[!NOTE]
   사용자에 대한 관리자 권한을 취소하려면 [관리 **편집** ] 페이지에서 적절한 변경을 수행한 다음 [ **저장**] 를 클릭합니다.

## 사용자 역할 관리 {#manage-user-roles}

관리자는 사용자의 역할을 수정할 [!DNL Brand Portal]수 있습니다.

관리자 역할 외에도 다음 역할을 [!DNL Brand Portal] 지원합니다.

* **뷰어**: 이 역할의 사용자는 관리자가 공유하는 파일과 폴더를 볼 수 있습니다. 뷰어는 자산을 검색하고 다운로드할 수도 있습니다. 그러나 뷰어는 다른 사용자와 콘텐트 (파일, 폴더, [!UICONTROL 컬렉션]) 를 공유할 수 없습니다.
* **편집기**: 이 역할의 사용자에게는 뷰어의 모든 권한이 있습니다. 또한 편집자는 다른 사용자와 콘텐트 (폴더, [!UICONTROL 컬렉션], 링크) 를 공유할 수 있습니다.

1. 상단에 [!DNL AEM] 있는 도구 모음에서 Adobe 로고를 클릭하여 관리 도구에 액세스합니다.

   ![Aemlogo](assets/aemlogo.png)

2. [관리 도구] 패널에서 **[사용자**] 를 클릭합니다.

   ![관리 툴 패널](assets/admin-tools-panel-9.png)

3. 사용자 **역할** 페이지에서 **기본적으로 사용자** 탭이 선택되어 있습니다. 역할을 변경할 사용자의 경우 [역할] 드롭다운에서 **[편집기** ] 또는 **[뷰어]** **를 선택합니다** .

   ![사용자 역할 수정](assets/modify_user_role.png)

   여러 사용자의 역할을 동시에 수정하려면 사용자를 선택하고 **역할** 드롭다운에서 적절한 역할을 선택합니다.

   >[!NOTE]
   관리자 사용자를 위한 **역할** 목록은 비활성화됩니다. 이러한 사용자를 선택하여 역할을 수정할 수 없습니다.

   >[!NOTE]
   사용자가 편집기 그룹의 구성원이면 사용자 역할도 비활성화됩니다. 사용자로부터 편집 권한을 취소하려면 편집기 그룹에서 사용자를 제거하거나 전체 그룹의 역할을 뷰어로 변경합니다.

4. **저장**&#x200B;을 클릭합니다. 해당 사용자에 대해 역할이 수정됩니다. 여러 사용자를 선택한 경우 모든 사용자에 대한 역할이 동시에 수정됩니다.

   >[!NOTE]
   사용자 권한의 변경 사항은 사용자가 브랜드 포털에 다시 로그인한 후에만 [ **사용자 역할** ] 페이지에 반영됩니다.

## 그룹 역할 및 권한 관리 {#manage-group-roles-and-privileges}

관리자는 브랜드 포털에서 특정 권한을 사용자 [그룹과](../using/brand-portal-adding-users.md#main-pars-title-278567577) 연결할 수 있습니다. **관리자는** **[사용자 역할** ] 페이지의 [그룹] 탭을 사용하여 다음을 수행할 수 있습니다.

* 사용자 그룹에 역할 할당
* 사용자 그룹을 제한하여 이미지 파일의 원본 변환을 다운로드합니다 (.jpeg. tiff. png. bmp. gif. pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image)./x-photoshop. psd, image/vnd. adobe. photoshop를 브랜드 포털에서 다운로드할 수 있습니다.

>[!NOTE]
링크로 공유되는 자산의 경우, 이미지 파일의 원본 변환에 액세스할 수 있는 권한은 자산을 공유하는 사용자의 권한에 따라 적용됩니다.

특정 그룹 구성원의 원래 변환에 액세스할 수 있는 역할과 권한을 수정하려면 다음 단계를 수행하십시오.

1. **사용자 역할** 페이지에서 **그룹** 탭으로 이동합니다.
2. 역할을 변경할 그룹을 선택합니다.
3. **역할** 드롭다운 목록에서 적절한 역할을 선택합니다.

   그룹 구성원이 이미지 파일의 원본 변환에 액세스할 수 있게 하려면 (.jpeg. tiff. png. bmp. gif. pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon), image/photoshop, image/x-photoshop. psd, image/vnd. adobe. photoshop) 포털 또는 공유 링크에서 다운로드하는 경우 해당 그룹에 **대해 선택된 원본** 옵션을 유지합니다. 기본적으로 **모든 사용자에 대해 원본** 액세스 옵션이 선택되어 있습니다. 사용자 그룹이 원래 변환에 액세스하지 못하도록 하려면 해당 그룹에 해당하는 옵션을 선택 취소합니다.

   ![사용자 그룹 역할](assets/access-original-rend.png)

   >[!NOTE]
   사용자가 여러 그룹에 추가되고 이러한 그룹 중 하나에 제한 사항이 있는 경우 제한 사항이 해당 사용자에게 적용됩니다.
   또한 제한된 그룹 구성원인 경우에도 이미지 파일의 원래 변환에 액세스하는 제한 사항은 관리자에게는 적용되지 않습니다.

4. **저장**&#x200B;을 클릭합니다. 해당 그룹에 대해 역할이 수정됩니다.

   >[!NOTE]
   사용자 대 그룹 연결 또는 사용자의 그룹 멤버십은 8 시간마다 [!DNL Brand Portal] 동기화됩니다. 다음 동기화 작업이 실행된 후에는 사용자 또는 그룹 역할에 대한 변경 사항이 적용됩니다.
