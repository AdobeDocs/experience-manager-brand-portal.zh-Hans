---
title: 管理用户、组和用户角色
seo-title: 管理用户、组和用户角色
description: 管理员可以使用Adobe Admin Console创建AEM Assets品牌门户用户和产品用户档案，并使用品牌门户用户界面管理他们的角色。 此权限对查看者和编辑者不可用。
seo-description: 管理员可以使用Adobe Admin Console创建AEM Assets品牌门户用户和产品用户档案，并使用品牌门户用户界面管理他们的角色。 此权限对查看者和编辑者不可用。
uuid: 0dc1867c-6d1b-4d0d-a25e-0df207c269b8
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: ba468e80-d077-4af6-b782-238fc557e22b
translation-type: tm+mt
source-git-commit: ecd53a7d92dd020e6a3527793ff11efadcb531ee
workflow-type: tm+mt
source-wordcount: '2209'
ht-degree: 1%

---


# Manage Users, Groups, and User Roles {#manage-users-groups-and-user-roles}

管理员可以使用Adobe Admin Console创建AEM Assets品牌门户用户和产品用户档案，并使用品牌门户用户界面管理他们的角色。 此权限对查看者和编辑者不可用。

在Admin Console [[!UICONTROL 中]](http://adminconsole.adobe.com/enterprise/overview)，您可以视图与您的组织关联的所有产品。 产品可以是任何Experience Cloud解决方案，如Adobe Analytics、Adobe Target或AEM品牌门户。 您必须选择AEM Brand Portal产品，并创建产品用户档案。

<!--
Comment Type: draft

<note type="note">
<p>Product Profiles (formerly known as product configurations*). </p>
<p>* The nomenclature has changed from product configurations to product profiles in the new Adobe Admin Console.</p>
</note>
-->
![](assets/create-user-group.png)

这些产品用户档案每8小时与Brand Portal用户界面同步一次，在Brand Portal中以组的形式显示。 在添加用户和创建产品用户档案，以及将用户添加到这些产品用户档案后，您便可以在Brand Portal中为用户和用户组分配角色。

>[!NOTE]
>
>要在Brand Portal中创建组，请从Adobe [!UICONTROL Admin Console]，使 **[!UICONTROL 用“产品”>“产品用户档案]**”，而不 **[!UICONTROL 是“用户页面”>“用户组]**”。 Adobe用户档案中的产 [!UICONTROL 品Admin Console] ，用于在Brand Portal中创建组。

## 添加用户 {#add-a-user}

如果您是产品管理员，请使用Adobe [[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) ，创建用户并将其分配给产品用户档案(*以前称为产品配置*)，这些在Brand Portal中显示为组。 您可以使用组执行批量操作，如角色管理和资产共享。

>[!NOTE]
>
>无权访问Brand Portal的新用户可以从Brand Portal的登录屏幕请求访问权限。 有关详细信息，请参 [阅请求访问Brand Portal](../using/brand-portal.md#request-access-to-brand-portal)。 在通知区域中收到访问请求通知后，单击相关通知，然后单击“授予访 **[!UICONTROL 问权限”]**。 或者，也可以按照收到的访问请求电子邮件中的链接操作。 接下来，要通过Adobe [Admin Console [!UICONTROL 添加]](http://adminconsole.adobe.com/enterprise/overview)用户，请按照以下步骤4-7进行操作。

>[!NOTE]
>
>您可以直接或 [从 [!UICONTROL Brand]](http://adminconsole.adobe.com/enterprise/overview) Portal登录AdobeAdmin Console。 如果您直接登录，请按照以下步骤中的步骤4-7添加用户。

1. 从顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![AEM徽标](assets/aemlogo.png)

1. 在管理工具面板中，单击“ **[!UICONTROL 用户]**”。

   ![管理工具面板](assets/admin-tools-panel-5.png)

1. 在“用 [!UICONTROL 户角色] ”页中，单击“ **[!UICONTROL 管理]** ”选项卡，然后单 **[!UICONTROL 击“启动Admin Console]**”。

   ![要启动的用户角色Admin Console](assets/launch_admin_console.png)

1. 在Admin Console中，执行以下操作之一以创建新用户：

   * 在顶部的工具栏中，单击“ **[!UICONTROL 概述]**”。 在“概 [!UICONTROL 述] ”页面中，单 **[!UICONTROL 击Brand Portal产]** 品卡中的“分配用户”。

   ![Admin Console概述](assets/admin_console_overviewadduser.png)

   * 在顶部的工具栏中，单击“ **[!UICONTROL 用户]**”。 在“用 [!UICONTROL 户] ”页面 [!UICONTROL 中] ，默认情况下会选择左边栏中的“用户”。 单击“ **[!UICONTROL 添加用户]**”。

   ![Admin Console添加用户](assets/admin_console_adduseruserpage.png)

1. 在“添加用户”对话框中，键入要添加的用户的电子邮件ID，或从键入时显示的建议列表中选择该用户。

   ![将用户添加到Brand Portal](assets/add_user_to_aem_bp.png)

1. 将用户分配给至少一个产品用户档案（以前称为产品配置），以便用户可以访问Brand Portal。 从“请为此产品选择 **[!UICONTROL 用户档案”字段中选择相应的产品用户档案]** 。
1. 单击&#x200B;**[!UICONTROL 保存]**。将向您添加的用户发送一封欢迎电子邮件。 受邀用户可通过单击欢迎电子邮件中的链接并使用Adobe ID登录来访问品牌门 [!UICONTROL 户]。 有关详细信息，请 [参阅首次登录体验](../using/brand-portal-onboarding.md)。

   >[!NOTE]
   >
   >如果用户无法登录到Brand Portal，则组织的管理员应访问Adobe [!UICONTROL Admin Console] ，并检查用户是否存在以及是否已添加到至少一个产品用户档案。

   有关向用户授予管理权限的信息，请参 [阅向用户提供管理员权限](../using/brand-portal-adding-users.md#provideadministratorprivilegestousers)。

## 添加产品用户档案 {#add-a-product-profile}

用户档案中的产品Admin Console(以前称 [!UICONTROL 为] “产品配置”)用于在Brand Portal中创建组，以便您可以在Brand Portal中执行批量操作，如角色管理和资产共享。 **Brand Portal** 是提供的默认产品用户档案;您可以创建更多产品用户档案，并将用户添加到新产品用户档案。

>[!NOTE]
>
>您可以直接或 [[!UICONTROL 从Brand]](http://adminconsole.adobe.com/enterprise/overview) Portal登录Admin Console。 如果您直接登 [!UICONTROL 录Admin Console] ，请按照以下步骤4-7添加产品用户档案。

1. 从顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![AEM徽标](assets/aemlogo.png)

1. 在管理工具面板中，单击“ **[!UICONTROL 用户]**”。

   ![管理工具面板](assets/admin-tools-panel-6.png)

1. 在“用 [!UICONTROL 户角色] ”页中，单击“ **[!UICONTROL 管理]** ”选项卡，然后单 **[!UICONTROL 击“启动Admin Console]**”。

   ![启动Admin Console](assets/launch_admin_console.png)

1. 在顶部的工具栏中，单击 **[!UICONTROL 产品]**。
1. 在“产 [!UICONTROL 品] ”页面 [!UICONTROL 中] ，默认情况下选择“产品用户档案”。 单击 **[!UICONTROL 新建用户档案]**。

   ![添加新产品用户档案](assets/admin_console_addproductprofile.png)

1. 在“创 [!UICONTROL 建新用户档案] ”页面中，提供用户档案名称、显示名称、用户档案说明，并选择要在将用户添加到用户档案或从中删除时通过电子邮件通知用户。

   ![创建产品用户档案](assets/admin_console_addaproductprofilecreatenewprofile.png)

1. 单击&#x200B;**[!UICONTROL 完成]**。产品配置组(例如销 **[!UICONTROL 售组]**)将添加到Brand Portal。

   ![产品用户档案](assets/admin_console_productprofileadded.png)

## 将用户添加到产品用户档案 {#add-users-to-a-product-profile}

要将用户添加到Brand Portal组，请在Admin Console中将其添加到相应的产品用户档案(以前称为产品配 [!UICONTROL 置)]。 您可以单独或批量添加用户。

>[!NOTE]
>
>您可以直接或 [[!UICONTROL 从Brand]](http://adminconsole.adobe.com/enterprise/overview) Portal登录Admin Console。 如果您直接登录Admin Console，请按照以下步骤中的步骤4-7将用户添加到产品用户档案。

1. 从顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![AEM徽标](assets/aemlogo.png)

1. 在管理工具面板中，单击“ **[!UICONTROL 用户]**”。

   ![管理工具面板](assets/admin-tools-panel-7.png)

1. 在“用 [!UICONTROL 户角色] ”页中，单击“ **[!UICONTROL 管理]** ”选项卡，然后单 **[!UICONTROL 击“启动Admin Console]**”。

   ![启动 [!DNL Admin Console]](assets/launch_admin_console.png)

1. 在顶部的工具栏中，单击 **[!UICONTROL 产品]**。
1. 在“产 [!UICONTROL 品] ”页面 [!UICONTROL 中] ，默认情况下选择“产品用户档案”。 打开要向其添加用户的产品用户档案，例如销售 [!UICONTROL 组]。

   ![产品用户档案](assets/admin_console_productprofileadded.png)

1. 要向产品用户档案添加个人用户，请执行以下操作：

   * 单击“ **[!UICONTROL 添加用户]**”。

   ![要在Brand Portal中映射产品用户档案的组](assets/admin_console_productprofilesalesgroup.png)

   * 在“将 [!UICONTROL 用户添加到销售组] ”页中，键入要添加的用户的电子邮件ID，或从键入时显示的建议列表中选择该用户。

   ![将用户添加到组](assets/admin_console_addusertosalesgroup.png)

   * 单击&#x200B;**[!UICONTROL 保存]**。



1. 要将批量用户添加到产品用户档案，请执行以下操作：

   * 选 **[!UICONTROL 择省略号(...)>通过CSV添加用户]**。

   ![批量添加用户](assets/admin_console_addbulkusers.png)

   * 在“ **[!UICONTROL 通过CSV添加用户]** ”页面中，下载CSV模板或拖放CSV文件。

   ![通过csv添加用户](assets/admin_console_addbulkuserscsv.png)

   * Click **[!UICONTROL Upload]**.
   如果您将用户添加到默认的产品用户档案（即Brand Portal），则欢迎电子邮件会发送到您添加的用户的电子邮件ID。 受邀用户可以通过单击欢迎电子邮件中的链接并使用Adobe ID登录来访问品牌门 [!UICONTROL 户]。 有关详细信息，请 [参阅首次登录体验](../using/brand-portal-onboarding.md)。

   添加到自定义或新产品用户档案的用户不会收到电子邮件通知。

## 为用户提供管理员权限 {#provide-administrator-privileges-to-users}

您可以为Brand Portal用户提供系统管理员或产品管理员权限。 请勿提供Admin Console中可用的其 [!UICONTROL 他管理权]限，如产品用户档案管理员、用户组管理员和支持管理员。 要进一步了解这些角色，请参阅 [管理角色](https://helpx.adobe.com/enterprise/using/admin-roles.html)。

>[!NOTE]
>
>您可以直接或 [[!UICONTROL 从Brand]](https://adminconsole.adobe.com/enterprise/overview) Portal登录Admin Console。 如果您直接登 [!UICONTROL 录Admin Console] ，请按照以下步骤中的步骤4-8将用户添加到产品用户档案。

1. 从顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![AEMLogo](assets/aemlogo.png)

1. 在管理工具面板中，单击“ **[!UICONTROL 用户]**”。

   ![管理工具面板](assets/admin-tools-panel-8.png)

1. 在“用 [!UICONTROL 户角色] ”页中，单击“ **[!UICONTROL 管理]** ”选项卡，然后单 **[!UICONTROL 击“启动Admin Console]**”。

   ![启动Admin Console](assets/launch_admin_console.png)

1. 在顶部的工具栏中，单击“ **[!UICONTROL 用户]**”。
1. 在“用 [!UICONTROL 户] ”页面 [!UICONTROL 中] ，默认情况下会选择左边栏中的“用户”。 单击要向其提供管理员权限的用户的用户名。

   ![在Admin Console中添加用户](assets/admin_console_adduseruserpage.png)

1. 在用户用户档案页面中，找 **[!UICONTROL 到底部的]** “管理权限”部分，然后选择 **[!UICONTROL 省略号(...)>编辑管理权限]**。
   ![Admin Console中的管理权限](assets/admin_console_editadminrights.png)

1. 在“编 [!UICONTROL 辑管理员] ”页面中，选择“系统管理员”或“产品管理员”。

   ![在Admin Console中编辑管理权限](assets/admin_console_editadminrightsselection.png)

   >[!NOTE]
   >
   >Brand Portal仅支持系统管理员和产品管理员角色。
   >
   >Adobe建议您避免使用系统管理员角色，因为它授予组织内所有产品的管理员权限。 例如，某个组织（包括三个marketing cloud产品）的系统管理员对所有三个产品都具有整套权限。 只有系统管理员才能配置AEM Assets，以便将资产从AEM Assets发布到品牌门户。 For more information, see [Configure AEM Assets with Brand Portal](../using/configure-aem-assets-with-brand-portal.md).
   >
   >相反，产品管理员角色仅授予特定产品的管理员权限。 如果要在Brand Portal中强制实施更精细的访问控制，请使用“产品管理员”角色，然后选择产品作为Brand Portal。

   >[!NOTE]
   >
   >Brand Portal不支持产品用户档案管理员（以前称为配置管理员）权限。 避免为用户分配产品用户档案管理员权限。

1. 查看管理员类型选择，然后单 **[!UICONTROL 击保存]**。

   >[!NOTE]
   >
   >要撤销用户的管理员权限，请在“编辑管理员”页 **[!UICONTROL 面中进行相]** 应的更改，然后单 **[!UICONTROL 击保存]**。

## 管理用户角色 {#manage-user-roles}

管理员可以修改Brand Portal中用户的角色。

除了管理员角色之外，Brand Portal还支持以下角色：

* [!UICONTROL 查看器]:具有此角色的用户可以视图管理员与他们共享的文件和文件夹。 查看器还可以搜索和下载资产。 但是，查看器不能与其他用户共享内容(文件 [!UICONTROL 、文件夹]、集合)。
* [!UICONTROL 编辑]:具有此角色的用户具有查看器的所有权限。 此外，编辑人员还可以与其他用户共享内 [!UICONTROL 容]（文件夹、集合、链接）。

1. 从顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![AEMLogo](assets/aemlogo.png)

1. 在管理工具面板中，单击“ **[!UICONTROL 用户]**”。

   ![管理工具面板](assets/admin-tools-panel-9.png)

1. 在“用 [!UICONTROL 户角色] ”页中，默认 [!UICONTROL 情况下选] 择“用户”选项卡。 对于要更改其角色的用户，从“角 **[!UICONTROL 色]** ”下 **[!UICONTROL 拉菜单中选择]** “编辑 **[!UICONTROL 器]** ”或“查看器”。

   ![修改用户角色](assets/modify_user_role.png)

   要同时修改多个用户的角色，请选择这些用户，然后从“角色”下拉 **[!UICONTROL 菜单中选择]** 相应的角色。

   >[!NOTE]
   >
   >管理员 [!UICONTROL 用户的] “角色”列表被禁用。 您无法选择这些用户来修改其角色。

   >[!NOTE]
   >
   >如果用户是编辑者组的成员，则用户角色也会被禁用。 要撤销用户的编辑权限，请从编辑器组中删除该用户，或将整个组的角色更改为查看器。

1. 单击&#x200B;**[!UICONTROL 保存]**。将修改相应用户的角色。 如果选择了多个用户，则同时修改所有用户的角色。

   >[!NOTE]
   >
   >用户权限的更改仅在用 **[!UICONTROL 户重新登录]** Brand Portal后才会反映在“用户角色”页面中。

## 管理组角色和权限 {#manage-group-roles-and-privileges}

管理员可以将特定权限与品牌门 [户](../using/brand-portal-adding-users.md#main-pars-title-278567577) 上的一组用户关联。 “用 **[!UICONTROL 户角]** 色”页上的 **[!UICONTROL “组]** ”选项卡允许管理员：

* 为用户组分配角色
* 限制用户组从Brand Portal下载图像文件(.jpeg、.tiff、.png、.bmp、.gif、.pjpeg、x-portable-anymap、x-portable-bitmap、x-portable-graymap、x-portable-pixmap、x-rgbitmap、x-icon、image/x-photoshop、.psd、image/vnd.adobe.photoshop)的原始再现版本。

>[!NOTE]
>
>对于作为链接共享的资产，将根据共享资产的用户的权限，应用访问图像文件原始演绎版的权限。

要修改角色并有权访问特定用户组成员的原始演绎版，请执行以下步骤：

1. 在“用 **[!UICONTROL 户角色]** ”页上，导航到“ **[!UICONTROL 组]** ”选项卡。
1. 选择要更改其角色的组。
1. 从“角色”下拉 **[!UICONTROL 列表]** 中选择适当的角色。

   允许组成员访问图像文件的原始呈现形式(.jpeg、.tiff、.png、.bmp、.gif、.pjpeg、x-portable-anymap、x-portable-bitmap、x-portable-graymap、x-pixmap、x-rgb、x-xpixmap、x-icon、image/x-photoshop、.pshop、image/vnd.adobe.p)从门户或共享链接下载的“访 **[!UICONTROL 问原始]** ”选项。 默认情况下， **[!UICONTROL 会为所有用户]** 选择“访问原件”选项。 要阻止用户组访问原始演绎版，请取消选择与该组对应的选项。

   ![用户组角色](assets/access-original-rend.png)

   >[!NOTE]
   >
   >如果将用户添加到多个用户组，并且其中一个用户组具有限制，则限制将适用于该用户。
   >
   >此外，访问图像文件原始演绎版的限制不适用于管理员，即使管理员是受限组的成员。

1. 单击&#x200B;**[!UICONTROL 保存]**。将修改相应组的角色。

   >[!NOTE]
   >
   >用户与组的关联或用户的组成员关系每8小时同步一次到Brand Portal。 对用户或组角色的更改在下一个同步作业运行后生效。
