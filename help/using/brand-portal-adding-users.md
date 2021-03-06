---
title: 管理用户、组和用户角色
seo-title: Manage users, groups, and user roles
description: 管理员可以使用Adobe Admin Console创建Brand Portal用户和产品配置文件，并使用Brand Portal用户界面管理其角色。 此权限对查看器和编辑器不可用。
seo-description: Administrators can use Adobe Admin Console to create Brand Portal users and product profiles, and manage their roles using the Brand Portal user interface. This privilege is not available to Viewers and Editors.
uuid: 0dc1867c-6d1b-4d0d-a25e-0df207c269b8
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: ba468e80-d077-4af6-b782-238fc557e22b
role: Admin
exl-id: 35b1fd75-f9e4-4145-80bd-84de091f8b2b
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '2185'
ht-degree: 0%

---

# 管理用户、组和用户角色 {#manage-users-groups-and-user-roles}

管理员可以使用Adobe Admin Console创建Experience ManagerAssets Brand Portal用户和产品配置文件，并使用Brand Portal用户界面管理其角色。 此权限对查看器和编辑器不可用。

在[[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview)中，您可以查看与您的组织关联的所有产品。 产品可以是任何Experience Cloud解决方案，如Adobe Analytics、Adobe Target或Experience ManagerAssets Brand Portal。 您必须选择AEM Brand Portal产品并创建产品配置文件。

<!--
Comment Type: draft

<note type="note">
<p>Product Profiles (formerly known as product configurations*). </p>
<p>* The nomenclature has changed from product configurations to product profiles in the new Adobe Admin Console.</p>
</note>
-->
![](assets/create-user-group.png)

这些产品配置文件会每8小时与Brand Portal用户界面同步一次，并在Brand Portal中以组的形式显示。 添加用户和创建产品配置文件，并将用户添加到这些产品配置文件后，即可在Brand Portal中为用户和组分配角色。

>[!NOTE]
>
>要在Brand Portal中创建组，请从Adobe[!UICONTROL Admin Console]中，使用&#x200B;**[!UICONTROL 产品>产品配置文件]**，而不是&#x200B;**[!UICONTROL 用户页面>用户组]**。 Adobe[!UICONTROL Admin Console]中的产品配置文件用于在Brand Portal中创建组。

## 添加用户 {#add-a-user}

如果您是产品管理员，请使用Adobe[[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview)创建用户，并将其分配给在Brand Portal中显示为组的产品配置文件（*以前称为产品配置*）。 您可以使用组执行批量操作，如角色管理和资产共享。

>[!NOTE]
>
>无权访问Brand Portal的新用户可以从Brand Portal的登录屏幕请求访问权限。 有关更多信息，请参阅[请求访问Brand Portal](../using/brand-portal.md#request-access-to-brand-portal)。 在通知区域收到访问请求通知后，单击相关通知，然后单击&#x200B;**[!UICONTROL 授予访问权限]**。 或者，请按照收到的访问请求电子邮件中的链接进行操作。 接下来，要通过[Adobe[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview)添加用户，请按照以下过程中的步骤4-7操作。

>[!NOTE]
>
>您可以直接或从Brand Portal登录到[Adobe[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview)。 如果您直接登录，请按照以下步骤中的步骤4-7添加用户。

1. 在顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![AEM徽标](assets/aemlogo.png)

1. 在管理工具面板中，单击&#x200B;**[!UICONTROL 用户]**。

   ![“管理工具”面板](assets/admin-tools-panel-5.png)

1. 在[!UICONTROL 用户角色]页面中，单击&#x200B;**[!UICONTROL 管理]**&#x200B;选项卡，然后单击&#x200B;**[!UICONTROL 启动Admin Console]**。

   ![要启动的用户角色Admin Console](assets/launch_admin_console.png)

1. 在Admin Console中，执行以下操作之一以创建新用户：

   * 在顶部的工具栏中，单击&#x200B;**[!UICONTROL 概述]**。 在[!UICONTROL 概述]页面中，单击Brand Portal产品卡中的&#x200B;**[!UICONTROL 分配用户]** 。

   ![Admin Console概述](assets/admin_console_overviewadduser.png)

   * 在顶部的工具栏中，单击&#x200B;**[!UICONTROL 用户]**。 在[!UICONTROL Users]页面中，默认情况下会选择左边栏中的[!UICONTROL Users]。 单击&#x200B;**[!UICONTROL Add User]**。

   ![Admin Console添加用户](assets/admin_console_adduseruserpage.png)

1. 在“添加用户”对话框中，键入要添加的用户的电子邮件ID，或从键入时显示的建议列表中选择该用户。

   ![将用户添加到Brand Portal](assets/add_user_to_aem_bp.png)

1. 将用户至少分配一个产品配置文件（以前称为产品配置），以便用户可以访问Brand Portal。 从&#x200B;**[!UICONTROL Please select a profile for this product]**&#x200B;字段中选择相应的产品配置文件。
1. 单击&#x200B;**[!UICONTROL 保存]**。将向新添加的用户发送欢迎电子邮件。 受邀用户可以单击欢迎电子邮件中的链接以访问Brand Portal。 用户可以使用在Admin Console中配置的电子邮件ID([!UICONTROL Adobe ID]、[!UICONTROL Enterprise ID]或[!UICONTROL 已发送的ID])登录。 有关更多信息，请参阅[首次登录体验](../using/brand-portal-onboarding.md)。

   >[!NOTE]
   >
   >如果用户无法登录Brand Portal，则组织管理员应访问Adobe[!UICONTROL Admin Console]，并检查用户是否存在且已添加到至少一个产品配置文件中。

   有关向用户授予管理权限的信息，请参阅[向用户提供管理员权限](../using/brand-portal-adding-users.md#provideadministratorprivilegestousers)。

## 添加产品配置文件 {#add-a-product-profile}

[!UICONTROL Admin Console]中的产品配置文件（以前称为产品配置）用于在Brand Portal中创建组，以便您能够在Brand Portal中执行批量操作，如角色管理和资产共享。 **Brand Portalis** 提供默认的产品配置文件；您可以创建更多产品配置文件，并将用户添加到新的产品配置文件中。

>[!NOTE]
>
>您可以直接或从Brand Portal登录[[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview)。 如果您直接登录[!UICONTROL Admin Console]，请按照以下步骤中的步骤4-7添加产品配置文件。

1. 在顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![AEM徽标](assets/aemlogo.png)

1. 在管理工具面板中，单击&#x200B;**[!UICONTROL 用户]**。

   ![“管理工具”面板](assets/admin-tools-panel-6.png)

1. 在[!UICONTROL 用户角色]页面中，单击&#x200B;**[!UICONTROL 管理]**&#x200B;选项卡，然后单击&#x200B;**[!UICONTROL 启动Admin Console]**。

   ![启动Admin Console](assets/launch_admin_console.png)

1. 在顶部的工具栏中，单击&#x200B;**[!UICONTROL Products]**。
1. 在[!UICONTROL Products]页面中，默认情况下会选择[!UICONTROL Product Profiles]。 单击&#x200B;**[!UICONTROL 新建配置文件]**。

   ![添加新的产品配置文件](assets/admin_console_addproductprofile.png)

1. 在[!UICONTROL 创建新配置文件]页面中，提供配置文件名称、显示名称、配置文件描述，并选择要在添加到配置文件或从配置文件中删除用户时通过电子邮件通知用户。

   ![创建产品配置文件](assets/admin_console_addaproductprofilecreatenewprofile.png)

1. 单击&#x200B;**[!UICONTROL 完成]**。产品配置组（例如&#x200B;**[!UICONTROL Sales group]**）已添加到Brand Portal。

   ![产品配置文件](assets/admin_console_productprofileadded.png)

## 将用户添加到产品配置文件 {#add-users-to-a-product-profile}

要将用户添加到Brand Portal组，请将其添加到[!UICONTROL Admin Console]中的相应产品配置文件（以前称为产品配置）中。 您可以单独或批量添加用户。

>[!NOTE]
>
>您可以直接或从Brand Portal登录[[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview)。 如果您直接登录Admin Console，请按照以下步骤中的步骤4-7将用户添加到产品配置文件。

1. 在顶部的工具栏中，单击Experience Manager徽标以访问管理工具。

   ![AEM徽标](assets/aemlogo.png)

1. 在管理工具面板中，单击&#x200B;**[!UICONTROL 用户]**。

   ![“管理工具”面板](assets/admin-tools-panel-7.png)

1. 在[!UICONTROL 用户角色]页面中，单击&#x200B;**[!UICONTROL 管理]**&#x200B;选项卡，然后单击&#x200B;**[!UICONTROL 启动Admin Console]**。

   ![启动 [!DNL Admin Console]](assets/launch_admin_console.png)

1. 在顶部的工具栏中，单击&#x200B;**[!UICONTROL Products]**。
1. 在[!UICONTROL Products]页面中，默认情况下会选择[!UICONTROL Product Profiles]。 打开要向其添加用户的产品配置文件，例如[!UICONTROL Sales group]。

   ![产品配置文件](assets/admin_console_productprofileadded.png)

1. 要将个人用户添加到产品配置文件，请执行以下操作：

   * 单击&#x200B;**[!UICONTROL Add User]**。

   ![要在Brand Portal中映射产品配置文件的组](assets/admin_console_productprofilesalesgroup.png)

   * 在[!UICONTROL 将用户添加到销售组]页面中，键入要添加或从键入时显示的建议列表中选择用户的电子邮件ID。

   ![将用户添加到群组](assets/admin_console_addusertosalesgroup.png)

   * 单击&#x200B;**[!UICONTROL 保存]**。



1. 要将批量用户添加到产品配置文件，请执行以下操作：

   * 选择&#x200B;**[!UICONTROL 省略号(...)>通过CSV]**&#x200B;添加用户。

   ![批量添加用户](assets/admin_console_addbulkusers.png)

   * 在&#x200B;**[!UICONTROL 通过CSV添加用户]**&#x200B;页面中，下载CSV模板或拖放CSV文件。

   ![通过csv添加用户](assets/admin_console_addbulkuserscsv.png)

   * 单击&#x200B;**[!UICONTROL 上传]**。
   如果您将用户添加到默认的产品配置文件(即Brand Portal)，则会向您添加的用户的电子邮件ID发送一封欢迎电子邮件。 受邀用户可以通过单击欢迎电子邮件中的链接并使用[!UICONTROL Adobe ID]登录来访问Brand Portal。 有关更多信息，请参阅[首次登录体验](../using/brand-portal-onboarding.md)。

   添加到自定义或新产品配置文件的用户不会收到电子邮件通知。

## 向用户提供管理员权限 {#provide-administrator-privileges-to-users}

您可以向Brand Portal用户提供系统管理员或产品管理员权限。 请勿在[!UICONTROL Admin Console]中提供其他可用的管理权限，例如产品配置文件管理员、用户组管理员和支持管理员。 要了解这些角色的更多信息，请参阅[管理角色](https://helpx.adobe.com/enterprise/using/admin-roles.html)。

>[!NOTE]
>
>您可以直接或从Brand Portal登录[[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview)。 如果您直接登录[!UICONTROL Admin Console]，请按照以下过程中的步骤4-8将用户添加到产品配置文件。

1. 在顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![AEMLogo](assets/aemlogo.png)

1. 在管理工具面板中，单击&#x200B;**[!UICONTROL 用户]**。

   ![“管理工具”面板](assets/admin-tools-panel-8.png)

1. 在[!UICONTROL 用户角色]页面中，单击&#x200B;**[!UICONTROL 管理]**&#x200B;选项卡，然后单击&#x200B;**[!UICONTROL 启动Admin Console]**。

   ![启动Admin Console](assets/launch_admin_console.png)

1. 在顶部的工具栏中，单击&#x200B;**[!UICONTROL 用户]**。
1. 在[!UICONTROL Users]页面中，默认情况下会选择左边栏中的[!UICONTROL Users]。 单击要向其提供管理员权限的用户的用户名。

   ![在Admin Console中添加用户](assets/admin_console_adduseruserpage.png)

1. 在用户配置文件页面中，找到底部的&#x200B;**[!UICONTROL 管理权限]**&#x200B;部分，然后选择&#x200B;**[!UICONTROL 省略号(...)>编辑管理权限]**。
   ![Admin Console中的管理权限](assets/admin_console_editadminrights.png)

1. 在[!UICONTROL 编辑管理员]页面中，选择系统管理员或产品管理员。

   ![在Admin Console中编辑管理权限](assets/admin_console_editadminrightsselection.png)

   >[!NOTE]
   >
   >Brand Portal仅支持“系统管理员”和“产品管理员”角色。
   >
   >Adobe建议您避免使用系统管理员角色，因为它授予组织内所有产品的管理员权限。 例如，某个组织（包含三个Marketing Cloud产品）的系统管理员拥有所有三个产品的全部权限集。 只有系统管理员才能配置Experience Manager资产，以便将资产从Experience Manager资产发布到Brand Portal。 有关更多信息，请参阅[使用Brand Portal配置Experience Manager资产](../using/configure-aem-assets-with-brand-portal.md)。
   >
   >相反，产品管理员角色仅授予特定产品的管理员权限。 如果要在Brand Portal中强制实施更精细的访问控制，请使用产品管理员角色并选择产品作为Brand Portal。

   >[!NOTE]
   >
   >Brand Portal不支持产品配置文件管理员（以前称为配置管理员）权限。 避免向用户分配产品配置文件管理员权限。

1. 查看管理员类型选择并单击&#x200B;**[!UICONTROL 保存]**。

   >[!NOTE]
   >
   >要撤销用户的管理员权限，请在&#x200B;**[!UICONTROL 编辑管理员]**&#x200B;页面中进行相应更改，然后单击&#x200B;**[!UICONTROL 保存]**。


## 管理用户角色 {#manage-user-roles}

管理员可以在Brand Portal中修改用户的角色。

除了管理员角色之外，Brand Portal还支持以下角色：

* [!UICONTROL 查看器]:具有此角色的用户可以查看管理员与他们共享的文件和文件夹。查看者还可以搜索和下载资产。 但是，查看器无法与其他用户共享内容（文件、文件夹、[!UICONTROL 收藏集]）。
* [!UICONTROL 编辑者]:具有此角色的用户拥有查看器的所有权限。此外，编辑者还可以与其他用户共享内容（文件夹、[!UICONTROL 集合]、链接）。

1. 在顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![AEMLogo](assets/aemlogo.png)

1. 在管理工具面板中，单击&#x200B;**[!UICONTROL 用户]**。

   ![“管理工具”面板](assets/admin-tools-panel-9.png)

1. 在[!UICONTROL 用户角色]页面中，默认情况下会选择[!UICONTROL 用户]选项卡。 对于要更改其角色的用户，从&#x200B;**[!UICONTROL 角色]**&#x200B;下拉列表中选择&#x200B;**[!UICONTROL Editor]**&#x200B;或&#x200B;**[!UICONTROL Viewer]**。

   ![修改用户角色](assets/modify_user_role.png)

   要同时修改多个用户的角色，请选择这些用户，然后从&#x200B;**[!UICONTROL 角色]**&#x200B;下拉列表中选择相应的角色。

   >[!NOTE]
   >
   >管理员用户的[!UICONTROL 角色]列表处于禁用状态。 您无法选择这些用户来修改其角色。


   >[!NOTE]
   >
   >如果用户是编辑者组的成员，则也会禁用用户角色。 要撤消用户的编辑权限，请从编辑器组中删除该用户，或将整个组的角色更改为查看器。


1. 单击&#x200B;**[!UICONTROL 保存]**。将为相应用户修改角色。 如果您选择了多个用户，则所有用户的角色都会同时修改。

   >[!NOTE]
   >
   >用户权限的更改仅在用户重新登录Brand Portal后才会反映在&#x200B;**[!UICONTROL User Roles]**&#x200B;页面中。

## 管理组角色和权限 {#manage-group-roles-and-privileges}

管理员可以将特定权限与Brand Portal上[组](../using/brand-portal-adding-users.md#main-pars-title-278567577)的用户相关联。 **[!UICONTROL 用户角色]**&#x200B;页面上的&#x200B;**[!UICONTROL 组]**&#x200B;选项卡允许管理员：

* 为用户组分配角色
* 限制用户组从Brand Portal下载图像文件的原始呈现版本(.jpeg、.tiff、.png、.bmp、.gif、.pjpeg、x-portable-anymap、x-portable-bitmap、x-portable-graymap、x-pixmap、x-rgb、x-xpixmap、x-icon、image/photoshop、image/x-photoshop、.psd、image/vnd.adobe.photoshop)。

>[!NOTE]
>
>对于作为链接共享的资产，根据共享资产的用户权限，将应用访问图像文件原始演绎版的权限。

要修改特定组成员的角色和访问原始呈现的权限，请执行以下步骤：

1. 在&#x200B;**[!UICONTROL 用户角色]**&#x200B;页面上，导航到&#x200B;**[!UICONTROL 组]**&#x200B;选项卡。
1. 选择要更改其角色的组。
1. 从&#x200B;**[!UICONTROL 角色]**&#x200B;下拉列表中选择相应的角色。

   要允许组成员访问图像文件(.jpeg、.tiff、.png、.bmp、.gif、.pjpeg、x-portable-anymap、x-portable-bitmap、x-portable-graymap、x-portable-pixmap、x-rgb、x-xbitmap、x-xpixmap、x-icon、image/photoshop、image/x-photoshop、.psd、image/vnd.adobe.photoshop)的原始呈现版本，请保留为该组选择的&#x200B;**[!UICONTROL 访问原始]**&#x200B;选项。 默认情况下，为所有用户选择了&#x200B;**[!UICONTROL 访问原始]**&#x200B;选项。 要阻止用户组访问原始演绎版，请取消选择与该组对应的选项。

   ![用户组角色](assets/access-original-rend.png)

   >[!NOTE]
   >
   >如果将一个用户添加到多个组，并且其中一个组具有限制，则该限制将适用于该用户。
   >
   >此外，访问图像文件原始呈现版本的限制不适用于管理员，即使他们是受限组的成员。


1. 单击&#x200B;**[!UICONTROL 保存]**。将为相应的组修改角色。

   >[!NOTE]
   >
   >用户到群组关联或用户的群组成员资格每8小时会同步一次到Brand Portal。 对用户或组角色的更改在下次同步作业运行后生效。
