---
title: AEM Assets品牌门户概述
seo-title: AEM Assets品牌门户概述
description: AEM Assets品牌门户可以帮助您轻松地跨设备获得、控制和安全地将获准的创意资产分发给外部方和内部业务用户。
seo-description: AEM Assets品牌门户可以帮助您轻松地跨设备获得、控制和安全地将获准的创意资产分发给外部方和内部业务用户。
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
translation-type: tm+mt
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '1522'
ht-degree: 8%

---


# AEM Assets品牌门户概述 {#overview-of-aem-assets-brand-portal}

作为营销人员，您有时需要与渠道合作伙伴和内部业务用户协作，以快速创建、管理相关数字内容并向客户提供相关内容。 在整个客户旅程中及时投放相关内容对于提高需求、转化率、参与度和客户忠诚度至关重要。

但是，开发解决方案是一个挑战，它们支持与扩展的内部团队、合作伙伴和经销商高效、安全地共享经批准的品牌徽标、准则、活动资产或产品照片。

**Adobe Experience Manager(AEM)资产品牌门户** ，注重营销人员通过提供资产分发和资产贡献功能与全球分布的品牌门户用户进行有效协作的需求。

通过资产分发，您可以轻松地跨设备向外部方和内部业务用户分发获准的创意资产，并对其进行控制和安全分发。 但是，资产贡献使Brand Portal用户能够将资产上传到Brand Portal并发布到AEM Assets，而无需访问作者环境。 贡献功能在品牌门户 **中称为资产来源补充**。 此外，它还改善了Brand Portal用户（外部机构／团队）在资产分发和贡献方面的整体Brand Portal体验，加快了资产上市时间，并降低了不合规和未经授权的访问风险。
请参阅， [品牌门户中的资产来源补充](brand-portal-asset-sourcing.md)。

基于浏览器的门户环境使您能够轻松上传、浏览、搜索、预览和导出已批准格式的资产。

## 使用 Brand Portal 配置 AEM Assets {#configure-brand-portal}

Adobe Experience Manager(AEM)资产通过Adobe开发人员控制台配置为品牌门户，该控制台为您的品牌门户租户购买IMS令牌以进行授权。

>[!NOTE]
>
>AEM Assets云服务、AEM Assets6.3及更高版本支持通过Adobe开发人员控制台使用品牌门户配置AEM Assets。

### Prerequisites to configure AEM Assets with Brand Portal {#prerequisites}

您需要以下各项才能使用 Brand Portal 配置 AEM Assets：

* 一个正在运行的AEM Assets实例。
* Brand Portal 租户 URL。
* 对 Brand Portal 租户的 IMS 组织具有系统管理员权限的用户。

有关详细信息，请参 [阅使用品牌门户配置AEM Assets](../using/configure-aem-assets-with-brand-portal.md)。

## Brand Portal中的用户角色 {#Personas}

Brand Portal支持以下用户角色：

* 客人用户
* 查看者
* 编辑者
* 管理员

下表列表了这些角色中的用户可以执行的任务:

|  | **浏览** | **搜索** | **下载** | **共享文件夹** | **共享收藏集** | **以链接方式共享资产** | **访问管理工具** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **客人用户** | ✓* | ✓* | ✓* | x | x | x | x |
| **查看者** | ✓ | ✓ | ✓ | x | x | x | x |
| **编辑者** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **管理员** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

*客人用户只能浏览、访问和搜索公共文件夹和集合中的资产。

### Guest user {#guest-user}

未经身份验证而对品牌门户上的资源具有有限访问权限的任何用户都是客人用户。 客人会话允许用户访问公共文件夹和集合。 作为客人用户，您可以浏览资产详细信息，并拥有公共文件夹和集合成员的完整资产视图。 您可以搜索、下载公共资产并将其添加到Lightbox [!UICONTROL 收藏集] 。

但是，客人会话限制您创建集合和保存的搜索，并进一步共享它们。 来宾会话中的用户无法访问文件夹和集合设置，也无法将资产共享为链接。 以下是客人用户可以执行的列表任务:

[浏览和访问公共资源](browse-assets-brand-portal.md)

