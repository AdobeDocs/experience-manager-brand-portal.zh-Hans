---
title: AEM Assets品牌门户概述
seo-title: AEM Assets品牌门户概述
description: AEM Assets Brand Portal可帮助您在各种设备上轻松获取、控制和安全地分发经过审批的创意资源，并将其分发给外部的合作伙伴和内部业务用户。
seo-description: AEM Assets Brand Portal可帮助您在各种设备上轻松获取、控制和安全地分发经过审批的创意资源，并将其分发给外部的合作伙伴和内部业务用户。
uuid: b1e54d03-eb2 e-488e-af4 d-bae817 dd135 a
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Brand_ Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85 b-e419 ee37 f2 f4
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# AEM Assets品牌门户概述 {#overview-of-aem-assets-brand-portal}

作为营销人员，您有时需要与渠道合作伙伴和内部业务用户协作，以便快速创建、管理和向客户提供相关的数字内容。在整个客户旅程中及时交付相关内容对于提高需求、转化率、参与度和客户忠诚度至关重要。

但是，开发支持有效和安全地共享已批准品牌徽标、准则、系列活动资源或产品照片(与扩展的内部团队、合作伙伴和经销商)的解决方案是一个挑战。

**Adobe Experience Manager(AEM) Assets Brand Portal** 可帮助您在各种设备上轻松获取、控制和安全地分发经过批准的创意资产，并将其分发给外部的合作伙伴和内部业务用户。它有助于提高资产共享的效率，加快资产的上市时间，并降低不合规和未授权访问的风险。

基于浏览器的门户环境使您能够以批准的格式轻松上传、浏览、搜索、预览和导出资产。

## Brand Portal中的用户角色 {#Personas}

Brand Portal支持以下用户角色：

* 客人用户
* 查看者
* 编辑者
* 管理员

下表列出了这些角色中用户可以执行的任务：

|  | **浏览** | **搜索** | **下载** | **共享文件夹** | **共享集合** | **将资产共享为链接** | **访问管理工具** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **客人用户** | ✓* | ✓* | ✓* | x | x | x | x |
| **查看者** | ✓ | ✓ | ✓ | x | x | x | x |
| **编辑者** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **管理员** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

*客人用户只能在公共文件夹和集合中浏览、访问和搜索资产。

### Guest user {#guest-user}

在Brand Portal上对资产拥有有限访问权限的任何用户都是客人用户。客人会话允许用户访问公共文件夹和集合。作为客人用户，您可以浏览资产详细信息，并具有公共文件夹和集合成员的完整资产视图。您可以搜索、下载公共资产并将其添加到 [!UICONTROL Lightbox] 集合。

但是，客人会话限制您创建集合和保存的搜索，并进一步共享。客人会话中的用户无法访问文件夹和集合设置，也无法将资源共享为链接。下面列出了客人用户可以执行的任务：

[浏览和访问公共资产](browse-assets-brand-portal.md)

[搜索公共资产](brand-portal-searching.md)

[下载公共资源](brand-portal-download-users.md)

