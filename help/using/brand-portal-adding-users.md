---
title: 管理用户、组和用户角色
seo-title: Manage users, groups, and user roles
description: 管理员可以使用Adobe Admin Console创建Brand Portal用户和产品配置文件，并使用Brand Portal用户界面管理其角色。 查看者和编辑者无法使用此权限。
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

管理员可以使用Adobe Admin Console创建Experience Manager Assets Brand Portal用户和产品配置文件，并使用Brand Portal用户界面管理其角色。 查看者和编辑者无法使用此权限。

In [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview)，您可以查看与您的组织关联的所有产品。 产品可以是任何Experience Cloud解决方案，例如Adobe Analytics、Adobe Target或Experience Manager Assets Brand Portal。 您必须选择AEM Brand Portal产品，并创建产品配置文件。

<!--
Comment Type: draft

<note type="note">
<p>Product Profiles (formerly known as product configurations*). </p>
<p>* The nomenclature has changed from product configurations to product profiles in the new Adobe Admin Console.</p>
</note>
-->
![](assets/create-user-group.png)

这些产品配置文件每8小时与Brand Portal用户界面同步一次，并在Brand Portal中作为组显示。 添加用户和创建产品配置文件，并将用户添加到这些产品配置文件后，您可以在Brand Portal中为用户和组分配角色。

>[!NOTE]
>
>要在Brand Portal中创建组，请从Adobe [!UICONTROL Admin Console]，使用 **[!UICONTROL 产品>产品配置文件]**，而不是 **[!UICONTROL “用户”页>“用户组”]**. Adobe中的产品配置文件 [!UICONTROL Admin Console] 用于在Brand Portal中创建组。

## 添加用户 {#add-a-user}

如果您是产品管理员，请使用Adobe [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) 要创建用户并将其分配给产品配置文件(*以前称为产品配置*)，在Brand Portal中显示为组。 您可以使用组执行批量操作，如角色管理和资产共享。

