---
title: Experience Manager Assets Brand Portal概述
seo-title: Overview of Experience Manager Assets Brand Portal
description: Experience Manager Assets Brand Portal可以帮助您跨设备轻松获取、控制和安全地将已批准的创意资产分发给外部各方和内部业务用户。
seo-description: Experience Manager Assets Brand Portal can help you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
exl-id: 0f2c45e4-416e-451a-905b-06c5e42a9272
source-git-commit: 12187c4a98e1541be27b06eefedb1b654c5fb083
workflow-type: tm+mt
source-wordcount: '1528'
ht-degree: 7%

---

# Experience Manager Assets Brand Portal概述 {#overview-of-aem-assets-brand-portal}

作为营销人员，您有时需要与渠道合作伙伴和内部业务用户协作，以快速创建、管理和向客户交付相关的数字内容。 在整个客户历程中及时交付相关内容对于提高需求、转化、参与度和客户忠诚度至关重要。

但是，开发解决方案是一项挑战，该解决方案支持与扩展的内部团队、合作伙伴和经销商高效、安全地共享已批准的品牌徽标、准则、活动资产或产品照片。

**Adobe Experience Manager(AEM)Assets Brand Portal** 重点关注营销人员通过提供资产分发和资产贡献功能与全球分布的Brand Portal用户进行有效协作的需求。

资产分发允许您跨设备轻松获取、控制和安全地将批准的创意资产分发给外部各方和内部业务用户。 然而，资产贡献功能使Brand Portal用户能够将资产上传到Brand Portal并发布到Experience Manager Assets，而无需访问创作环境。 贡献功能称为 **Brand Portal中的资产源**. 同时，它还改善了Brand Portal在资产分发方面的整体体验，并且改善了Brand Portal用户（外部机构/团队）的贡献，加快了资产的上市时间，并降低了不合规和未授权访问的风险。
看， [Brand Portal中的资产源](brand-portal-asset-sourcing.md).

通过基于浏览器的门户环境，您可以轻松上传、浏览、搜索、预览和导出已批准格式的资产。

## 使用 Brand Portal 配置 Experience Manager Assets {#configure-brand-portal}

使用Brand Portal配置Adobe Experience Manager Assets可为Brand Portal用户启用资产发布、资产分发和资产贡献功能。

>[!NOTE]
>
>Experience Manager Assetsas a Cloud Service、Experience Manager Assets 6.3及更高版本支持使用Brand Portal配置Experience Manager Assets。

Experience Manager Assetsas a Cloud Service通过从Cloud Manager激活Brand Portal，自动配置为Brand Portal。 激活工作流会在后端创建所需的配置，并在与Experience Manager Assetsas a Cloud Service实例相同的IMS组织上激活Brand Portal。

而是，Experience Manager Assets（内部部署版和托管服务版）会使用Brand Portal开发人员控制台通过Adobe手动配置，该控制台可获取AdobeIdentity Management服务(IMS)令牌以授权Brand Portal租户。