[搜索公共资产](brand-portal-searching.md)

[下载公共资产](brand-portal-download-users.md)

[将资产添加到 [!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

### 查看者 {#viewer}

Brand Portal中的标准用户通常是具有查看器角色的用户。 具有此角色的用户可以访问允许的文件夹、收藏集和资产。 用户还可以浏览、预览、下载和导出资产（原始或特定演绎版）、配置帐户设置以及搜索资产。 以下是查看器可以执行的列表任务:

[浏览资源](browse-assets-brand-portal.md)

[搜索资产](brand-portal-searching.md)

[下载资产](brand-portal-download-users.md)

### 编辑者 {#editor}

具有编辑者角色的用户可以执行查看器可以执行的所有任务。 此外，编辑者还可以视图管理员共享的文件和文件夹。 具有编辑者角色的用户还可以与他人共享内容（文件、文件夹、集合）。

除了查看器可以执行的任务之外，编辑者还可以执行以下其他任务:

[共享文件夹](brand-portal-sharing-folders.md)

[共享收藏集](brand-portal-share-collection.md)

[以链接方式共享资产](brand-portal-link-share.md)

### 管理员 {#administrator}

管理员包括在Admin Console中标记为系统管理员或Brand Portal产品管理员的 [!UICONTROL 用户]。 管理员可以添加和删除系统管理员和用户、定义预设、向用户发送电子邮件以及视图门户使用情况和存储报告。

管理员可以执行编辑者可以执行的所有任务，以执行以下其他任务:

[管理用户、组和用户角色](brand-portal-adding-users.md)

[自定义墙纸、页眉和电子邮件](brand-portal-branding.md)

[使用自定义搜索 Facet](brand-portal-search-facets.md)

[使用元数据架构表单](brand-portal-metadata-schemas.md)

[应用图像预设或动态演绎版](brand-portal-image-presets.md)

[使用报告](brand-portal-reports.md)

除了上述任务之外，AEM Assets中的作者还可以执行以下任务:

[使用 Brand Portal 配置 AEM Assets](../using/configure-aem-assets-with-brand-portal.md)

[将文件夹发布到 Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-folder.html)

[将收藏集发布到 Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-collection.html)

## 品牌门户URL的替代别名 {#tenant-alias-for-portal-url}

从Brand Portal 6.4.3开始，组织可以拥有其Brand Portal租户的现有URL的一个替代（别名）URL。 别名URL可以通过在URL中具有替代前缀来创建。\
请注意，只能自定义品牌门户URL的前缀，而不能自定义整个URL。 例如，具有现有域 **[!UICONTROL geometrix.brand-portal.adobe.com的组织]** ，可 **[!UICONTROL 以获取根据请求创建的geometrixinc.brand-portal]** .adobe.com。

但是，AEM Author实例只能 [使用租](../using/configure-aem-assets-with-brand-portal.md) 户ID URL进行配置，而不能使用租户别名（备用）URL进行配置。

>[!NOTE]
>
>要获取现有门户URL中租户名称的别名，组织需要通过新的租户别名创建请求与Adobe支持部门联系。 处理此请求的方法是先检查别名是否可用，然后创建别名。
>
>要替换旧别名或删除旧别名，需要执行相同的过程。

## Request access to Brand Portal {#request-access-to-brand-portal}

用户可以从登录屏幕请求对Brand Portal的访问权。 这些请求将发送给Brand Portal管理员，管理员通过AdobeAdmin Console授予用户访 [!UICONTROL 问权]。 授予访问权限后，用户将收到通知电子邮件。

要请求访问权限，请执行以下操作：

1. 从Brand Portal登录页面，选择“ **[!UICONTROL 单击此处]** ”，与“需 **[!UICONTROL 要访问？”]**. 但是，要进入来宾会话，请选择“ **[!UICONTROL 单击此处]** ”, **[!UICONTROL 与“来宾访问？]**”

   ![Brand Portal登录屏幕](assets/bp-login-requestaccess.png)

   此时将 [!UICONTROL 打开“请求访] 问”页面。

1. 要请求访问组织的Brand Portal，您必须具有有效 [!UICONTROL Adobe ID]、 [!UICONTROL Enterprise ID]或 [!UICONTROL Federated ID]。

   在“请 [!UICONTROL 求访问] ”页中，使用您的ID登录（方案1）或创建 [!UICONTROL Adobe ID] （方案2）:<br />
   ![[!UICONTROL 请求访问]](assets/bplogin_request_access_2.png)

   **方案1**
   1. 如果您有 [!UICONTROL Adobe ID]、 [!UICONTROL Enterprise ID]或 [!UICONTROL Federated ID]，请单击 **[!UICONTROL “登录]**”。
将打开 [!UICONTROL “登录] ”页面。
   1. 提供您的 [!UICONTROL Adobe ID] 凭据，然后单 **[!UICONTROL 击“登录”]**。<br />

   ![Adobe登录](assets/bplogin_request_access_3.png)

   您将被重定向到“请 [!UICONTROL 求访问] ”页面。<br />
   **方案2**
   1. 如果您没有Adobe ID [!UICONTROL ，请单击“请求访]问 **[!UICONTROL ”页面中的“获取]** Adobe ID [!UICONTROL ”,] 以创建。
将打开 [!UICONTROL “登录] ”页面。
   1. Click **[!UICONTROL Get an Adobe ID]**.
将打开 [!UICONTROL “注册] ”页面。
   1. 输入您的姓、名、电子邮件ID和密码。
   1. 选择 **[!UICONTROL 注册]**。<br />

   ![](assets/bplogin_request_access_5.png)

   您将被重定向到“请 [!UICONTROL 求访问] ”页面。

1. 下一页显示您的姓名和用于请求访问权限的电子邮件ID。 为管理员保留注释，然后单击“ **[!UICONTROL 提交]**”。<br />

   ![](assets/bplogin-request-access.png)

## 产品管理员授予访问权限 {#grant-access-to-brand-portal}

Brand Portal产品管理员会在其Brand Portal通知区域或通过收件箱中的电子邮件接收访问请求。

![访问请求的通知](assets/bplogin_request_access_7.png)

要授予访问权限，产品管理员需要单击品牌门户通知区域中的相关通知，然后单击授 **[!UICONTROL 予访问权限]**。
或者，产品管理员也可以按照访问请求电子邮件中提供的链接访问Adobe [!UICONTROL Admin Console] ，并将用户添加到相关的产品配置中。

您将被重定向到 [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) 主页。 使用Adobe [!UICONTROL Admin Console] ，创建用户并将其分配给产品用户档案（以前称为产品配置），这些在品牌门户中显示为组。 有关在Admin Console中添加用 [!UICONTROL 户的详]细信息， [请参阅添加用户](brand-portal-adding-users.md#add-a-user) （按照过程中的步骤4-7添加用户）。

## 品牌门户语言 {#brand-portal-language}

您可以从AdobeExperience Cloud设置中更改Brand [!UICONTROL Portal语言]。

![访问请求的通知](assets/BPLang.png)

要更改语言：

1. 从顶 [!UICONTROL 部菜] 单中选 [!UICONTROL 择“用户] ”>“编辑用户档案”。<br />

   ![编辑个人资料](assets/EditBPProfile.png)

1. 在 [!UICONTROL Experience Cloud] “设置”页面上，从“语言  ”下拉菜单中选择一种语言。

## 品牌门户维护通知 {#brand-portal-maintenance-notification}

在Brand Portal计划停用以进行维护之前，登录Brand Portal后，将显示一条通知作为横幅。 示例通知：

![](assets/bp_maintenance_notification.png)

您可以关闭此通知并继续使用Brand Portal。 此通知显示在每个新会话中。

## 发布和系统信息 {#release-and-system-information}

* [新增功能](whats-new.md)
* [发行说明](brand-portal-release-notes.md)
* [支持的文件格式](brand-portal-supported-formats.md)

## Related resources {#related-resources}

* [Adobe客户关怀](https://helpx.adobe.com/cn/marketing-cloud/contact-support.html)
* [AEM 论坛](https://www.adobe.com/go/aod_forums_en)