>[!NOTE]
>
>无权访问Brand Portal的新用户可以从Brand Portal的登录屏幕请求访问权限。 有关更多信息，请参阅 [请求访问Brand Portal](../using/brand-portal.md#request-access-to-brand-portal). 在通知区域收到访问请求通知后，单击相关通知，然后单击 **[!UICONTROL 授予访问权限]**. 或者，按照收到的访问请求电子邮件中的链接操作。 接下来，通过添加用户 [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview)，请按照以下过程中的步骤4 - 7执行操作。

>[!NOTE]
>
>您可以登录到 [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) 直接访问或从Brand Portal访问。 如果直接登录，请按照以下过程中的步骤4-7添加用户。

1. 从顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![AEM徽标](assets/aemlogo.png)

1. 在管理工具面板中，单击 **[!UICONTROL 用户]**.

   ![“管理工具”面板](assets/admin-tools-panel-5.png)

1. 在 [!UICONTROL 用户角色] 页面上，单击 **[!UICONTROL 管理]** 选项卡，然后单击 **[!UICONTROL 启动Admin Console]**.

   ![要启动Admin Console的用户角色](assets/launch_admin_console.png)

1. 在Admin Console中，执行以下操作之一以创建新用户：

   * 在顶部的工具栏中，单击 **[!UICONTROL 概述]**. 在 [!UICONTROL 概述] 页面，单击 **[!UICONTROL 分配用户]** 从Brand Portal产品信息卡中获取。

   ![Admin Console概述](assets/admin_console_overviewadduser.png)

   * 在顶部的工具栏中，单击 **[!UICONTROL 用户]**. 在 [!UICONTROL 用户] 页面， [!UICONTROL 用户] 默认选中左边栏中的。 单击 **[!UICONTROL 添加用户]**.

   ![Admin Console添加用户](assets/admin_console_adduseruserpage.png)

1. 在“添加用户”对话框中，键入要添加的用户的电子邮件ID，或从键入时显示的建议列表中选择该用户。

   ![将用户添加到Brand Portal](assets/add_user_to_aem_bp.png)

1. 将用户分配给至少一个产品配置文件（以前称为产品配置），以便用户可以访问Brand Portal。 从中选择相应的产品配置文件 **[!UICONTROL 请选择此产品的配置文件]** 字段。
1. 单击“**[!UICONTROL 保存]**”。将向新添加的用户发送欢迎电子邮件。 受邀用户可单击欢迎电子邮件中的链接以访问Brand Portal。 用户可以使用电子邮件ID登录([!UICONTROL Adobe ID]， [!UICONTROL Enterprise ID]，或 [!UICONTROL 已提交的ID])在Admin Console中配置。 有关更多信息，请参阅 [首次登录体验](../using/brand-portal-onboarding.md).

   >[!NOTE]
   >
   >如果用户无法登录Brand Portal，则组织的管理员应访问Adobe [!UICONTROL Admin Console] 和检查用户是否存在并已添加到至少一个产品配置文件。

   有关授予用户管理权限的信息，请参见 [向用户提供管理员权限](../using/brand-portal-adding-users.md#provideadministratorprivilegestousers).

## 添加产品配置文件 {#add-a-product-profile}

中的产品配置文件（以前称为产品配置） [!UICONTROL Admin Console] 用于在Brand Portal中创建组，以便您能够执行批量操作，例如Brand Portal中的角色管理和资产共享。 **Brand Portal** 是默认可用的产品配置文件；您可以创建更多产品配置文件并将用户添加到新的产品配置文件。

>[!NOTE]
>
>您可以登录到 [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) 直接访问或从Brand Portal访问。 如果您登录到 [!UICONTROL Admin Console] 直接按照以下步骤中的步骤4-7添加产品配置文件。

1. 从顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![AEM徽标](assets/aemlogo.png)

1. 在管理工具面板中，单击 **[!UICONTROL 用户]**.

   ![“管理工具”面板](assets/admin-tools-panel-6.png)

1. 在 [!UICONTROL 用户角色] 页面上，单击 **[!UICONTROL 管理]** 选项卡，然后单击 **[!UICONTROL 启动Admin Console]**.

   ![启动Admin Console](assets/launch_admin_console.png)

1. 在顶部的工具栏中，单击 **[!UICONTROL 产品]**.
1. 在 [!UICONTROL 产品] 页面， [!UICONTROL 产品配置文件] 默认情况下处于选中状态。 单击 **[!UICONTROL 新建配置文件]**.

   ![添加新产品配置文件](assets/admin_console_addproductprofile.png)

1. 在 [!UICONTROL 创建新配置文件] 页面中，提供配置文件名称、显示名称和配置文件描述，并选择在用户添加到配置文件中或从配置文件中删除用户时，是否要通过电子邮件通知用户。

   ![创建产品配置文件](assets/admin_console_addaproductprofilecreatenewprofile.png)

1. 单击 **[!UICONTROL 完成]**. 产品配置组，例如 **[!UICONTROL 销售组]**，则会添加到Brand Portal中。

   ![产品配置文件](assets/admin_console_productprofileadded.png)

## 将用户添加到产品配置文件 {#add-users-to-a-product-profile}

要将用户添加到Brand Portal组，请将其添加到中相应的产品配置文件（以前称为产品配置） [!UICONTROL Admin Console]. 您可以单独或批量添加用户。

>[!NOTE]
>
>您可以登录到 [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) 直接访问或从Brand Portal访问。 如果您直接登录Admin Console，请按照以下过程中的步骤4-7将用户添加到产品配置文件。

1. 在顶部的工具栏中，单击Experience Manager徽标以访问管理工具。

   ![AEM徽标](assets/aemlogo.png)

1. 在管理工具面板中，单击 **[!UICONTROL 用户]**.

   ![“管理工具”面板](assets/admin-tools-panel-7.png)

1. 在 [!UICONTROL 用户角色] 页面上，单击 **[!UICONTROL 管理]** 选项卡，然后单击 **[!UICONTROL 启动Admin Console]**.

   ![启动 [!DNL Admin Console]](assets/launch_admin_console.png)

1. 在顶部的工具栏中，单击 **[!UICONTROL 产品]**.
1. 在 [!UICONTROL 产品] 页面， [!UICONTROL 产品配置文件] 默认情况下处于选中状态。 打开要添加用户的产品配置文件，例如， [!UICONTROL 销售组].

   ![产品配置文件](assets/admin_console_productprofileadded.png)

1. 要将个人用户添加到产品配置文件，请执行以下操作：

   * 单击 **[!UICONTROL 添加用户]**.

   ![要在Brand Portal中映射产品配置文件的组](assets/admin_console_productprofilesalesgroup.png)

   * 在 [!UICONTROL 将用户添加到销售组] 页面上，键入要添加的用户的电子邮件ID，或从键入时显示的建议列表中选择该用户。

   ![将用户添加到组](assets/admin_console_addusertosalesgroup.png)

   * 单击“**[!UICONTROL 保存]**”。



1. 要将批量用户添加到产品配置文件，请执行以下操作：

   * 选择 **[!UICONTROL 省略号(...) >通过CSV添加用户]**.

   ![批量添加用户](assets/admin_console_addbulkusers.png)

   * 在 **[!UICONTROL 通过CSV添加用户]** 页面，下载CSV模板或拖放CSV文件。

   ![通过csv添加用户](assets/admin_console_addbulkuserscsv.png)

   * 单击 **[!UICONTROL 上传]**.
   如果您将用户添加到默认产品配置文件(即Brand Portal)，则会向您添加用户的电子邮件ID发送欢迎电子邮件。 受邀用户可以通过单击欢迎电子邮件中的链接并使用登录来访问Brand Portal [!UICONTROL Adobe ID]. 有关更多信息，请参阅 [首次登录体验](../using/brand-portal-onboarding.md).

   添加到自定义或新产品配置文件的用户不会收到电子邮件通知。

## 向用户提供管理员权限 {#provide-administrator-privileges-to-users}

您可以向Brand Portal用户提供系统管理员或产品管理员权限。 不提供中可用的其他管理权限 [!UICONTROL Admin Console]，如产品配置文件管理员、用户组管理员和支持管理员。 要了解有关这些角色的更多信息，请参阅 [管理角色](https://helpx.adobe.com/enterprise/using/admin-roles.html).

>[!NOTE]
>
>您可以登录到 [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) 直接访问或从Brand Portal访问。 如果您登录到 [!UICONTROL Admin Console] 直接按照以下过程中的步骤4-8将用户添加到产品配置文件。

1. 从顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![AEMLogo](assets/aemlogo.png)

1. 在管理工具面板中，单击 **[!UICONTROL 用户]**.

   ![“管理工具”面板](assets/admin-tools-panel-8.png)

1. 在 [!UICONTROL 用户角色] 页面上，单击 **[!UICONTROL 管理]** 选项卡，然后单击 **[!UICONTROL 启动Admin Console]**.

   ![启动Admin Console](assets/launch_admin_console.png)

1. 在顶部的工具栏中，单击 **[!UICONTROL 用户]**.
1. 在 [!UICONTROL 用户] 页面， [!UICONTROL 用户] 默认选中左边栏中的。 单击要向其提供管理员权限的用户的用户名。

   ![在Admin Console中添加用户](assets/admin_console_adduseruserpage.png)

1. 在用户配置文件页面中，找到 **[!UICONTROL 管理权限]** 部分，然后选择 **[!UICONTROL 省略号(...) >编辑管理权限]**.
   ![Admin Console中的管理员权限](assets/admin_console_editadminrights.png)

1. 在 [!UICONTROL 编辑管理员] 页面上，选择“系统管理员”或“产品管理员”。

   ![在Admin Console中编辑管理员权限](assets/admin_console_editadminrightsselection.png)

   >[!NOTE]
   >
   >Brand Portal仅支持系统管理员和产品管理员角色。
   >
   >Adobe建议您避免使用系统管理员角色，因为它授予组织范围管理员权限，以便管理组织的所有产品。 例如，包含三种Marketing Cloud产品的组织的系统管理员拥有所有三种产品的完整权限集。 只有系统管理员才能配置Experience Manager Assets，以便将资源从Experience Manager Assets发布到Brand Portal。 有关更多信息，请参阅 [使用Brand Portal配置Experience Manager Assets](../using/configure-aem-assets-with-brand-portal.md).
   >
   >相反，“产品管理员”角色仅授予特定产品的管理员权限。 如果要在Brand Portal中实施更细粒度的访问控制，请使用产品管理员角色并选择产品作为Brand Portal。

   >[!NOTE]
   >
   >Brand Portal不支持产品配置文件管理员（以前称为配置管理员）权限。 避免为用户分配产品配置文件管理员权限。

1. 查看管理员类型选择并单击 **[!UICONTROL 保存]**.

   >[!NOTE]
   >
   >要撤销用户的管理员权限，请在 **[!UICONTROL 编辑管理员]** 页面，然后单击 **[!UICONTROL 保存]**.


## 管理用户角色 {#manage-user-roles}

管理员可以在Brand Portal中修改用户的角色。

除了管理员角色之外，Brand Portal还支持以下角色：

* [!UICONTROL 查看器]：具有此角色的用户可以查看管理员与他们共享的文件和文件夹。 查看者还可以搜索和下载资产。 但是，查看器不能共享内容(文件、文件夹、 [!UICONTROL 收藏集])。
* [!UICONTROL 编辑者]：具有此角色的用户拥有查看器的所有权限。 此外，编辑人员可以共享内容(文件夹、 [!UICONTROL 收藏集]，链接)。

1. 从顶部的AEM工具栏中，单击Adobe徽标以访问管理工具。

   ![AEMLogo](assets/aemlogo.png)

1. 在管理工具面板中，单击 **[!UICONTROL 用户]**.

   ![“管理工具”面板](assets/admin-tools-panel-9.png)

1. 在 [!UICONTROL 用户角色] 页面， [!UICONTROL 用户] 选项卡默认处于选中状态。 对于要更改其角色的用户，选择 **[!UICONTROL 编辑者]** 或 **[!UICONTROL 查看器]** 从 **[!UICONTROL 角色]** 下拉菜单。

   ![修改用户角色](assets/modify_user_role.png)

   要同时修改多个用户的角色，请选择用户，然后从中选择适当的角色 **[!UICONTROL 角色]** 下拉菜单。

   >[!NOTE]
   >
   >此 [!UICONTROL 角色] 管理员用户列表已禁用。 不能选择这些用户来修改其角色。


   >[!NOTE]
   >
   >如果用户是编辑者组的成员，则用户角色也会被禁用。 要从用户撤销编辑权限，请从“编辑者”组中删除用户，或将整个组的角色更改为“查看器”。


1. 单击“**[!UICONTROL 保存]**”。相应用户的角色已修改。 如果选择多个用户，则所有用户的角色将同时修改。

   >[!NOTE]
   >
   >用户权限更改会反映在 **[!UICONTROL 用户角色]** 仅在用户重新登录Brand Portal后创建页面。

## 管理组角色和权限 {#manage-group-roles-and-privileges}

管理员可以将特定权限与 [群组](../using/brand-portal-adding-users.md#main-pars-title-278567577) 用户在Brand Portal上的注册表。 此 **[!UICONTROL 组]** 选项卡 **[!UICONTROL 用户角色]** 页面允许管理员：

* 为用户组分配角色
* 限制用户组从Brand Portal下载图像文件的原始演绎版(.jpeg、.tiff、.png、.bmp、.gif、.pjpeg、 x-portable-anymap、 x-portable-bitmap、 x-portable-graymap、 x-rgb、 x-xbitmap、 x-xpixmap、 x-icon、image/photoshop、image/x-photoshop、.psd、image/vnd.adobe.photoshop)。

>[!NOTE]
>
>对于作为链接共享的资产，将根据共享资产的用户的权限，应用对图像文件原始演绎版的访问权限。

要修改角色和访问特定组成员原始演绎版的权利，请执行以下步骤：

1. 在 **[!UICONTROL 用户角色]** 页面，导航到 **[!UICONTROL 组]** 选项卡。
1. 选择要为其更改角色的组。
1. 从中选择适当的角色 **[!UICONTROL 角色]** 下拉列表。

   要允许组的成员访问他们从门户或共享链接下载的图像文件(.jpeg、.tiff、.png、.bmp、.gif、.pjpeg、 x-portable-anymap、 x-portable-bitmap、 x-portable-graymap、 x-rgb、 x-xbitmap、 x-xpixmap、 x-icon、 image/photoshop、.psd、.image/vnd.adobe.photoshop)的原始演绎版，请保留 **[!UICONTROL 对原始内容的访问权限]** 已为该组选择选项。 默认情况下， **[!UICONTROL 对原始内容的访问权限]** 选项。 要阻止用户组访问原始演绎版，请取消选择与该组对应的选项。

   ![用户组角色](assets/access-original-rend.png)

   >[!NOTE]
   >
   >如果将一个用户添加到多个组，并且其中一个组具有限制，则该限制将适用于该用户。
   >
   >此外，对访问图像文件原始演绎版的限制不适用于管理员，即使他们属于受限组。


1. 单击“**[!UICONTROL 保存]**”。相应组的角色已修改。

   >[!NOTE]
   >
   >用户到组的关联，即用户的组成员资格，每8小时同步到Brand Portal一次。 对用户或组角色的更改将在下次同步作业运行后生效。