有关更多信息，请参阅 [将Experience Manager Assets配置为Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

## Brand Portal中的用户角色 {#Personas}

Brand Portal支持以下用户角色：

* 来宾用户
* 查看者
* 编辑者
* 管理员

下表列出了这些角色中的用户可以执行的任务：

|  | **浏览** | **搜索** | **下载** | **共享文件夹** | **共享收藏集** | **以链接方式共享资产** | **访问管理工具** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **来宾用户** | ✓* | ✓* | ✓* | x | x | x | x |
| **查看者** | ✓ | ✓ | ✓ | x | x | x | x |
| **编辑者** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **管理员** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

>[!NOTE]
>
>来宾用户只能浏览、访问和搜索公共文件夹和收藏集中的资产。

<!--
&#42; Viewer users can access and download the public assets shared with them, and can add these assets to create their own collections.

>[!NOTE]
>
>There is a known issue that the share link for collections is currently visible to the viewer users. The viewer users does not have the privilege to add users to create a share link. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.
-->

### 来宾用户 {#guest-user}

任何未经身份验证而对Brand Portal上的资产具有有限访问权限的用户都是来宾用户。 来宾会话允许用户访问公共文件夹和收藏集。 作为来宾用户，您可以浏览资产详细信息，并拥有公共文件夹和收藏集成员的完整资产视图。 您可以搜索、下载公共资产并将其添加到 [!UICONTROL 灯箱] 收藏集。

但是，来宾会话会限制您创建收藏集和保存的搜索，并进一步共享这些搜索。 来宾会话中的用户无法访问文件夹和收藏集设置，并且无法将资产共享为链接。 以下是来宾用户可以执行的任务列表：

* [浏览和访问公共资产](browse-assets-brand-portal.md)

* [搜索公共资产](brand-portal-searching.md)

* [下载公共资产](download-assets.md)

* [将资产添加到 [!UICONTROL 灯箱]](brand-portal-light-box.md#add-assets-to-lightbox)

### 查看者 {#viewer}

Brand Portal中的标准用户通常是具有“查看者”角色的用户。 具有此角色的用户可以访问允许的文件夹、收藏集和资产。 用户还可以浏览、预览、下载和导出资产（原始或特定演绎版）、配置帐户设置，以及搜索资产。 以下是查看器可以执行的任务列表：

* [浏览资产](browse-assets-brand-portal.md)

* [搜索资产](brand-portal-searching.md)

* [下载资源](download-assets.md)

### 编辑者 {#editor}

具有编辑者角色的用户可以执行查看器可以执行的所有任务。 此外，和编辑器还可以查看管理员共享的文件和文件夹。 具有编辑者角色的用户还可以与他人共享内容（文件、文件夹、收藏集）。

除了查看器可以执行的任务之外，编辑器还可以执行以下其他任务：

* [共享文件夹](brand-portal-sharing-folders.md)

* [共享收藏集](brand-portal-share-collection.md)

* [以链接方式共享资产](brand-portal-link-share.md)

### 管理员 {#administrator}

管理员包括在中标记为系统管理员或Brand Portal产品管理员的用户 [!UICONTROL Admin Console]. 管理员可以添加和删除系统管理员和用户、定义预设、向用户发送电子邮件，以及查看门户使用情况和存储报告。

管理员可以执行编辑器可以执行的所有任务，以执行以下其他任务：

* [管理用户、组和用户角色](brand-portal-adding-users.md)

* [自定义墙纸、页眉和电子邮件](brand-portal-branding.md)

* [使用自定义搜索 Facet](brand-portal-search-facets.md)

* [使用元数据架构表单](brand-portal-metadata-schemas.md)

* [应用图像预设或动态演绎版](brand-portal-image-presets.md)

* [使用报告](brand-portal-reports.md)

除了上述任务之外，AEM Assets中的作者还可以执行以下任务：

* [使用 Brand Portal 配置 AEM Assets](../using/configure-aem-assets-with-brand-portal.md)

* [将文件夹发布到 Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-folder.html)

* [将收藏集发布到 Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-collection.html)

## Brand Portal url的替代别名 {#tenant-alias-for-portal-url}

从Brand Portal 6.4.3开始，组织可以为其Brand Portal租户的现有URL使用一个替代（别名）URL。 别名URL可通过在URL中使用备用前缀来创建。\
请注意，只能自定义Brand Portal URL的前缀，而不能自定义整个URL。 例如，具有现有域的组织 `geomettrix.brand-portal.adobe.com` ceg `geomettrixinc.brand-portal.adobe.com` 已根据请求创建。

但是，AEM创作实例可以是 [已配置](../using/configure-aem-assets-with-brand-portal.md) 仅使用租户ID URL，而不使用租户别名（备用）URL。

>[!NOTE]
>
>要获取现有门户URL中租户名称的别名，组织需要通过新的租户别名创建请求联系客户支持。 首先检查别名是否可用，然后创建别名，即可处理此请求。
>
>要替换旧别名或删除旧别名，需要执行相同的过程。

## 请求访问Brand Portal {#request-access-to-brand-portal}

用户可以从登录屏幕请求访问Brand Portal。 这些请求将发送给Brand Portal管理员，管理员会通过Adobe授予用户访问权限 [!UICONTROL Admin Console]. 授予访问权限后，用户会收到通知电子邮件。

要请求访问，请执行以下操作：

1. 从Brand Portal登录页面中，选择 **[!UICONTROL 单击此处]** 对应 **[!UICONTROL 需要访问权限？]**. 但是，要进入来宾会话，请选择 **[!UICONTROL 单击此处]** 对应 **[!UICONTROL 来宾访问？]**.

   ![Brand Portal登录屏幕](assets/bp-login-requestaccess.png)

   的 [!UICONTROL 请求访问] 页面。

1. 要请求访问组织的Brand Portal，您必须具有 [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID]或 [!UICONTROL Federated ID].

   在 [!UICONTROL 请求访问] 页面，使用您的ID登录（场景1），或创建 [!UICONTROL Adobe ID] (情景2:

   ![[!UICONTROL 请求访问]](assets/bplogin_request_access_2.png)

   **场景1**

   1. 如果您有 [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID]或 [!UICONTROL Federated ID]，单击 **[!UICONTROL 登录]**.
的 [!UICONTROL 登录] 页面。

   1. 提供 [!UICONTROL Adobe ID] 凭据，单击 **[!UICONTROL 登录]**.

      ![Adobe登录](assets/bplogin_request_access_3.png)
   系统会将您重定向到 [!UICONTROL 请求访问] 页面。

   **场景2**

   1. 如果您没有 [!UICONTROL Adobe ID]，要创建一个，请单击 **[!UICONTROL 获取Adobe ID]** 从 [!UICONTROL 请求访问] 页面。
的 [!UICONTROL 登录] 页面。
   1. 单击 **[!UICONTROL 获取Adobe ID]**.
的 [!UICONTROL 注册] 页面。
   1. 输入您的名字和姓氏、电子邮件ID和密码。
   1. 选择 **[!UICONTROL 注册]**.

      ![](assets/bplogin_request_access_5.png)
   系统会将您重定向到 [!UICONTROL 请求访问] 页面。

1. 下一页显示您的姓名和用于请求访问权限的电子邮件ID。 为管理员留下注释，然后单击 **[!UICONTROL 提交]**.

   ![](assets/bplogin-request-access.png)

## 产品管理员授予访问权限 {#grant-access-to-brand-portal}

Brand Portal产品管理员会在其Brand Portal通知区域并通过其收件箱中的电子邮件接收访问请求。

![访问请求的通知](assets/bplogin_request_access_7.png)

要授予访问权限，产品管理员需要单击Brand Portal通知区域中的相关通知，然后单击 **[!UICONTROL 授予访问权限]**.
或者，产品管理员也可以按照访问请求电子邮件中提供的链接来访问Adobe [!UICONTROL Admin Console] 并将用户添加到相关产品配置。

系统会将您重定向到 [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) 主页。 使用Adobe [!UICONTROL Admin Console] 创建用户并将其分配给在Brand Portal中显示为组的产品配置文件（以前称为产品配置）。 有关在 [!UICONTROL Admin Console]，请参阅 [添加用户](brand-portal-adding-users.md#add-a-user) （按照过程中的步骤4-7添加用户）。

## Brand Portal语 {#brand-portal-language}

您可以将Brand Portal语言从Adobe [!UICONTROL Experience Cloud设置].

![访问请求的通知](assets/BPLang.png)

要更改语言，请执行以下操作：

1. 选择 [!UICONTROL 用户] > [!UICONTROL 编辑配置文件] 中。

   ![编辑个人资料](assets/EditBPProfile.png)

1. 开 [!UICONTROL Experience Cloud设置] ，请从 [!UICONTROL 语言] 下拉菜单。

## Brand Portal维护通知 {#brand-portal-maintenance-notification}

在计划Brand Portal停机进行维护之前，您登录Brand Portal后，会将通知显示为横幅。 示例通知：

![](assets/bp_maintenance_notification.png)

您可以关闭此通知并继续使用Brand Portal。 此通知将显示在每个新会话中。

## 发行和系统信息 {#release-and-system-information}

* [新增功能](whats-new.md)
* [发行说明](brand-portal-release-notes.md)
* [支持的文件格式](brand-portal-supported-formats.md)

## 相关资源 {#related-resources}

<!--
* [Adobe Customer Support]()
-->

* [AEM 论坛](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community)
