---
title: Experience Manager Assets Brand Portal概述
description: 了解Experience Manager Assets Brand Portal如何帮助您轻松地获取、控制经过批准的创意资源并将其安全分发给跨设备的外部方和内部业务用户。
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
exl-id: 0f2c45e4-416e-451a-905b-06c5e42a9272
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '1622'
ht-degree: 4%

---

# Experience Manager Assets Brand Portal概述 {#overview-of-aem-assets-brand-portal}

作为营销人员，您有时需要与渠道合作伙伴和内部业务用户协作，以创建、管理和快速地将相关数字内容交付给客户。 在整个客户历程中及时交付相关内容对于提高需求、转化、参与度和客户忠诚度至关重要。

但是，开发支持与团队、合作伙伴和经销商高效、安全地共享诸如已批准的品牌徽标、活动资产或产品快照等内容的解决方案非常困难。 在此过程中既要确保效率又要确保安全性，需要仔细规划和执行。

**Adobe Experience Manager (AEM) Assets Brand Portal**&#x200B;侧重于营销人员通过提供资产分发和资产贡献功能，与分布在全球的Brand Portal用户进行有效协作的需求。

Asset Distribution允许您获取、控制经批准的创意资产，并将这些资产安全地分发给跨设备的外部各方和内部业务用户。 但是，通过资产贡献，Brand Portal用户能够将资产上传到Brand Portal并发布到Experience Manager Assets，而无需访问创作环境。 在Brand Portal **中，贡献功能称为**Assets源。 同时，它还改善了Brand Portal在资产分发方面的整体体验以及Brand Portal用户（外部机构/团队）的贡献，加快了资产上市时间，并降低了不合规和未经授权访问的风险。
请参阅Brand Portal](brand-portal-asset-sourcing.md)中的[资源源。

通过基于浏览器的门户环境，您可以轻松以批准的格式上传、浏览、搜索、预览和导出资源。

## 使用 Brand Portal 配置 Experience Manager Assets {#configure-brand-portal}

使用Brand Portal配置Adobe Experience Manager Assets可为Brand Portal用户启用资产发布、资产分配和资产贡献功能。

>[!NOTE]
>
>Experience Manager Assetsas a Cloud Service、Experience Manager Assets 6.3及更高版本支持使用Brand Portal配置Experience Manager Assets。

通过从Cloud Manager激活Experience Manager Assets，可使用Brand Portal自动配置Brand Portalas a Cloud Service。 激活工作流会在后端创建所需的配置，并在与Experience Manager Assetsas a Cloud Service实例相同的IMS组织上激活Brand Portal。

但是，Experience Manager Assets（内部部署和托管服务）是使用Brand Portal手动配置的，Adobe Developer Console可获取AdobeIdentity Management Services (IMS)令牌以授权Brand Portal租户。

有关详细信息，请参阅[使用Brand Portal配置Experience Manager Assets](../using/configure-aem-assets-with-brand-portal.md)。

## Brand Portal中的用户角色 {#Personas}

Brand Portal支持以下用户角色：

* 访客用户
* 查看者
* 编辑器
* 管理员

下表列出了具有这些角色的用户可以执行的任务：

|  | **浏览** | **搜索** | **下载** | **共享文件夹** | **共享收藏集** | **以链接方式共享资产** | **访问管理工具** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **来宾用户** | ✓韩亚航空* | ✓韩亚航空* | ✓韩亚航空* | x | x | x | x |
| **查看器** | ✓ | ✓ | ✓ | x | x | x | x |
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

Experience Manager Assets Brand Portal允许[来宾访问Brand Portal](#request-access-to-brand-portal)。 访客用户无需凭据即可进入门户，并且有权访问公共文件夹和收藏集。 作为访客用户，您可以浏览资源详细信息，并拥有公用文件夹和收藏集成员的完整资源视图。 您可以搜索、下载公共资产，并将其添加到[!UICONTROL Lightbox]收藏集。

但是，来宾会话会限制您创建收藏集和保存的搜索，并进一步共享它们。 来宾会话中的用户无法访问文件夹和收藏集设置，也无法以链接形式共享资产。 以下是访客用户可以执行的任务列表：

* [浏览和访问公共资源](browse-assets-brand-portal.md)

* [搜索公共资产](brand-portal-searching.md)

* [下载公共资产](brand-portal-download-assets.md)

* [将资源添加到[!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

有关详细信息，请转到[来宾访问Brand Portal](../using/guest-access.md)。

### 查看者 {#viewer}

在[!DNL Admin Console]中定义的Brand Portal用户，其可通过查看者角色访问Brand Portal。 具有此角色的用户可以登录Brand Portal并访问允许的文件夹、收藏集和资源。 用户还可以浏览、预览、下载和导出资源（原始或特定演绎版）、配置帐户设置以及搜索资源。 以下是查看器可以执行的任务列表：

* [浏览资源](browse-assets-brand-portal.md)

* [搜索资产](brand-portal-searching.md)

* [下载资源](brand-portal-download-assets.md)

### 编辑器 {#editor}

具有编辑者角色的用户可以执行查看器可以执行的所有任务。 此外，和编辑器可以查看管理员共享的文件和文件夹。 具有编辑者角色的用户还可以与其他人共享内容（文件、文件夹、收藏集）。

除了查看器可以执行的任务外，编辑器还可以执行以下附加任务：

* [共享文件夹](brand-portal-sharing-folders.md)

* [共享收藏集](brand-portal-share-collection.md)

* [以链接形式共享资产](brand-portal-link-share.md)

### 管理员 {#administrator}

管理员包括在[!UICONTROL Admin Console]中标记为系统管理员或Brand Portal产品管理员的用户。 管理员可以添加和删除系统管理员和用户，定义预设，向用户发送电子邮件，以及查看门户使用情况和存储报告。

>[!NOTE]
>
>在Brand Portal中，在[!UICONTROL Admin Console]中标记为支持管理员角色的用户具有与系统管理员相同的权限。

管理员可以执行编辑者可以执行的所有任务。 以下是管理员可以执行的其他任务：

* [管理用户、组和用户角色](brand-portal-adding-users.md)
* [自定义壁纸、页面标题和电子邮件](brand-portal-branding.md)
* [使用自定义搜索彩块化](brand-portal-search-facets.md)
* [使用元数据架构](brand-portal-metadata-schemas.md)
* [应用图像预设或动态演绎版](brand-portal-image-presets.md)
* [使用报告](brand-portal-reports.md)

除了上述任务之外，AEM Assets中的作者还可以执行以下任务：

* [使用Brand Portal配置AEM Assets](../using/configure-aem-assets-with-brand-portal.md)
* [将文件夹发布到 Brand Portal](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/brandportal/brand-portal-publish-folder)
* [将收藏集发布到 Brand Portal](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/brandportal/brand-portal-publish-collection)

## Brand Portal URL的替代别名 {#tenant-alias-for-portal-url}

从Brand Portal 6.4.3开始，组织可以为其Brand Portal租户的每个现有URL拥有一个替代（别名）URL。 别名URL可通过在URL中使用备用前缀来创建。\
如果租户名称大于32个字符，则需要创建租户别名。
请注意，只能自定义Brand Portal URL的前缀，而不能自定义整个URL。 例如，具有现有域`geomettrix.brand-portal.adobe.com`的组织可以按请求创建`geomettrixinc.brand-portal.adobe.com`。

但是，AEM创作实例只能使用租户ID URL [配置](../using/configure-aem-assets-with-brand-portal.md)，而不能使用租户别名（替代）URL。

>[!NOTE]
>
>要在现有门户URL中获取租户名称的别名，组织需要通过新的租户别名创建请求联系客户支持。 首先，检查别名是否可用，然后创建别名以处理此请求。
>
>要替换旧别名或删除旧别名，需要执行相同的过程。

## 请求访问Brand Portal {#request-access-to-brand-portal}

用户可以从登录屏幕请求访问Brand Portal。 这些请求将发送给Brand Portal管理员，管理员通过Adobe[!UICONTROL Admin Console]向用户授予访问权限。 授予访问权限后，用户会收到通知电子邮件。

要请求访问权限，请执行以下操作：

1. 从Brand Portal登录页面中，选择&#x200B;**[!UICONTROL 单击此处]**，它与&#x200B;**[!UICONTROL 需要访问吗？]**。但是，要进入来宾会话，请选择与&#x200B;**[!UICONTROL 来宾访问？]**&#x200B;对应的&#x200B;**[!UICONTROL 单击此处]**。

   ![Brand Portal登录屏幕](assets/bp-login-requestaccess.png)

   将打开[!UICONTROL 请求访问]页面。

1. 若要请求访问组织的Brand Portal，您必须拥有有效的[!UICONTROL Adobe ID]、[!UICONTROL Enterprise ID]或[!UICONTROL Federated ID]。

   在[!UICONTROL 请求访问]页面中，使用您的ID登录（场景1）或创建[!UICONTROL Adobe ID]（场景2）：

   ![[!UICONTROL 请求访问]](assets/bplogin_request_access_2.png)

   **方案1**

   1. 如果您有[!UICONTROL Adobe ID]、[!UICONTROL Enterprise ID]或[!UICONTROL Federated ID]，请单击&#x200B;**[!UICONTROL 登录]**。
[!UICONTROL 登录]页面打开。

   1. 提供您的[!UICONTROL Adobe ID]凭据，然后单击&#x200B;**[!UICONTROL 登录]**。

      ![Adobe登录](assets/bplogin_request_access_3.png)

   您被重定向到[!UICONTROL 请求访问]页面。

   **方案2**

   1. 如果您没有[!UICONTROL Adobe ID]，若要创建一个，请从[!UICONTROL 请求访问]页面中单击&#x200B;**[!UICONTROL 获取Adobe ID]**。
[!UICONTROL 登录]页面打开。
   1. 单击&#x200B;**[!UICONTROL 获取Adobe ID]**。
[!UICONTROL 注册]页面打开。
   1. 输入您的名字和姓氏、电子邮件ID和密码。
   1. 选择&#x200B;**[!UICONTROL 注册]**。

      ![](assets/bplogin_request_access_5.png)

   您被重定向到[!UICONTROL 请求访问]页面。

1. 下一页显示用于请求访问的姓名和电子邮件ID。 为管理员留下评论，然后单击&#x200B;**[!UICONTROL 提交]**。

   ![](assets/bplogin-request-access.png)

## 产品管理员授予访问权限 {#grant-access-to-brand-portal}

Brand Portal产品管理员在其Brand Portal通知区域并通过其收件箱中的电子邮件接收访问请求。

![访问请求的通知](assets/bplogin_request_access_7.png)

要授予访问权限，产品管理员需要单击Brand Portal通知区域中的相关通知，然后单击&#x200B;**[!UICONTROL 授予访问权限]**。
或者，产品管理员可以按照访问请求电子邮件中提供的链接访问Adobe[!UICONTROL Admin Console]，并将用户添加到相关的产品配置中。

您被重定向到[Adobe[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview)主页。 使用Adobe[!UICONTROL Admin Console]创建用户，并将其分配给产品配置文件（以前称为产品配置），这些配置文件在Brand Portal中显示为组。 有关在[!UICONTROL Admin Console]中添加用户的详细信息，请参阅[添加用户](brand-portal-adding-users.md#add-a-user)（按照过程中的步骤4-7添加用户）。

## Brand Portal语言 {#brand-portal-language}

您可以从Adobe[!UICONTROL Experience Cloud设置]中更改Brand Portal语言。

![访问请求的通知](assets/BPLang.png)

要更改语言，请执行以下操作：

1. 从顶部菜单中选择[!UICONTROL 用户] > [!UICONTROL 编辑配置文件]。

   ![编辑个人资料](assets/EditBPProfile.png)

1. 在[!UICONTROL Experience Cloud设置]页面上，从[!UICONTROL 语言]下拉菜单中选择一种语言。

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
