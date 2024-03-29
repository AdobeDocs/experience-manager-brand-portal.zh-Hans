---
title: Experience Manager Assets Brand Portal概述
seo-title: Overview of Experience Manager Assets Brand Portal
description: Experience Manager Assets Brand Portal可以帮助您轻松获取、控制经过批准的创意资产，并将这些资产安全地分发给跨设备的外部参与方和内部业务用户。
seo-description: Experience Manager Assets Brand Portal can help you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
exl-id: 0f2c45e4-416e-451a-905b-06c5e42a9272
source-git-commit: d84d138a2819ff293d0c808b0dcebe02e03da121
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Experience Manager Assets Brand Portal概述 {#overview-of-aem-assets-brand-portal}

作为营销人员，您有时需要与渠道合作伙伴和内部业务用户协作，以快速创建、管理和向客户提供相关数字内容。 在整个客户历程中及时交付相关内容对于提高需求、转化、参与度和客户忠诚度至关重要。

但是，开发解决方案来支持与扩展的内部团队、合作伙伴和经销商高效、安全地共享批准的品牌徽标、指南、活动资产或产品快照是一项挑战。

**Adobe Experience Manager (AEM) Assets Brand Portal** 关注营销人员通过提供资产分发和资产贡献功能来与在全球分发的Brand Portal用户有效协作的需求。

Asset Distribution允许您轻松地获取、控制经批准的创意资产，并将这些资产安全地分发给跨设备的外部参与方和内部业务用户。 相反，通过资源贡献，Brand Portal用户能够将资源上传到Brand Portal并发布到Experience Manager Assets，而无需访问创作环境。 贡献功能称为 **Brand Portal中的资源源**. 同时，它还改善了Brand Portal在资产分发方面的整体体验以及Brand Portal用户（外部机构/团队）的贡献，加快了资产上市时间，并降低了不合规和未经授权访问的风险。
看， [Brand Portal中的资源源](brand-portal-asset-sourcing.md).

通过基于浏览器的门户环境，您可以轻松地以批准的格式上传、浏览、搜索、预览和导出资源。

## 使用 Brand Portal 配置 Experience Manager Assets {#configure-brand-portal}

使用Brand Portal配置Adobe Experience Manager Assets可为Brand Portal用户启用资产发布、资产分配和资产贡献功能。

>[!NOTE]
>
>Experience Manager Assetsas a Cloud Service、Experience Manager Assets 6.3及更高版本支持使用Brand Portal配置Experience Manager Assets。

通过从Cloud Manager激活Experience Manager Assets，可使用Brand Portal自动配置Brand Portalas a Cloud Service。 激活工作流会在后端创建所需的配置，并在与Experience Manager Assetsas a Cloud Service实例相同的IMS组织上激活Brand Portal。

而使用Experience Manager Assets Console通过Brand Portal手动配置Adobe Developer （内部部署和托管服务），从而可获取Adobe的Identity Management Services (IMS)令牌以授权Brand Portal租户。

有关更多信息，请参阅 [使用Brand Portal配置Experience Manager Assets](../using/configure-aem-assets-with-brand-portal.md).

## Brand Portal中的用户角色 {#Personas}

Brand Portal支持以下用户角色：

* 访客用户
* 查看者
* 编辑器
* 管理员

下表列出了具有这些角色的用户可以执行的任务：

|  | **浏览** | **搜索** | **下载** | **共享文件夹** | **共享收藏集** | **以链接方式共享资产** | **访问管理工具** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **访客用户** | ✓韩亚航空* | ✓* | ✓* | x | x | x | x |
| **查看者** | ✓ | ✓ | ✓ | x | x | x | x |
| **编辑器** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **管理员** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

>[!NOTE]
>
>访客用户只能浏览、访问和搜索公共文件夹和收藏集中的资产。

<!--
&#42; Viewer users can access and download the public assets shared with them, and can add these assets to create their own collections.

>[!NOTE]
>
>There is a known issue that the share link for collections is currently visible to the viewer users. The viewer users does not have the privilege to add users to create a share link. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.
-->

### 访客用户 {#guest-user}

Experience Manager Assets Brand Portal允许 [访客访问](#request-access-to-brand-portal) Brand Portal。 访客用户无需凭据即可进入门户，并且有权访问公共文件夹和收藏集。 作为访客用户，您可以浏览资源详细信息，并完整查看公共文件夹和收藏集成员的资源。 您可以搜索、下载公共资产并将其添加到 [!UICONTROL 灯箱] 收藏集。

但是，来宾会话会限制您创建收藏集和保存的搜索，并进一步共享它们。 来宾会话中的用户无法访问文件夹和收藏集设置，也无法以链接形式共享资产。 以下是访客用户可以执行的任务列表：

* [浏览和访问公共资源](browse-assets-brand-portal.md)

* [搜索公共资产](brand-portal-searching.md)

* [下载公共资产](brand-portal-download-assets.md)

* [将资源添加到 [!UICONTROL 灯箱]](brand-portal-light-box.md#add-assets-to-lightbox)

有关更多信息，请参阅 [来宾访问Brand Portal](../using/guest-access.md).

### 查看者 {#viewer}

Brand Portal用户定义于 [!DNL Admin Console] 具有查看者角色且有权访问Brand Portal的用户。 具有此角色的用户可以登录Brand Portal并访问允许的文件夹、收藏集和资源。 用户还可以浏览、预览、下载和导出资源（原始或特定演绎版）、配置帐户设置以及搜索资源。 以下是查看器可以执行的任务列表：

* [浏览资源](browse-assets-brand-portal.md)

* [搜索资产](brand-portal-searching.md)

* [下载资源](brand-portal-download-assets.md)

### 编辑器 {#editor}

具有编辑者角色的用户可以执行查看器可以执行的所有任务。 此外，和编辑器可以查看管理员共享的文件和文件夹。 具有编辑者角色的用户还可以与其他人共享内容（文件、文件夹、收藏集）。

除了查看器可以执行的任务外，编辑器还可以执行以下附加任务：

* [共享文件夹](brand-portal-sharing-folders.md)

* [共享收藏集](brand-portal-share-collection.md)

* [以链接方式共享资产](brand-portal-link-share.md)

### 管理员 {#administrator}

管理员包括中标记为系统管理员或Brand Portal产品管理员的用户 [!UICONTROL Admin Console]. 管理员可以添加和删除系统管理员和用户，定义预设，向用户发送电子邮件，以及查看门户使用情况和存储报告。

>[!NOTE]
>
>在Brand Portal中，在中标记为支持管理员角色的用户 [!UICONTROL Admin Console] 具有与系统管理员相同的权限。

管理员可以执行编辑者可以执行的所有任务。 以下是管理员可以执行的其他任务：

* [管理用户、组和用户角色](brand-portal-adding-users.md)

* [自定义壁纸、页面标题和电子邮件](brand-portal-branding.md)

* [使用自定义搜索 Facet](brand-portal-search-facets.md)

* [使用元数据架构表单](brand-portal-metadata-schemas.md)

* [应用图像预设或动态演绎版](brand-portal-image-presets.md)

* [使用报告](brand-portal-reports.md)

除了上述任务之外，AEM Assets中的作者还可以执行以下任务：

* [使用 Brand Portal 配置 AEM Assets](../using/configure-aem-assets-with-brand-portal.md)

* [将文件夹发布到 Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-folder.html)

* [将收藏集发布到 Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-collection.html)

## Brand Portal URL的替代别名 {#tenant-alias-for-portal-url}

从Brand Portal 6.4.3开始，组织可以为其Brand Portal租户的现有URL拥有一个替代（别名） URL。 别名URL可通过在URL中使用备用前缀来创建。\
如果租户名称大于32个字符，则需要创建租户别名。
请注意，只能自定义Brand Portal URL的前缀，而不能自定义整个URL。 例如，具有现有域的组织 `geomettrix.brand-portal.adobe.com` 可以获取 `geomettrixinc.brand-portal.adobe.com` 已应请求创建。

但是，AEM创作实例可以是 [已配置](../using/configure-aem-assets-with-brand-portal.md) 仅使用租户ID URL，不使用租户别名（替代）URL。

>[!NOTE]
>
>要在现有门户URL中获取租户名称的别名，组织需要通过新的租户别名创建请求联系客户支持。 首先检查别名是否可用，然后创建别名，以处理此请求。
>
>要替换旧别名或删除旧别名，需要执行相同的过程。

## 请求访问Brand Portal {#request-access-to-brand-portal}

用户可以从登录屏幕请求访问Brand Portal。 这些请求将发送给Brand Portal管理员，管理员将通过Adobe向用户授予访问权限 [!UICONTROL Admin Console]. 授予访问权限后，用户会收到通知电子邮件。

要请求访问权限，请执行以下操作：

1. 从Brand Portal登录页面中，选择 **[!UICONTROL 单击此处]** 对应于 **[!UICONTROL 需要访问？]**. 但是，要进入来宾会话，请选择 **[!UICONTROL 单击此处]** 对应于 **[!UICONTROL 访客访问？]**.

   ![Brand Portal登录屏幕](assets/bp-login-requestaccess.png)

   此 [!UICONTROL 请求访问] 页面将打开。

1. 要申请访问组织的Brand Portal，您必须拥有有效的 [!UICONTROL Adobe ID]， [!UICONTROL Enterprise ID]，或 [!UICONTROL Federated ID].

   在 [!UICONTROL 请求访问] 页面，使用您的ID登录（场景1）或创建 [!UICONTROL Adobe ID] （情景2）：

   ![[!UICONTROL 请求访问]](assets/bplogin_request_access_2.png)

   **场景1**

   1. 如果您拥有 [!UICONTROL Adobe ID]， [!UICONTROL Enterprise ID]，或 [!UICONTROL Federated ID]，单击 **[!UICONTROL 登录]**.
此 [!UICONTROL 登录] 页面将打开。

   1. 提供您的 [!UICONTROL Adobe ID] 凭据，然后单击 **[!UICONTROL 登录]**.

      ![Adobe登录](assets/bplogin_request_access_3.png)

   您将被重定向到 [!UICONTROL 请求访问] 页面。

   **场景2**

   1. 如果您没有 [!UICONTROL Adobe ID]，要创建名称，请单击 **[!UICONTROL 获取Adobe ID]** 从 [!UICONTROL 请求访问] 页面。
此 [!UICONTROL 登录] 页面将打开。
   1. 单击 **[!UICONTROL 获取Adobe ID]**.
此 [!UICONTROL 注册] 页面将打开。
   1. 输入您的名字和姓氏、电子邮件ID和密码。
   1. 选择 **[!UICONTROL 注册]**.

      ![](assets/bplogin_request_access_5.png)

   您将被重定向到 [!UICONTROL 请求访问] 页面。

1. 下一页显示用于请求访问的姓名和电子邮件ID。 为管理员留下注释，然后单击 **[!UICONTROL 提交]**.

   ![](assets/bplogin-request-access.png)

## 产品管理员授予访问权限 {#grant-access-to-brand-portal}

Brand Portal产品管理员在其Brand Portal通知区域并通过其收件箱中的电子邮件接收访问请求。

![访问请求的通知](assets/bplogin_request_access_7.png)

要授予访问权限，产品管理员需要单击Brand Portal通知区域中的相关通知，然后单击 **[!UICONTROL 授予访问权限]**.
或者，产品管理员也可以按照访问请求电子邮件中提供的链接来访问Adobe [!UICONTROL Admin Console] 并将用户添加到相关的产品配置。

您将被重定向到 [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) 主页。 使用Adobe [!UICONTROL Admin Console] 以创建用户并将其分配给产品配置文件（以前称为产品配置），这些配置文件在Brand Portal中显示为组。 有关在中添加用户的详细信息 [!UICONTROL Admin Console]，请参见 [添加用户](brand-portal-adding-users.md#add-a-user) （按照过程中的步骤4-7添加用户）。

## Brand Portal语言 {#brand-portal-language}

您可以从Adobe更改Brand Portal语言 [!UICONTROL Experience Cloud设置].

![访问请求的通知](assets/BPLang.png)

要更改语言，请执行以下操作：

1. 选择 [!UICONTROL 用户] > [!UICONTROL 编辑个人资料] 从顶部菜单中。

   ![编辑个人资料](assets/EditBPProfile.png)

1. 开启 [!UICONTROL Experience Cloud设置] 页面上，从中选择语言 [!UICONTROL 语言] 下拉菜单。

## Brand Portal维护通知 {#brand-portal-maintenance-notification}

在计划Brand Portal停机进行维护之前，在您登录到Brand Portal后会向您显示一条通知作为横幅。 示例通知：

![](assets/bp_maintenance_notification.png)

您可以关闭此通知并继续使用Brand Portal。 此通知会显示在每个新会话中。

## 版本和系统信息 {#release-and-system-information}

* [新增功能](whats-new.md)
* [发行说明](brand-portal-release-notes.md)
* [支持的文件格式](brand-portal-supported-formats.md)

## 相关资源 {#related-resources}

<!--
* [Adobe Customer Support]()
-->

* [AEM论坛](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community)