[将资产添加到[！UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

### 查看者 {#viewer}

Brand Portal中的标准用户通常是具有查看器角色的用户。具有此角色的用户可以访问允许的文件夹、集合和资产。用户还可以浏览、预览、下载和导出资产(原始或特定演绎版)、配置帐户设置和搜索资产。下面列出了查看器可以执行的任务：

[浏览资产](browse-assets-brand-portal.md)

[搜索资产](brand-portal-searching.md)

[下载资源](brand-portal-download-users.md)

### 编辑者 {#editor}

具有编辑器角色的用户可以执行查看器可以执行的所有任务。此外，编辑器还可以查看管理员共享的文件和文件夹。具有编辑者角色的用户还可以与其他人共享内容(文件、文件夹、集合)。

除了查看器可以执行的任务之外，编辑者还可以执行以下其他任务：

[共享文件夹](brand-portal-sharing-folders.md)

[共享集合](brand-portal-share-collection.md)

[将资产共享为链接](brand-portal-link-share.md)

### 管理员 {#administrator}

管理员在 [!UICONTROL Admin Console]中包括被标记为系统管理员或Brand Portal产品管理员的用户。管理员可以添加和删除系统管理员和用户、定义预设、向用户发送电子邮件以及查看门户使用情况和存储报告。

管理员可以执行编辑可以执行以下其他任务的所有任务：

[管理用户、组和用户角色](brand-portal-adding-users.md)

[自定义墙纸、页眉和电子邮件](brand-portal-branding.md)

[使用自定义搜索彩块化](brand-portal-search-facets.md)

[使用元数据架构表单](brand-portal-metadata-schemas.md)

[应用图像预设或动态演绎版](brand-portal-image-presets.md)

[使用报告](brand-portal-reports.md)

除了上述任务之外，AEM资产中的作者还可以执行以下任务：

[配置AEM Assets与Brand Portal的集成](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html)

[将文件夹发布到Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-folder.html)

[将集合发布到Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-collection.html)

## Brand Portal url的替代别名 {#tenant-alias-for-portal-url}

从Brand Portal6.4.3开始，组织可以为其Brand Portal租户的现有URL具有一个替代(别名) URL。可以通过在URL中具有替代前缀来创建别名URL。\
请注意，只能自定义Brand Portal URL的前缀，而不能是整个URL。例如，具有现有域 **[!UICONTROL geomettrix.brand-portal.adobe.com]** 的组织可以获取 **[!UICONTROL 根据请求创建的geomettrixinc.brand-portal.adobe.com]** 。

但是，AEM作者实例只能通过租户id URL [进行配置](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) ，而不能使用租户别名(替代) URL进行配置。

>[!NOTE]
>
>要在现有门户URL中获取租户名称别名，组织需要与新的租户别名创建请求联系Adobe支持。通过首先检查别名是否可用，然后创建别名来处理此请求。
>
>要替换旧别名或删除旧别名，需要遵循相同的进程。

## 请求访问Brand Portal {#request-access-to-brand-portal}

用户可以从登录屏幕请求访问Brand Portal。这些请求会发送给Brand Portal管理员，他们通过Adobe [!UICONTROL Admin Console授予用户访问权限]。授予访问权限后，用户收到通知电子邮件。

要请求访问，请执行以下操作：

1. 从Brand Portal登录页面中，选择 **[!UICONTROL “单击此处]** 对应 **[!UICONTROL 是否需要访问”？]**. 但是，要进入客人会话，请选择与 ******[!UICONTROL 客人访问对应的单击此处]**。

   ![Brand Portal登录屏幕](assets/bp-login-requestaccess.png)

   [!UICONTROL 此时将打开请求访问] 页面。

2. 要请求访问组织的Brand Portal，您必须具有有效 [!UICONTROL 的Adobe ID]、 [!UICONTROL Enterprise ID]或 [!UICONTROL Federated ID]。

   在 [!UICONTROL 请求访问] 页面中，使用您的ID(场景1)登录或创建Adobe [!UICONTROL ID] (场景2)：
   ![[!UICONTROL 请求访问]](assets/bplogin_request_access_2.png)

   **场景1**
   1. 如果您有 [!UICONTROL Adobe ID]、 [!UICONTROL Enterprise ID]或 [!UICONTROL Federated ID]，请单击“ **[!UICONTROL 登录]**”。
[!UICONTROL 此时将打开“登录”] 页面。
   2. 提供您 [!UICONTROL 的Adobe ID] 凭据，然后单击 **[!UICONTROL 登录]**。
      ![Adobe登录](assets/bplogin_request_access_3.png)
   您将重定向到 [!UICONTROL 请求访问] 页面。
   **场景2**
   1. 如果您没有 [!UICONTROL Adobe ID]，要创建一个Adobe ID，请单击 ****[!UICONTROL “请求访问”] 页面中的“获取Adobe ID”。
[!UICONTROL 此时将打开“登录”] 页面。
   2. Click **[!UICONTROL Get an Adobe ID]**.
此时将打开 [!UICONTROL 注册] 页面。
   3. 输入您的名字、姓氏、电子邮件ID和密码。
   4. 选择 **[!UICONTROL 注册]**。
      ![](assets/bplogin_request_access_5.png)
   您将重定向到 [!UICONTROL 请求访问] 页面。

3. 下一页显示用于请求访问权限的姓名和电子邮件ID。为管理员留下评论，然后单击 **[!UICONTROL “提交]**”。

   ![](assets/bplogin-request-access.png)

## 产品管理员授予访问权限 {#grant-access-to-brand-portal}

Brand Portal产品管理员在其Brand Portal通知区域中和其收件箱中通过电子邮件接收访问请求。

![访问请求的通知](assets/bplogin_request_access_7.png)

要授予访问权限，产品管理员需要单击Brand Portal通知区域中的相关通知，然后单击 **[!UICONTROL “授权访问]**”。
或者，产品管理员可以遵循访问请求电子邮件中提供的链接访问Adobe [!UICONTROL Admin Console] ，并将用户添加到相关产品配置。![](assets/bplogin_request_access_8.png)


您被重定向到Adobe [[！UICCONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) 主页。使用Adobe [!UICONTROL Admin Console] 创建用户并将其分配到产品配置(以前称为产品配置)，该配置在Brand Portal中显示为组。有关在 [!UICONTROL Admin Console]中添加用户的详细信息，请参阅 [添加用户](brand-portal-adding-users.md#add-a-user) (按照步骤中的步骤4-7添加用户)。

## Brand Portal维护通知 {#brand-portal-maintenance-notification}

在Brand Portal预定进行维护之前，在登录Brand Portal后，通知将显示为横幅。示例通知：

![](assets/bp_maintenance_notification.png)

您可以忽略此通知并继续使用Brand Portal。此通知显示在每个新会话中。

## 版本和系统信息 {#release-and-system-information}

<!--* [What's new](../using/whats-new.md)-->
* [发行说明](brand-portal-release-notes.md)
* [支持的文件格式](brand-portal-supported-formats.md)

## Related resources {#related-resources}

* [Adobe客户关怀](https://helpx.adobe.com/marketing-cloud/contact-support.html)
* [AEM 论坛](https://www.adobe.com/go/aod_forums_en)