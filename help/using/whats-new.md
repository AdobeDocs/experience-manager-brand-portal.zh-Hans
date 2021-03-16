---
title: AEM Assets Brand Portal 的新增功能
seo-title: AEM Assets Brand Portal 的新增功能
description: 了解2021.02.0的新增功能和增强功能。
seo-description: 了解2021.02.0的新增功能和增强功能。
uuid: 2c59d738-9b53-4f25-a205-13bf75c80b77
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: introduction
discoiquuid: fec32ca3-142b-4a11-9b92-5113fc27277a
translation-type: tm+mt
source-git-commit: 26fbcf9970a77fc531b82919b29010bc37a1ab8e
workflow-type: tm+mt
source-wordcount: '6138'
ht-degree: 3%

---


# AEM Assets Brand Portal 的新增功能 {#what-s-new-in-aem-assets-brand-portal}

Adobe Experience Manager(AEM)Assets Brand Portal可帮助您轻松获取、控制获准的创意资产并将其安全地分发给外部各方和跨设备的内部业务用户。 它有助于提高资产共享的效率，加快资产的上市时间，并降低不合规和未授权访问的风险。 Adobe正在努力改善整体品牌门户体验。 抢先领略新增功能和增强功能。

## 2021.02.0 {#what-changed-in-feb-2021}中的变化

Brand Portal 2021.02.0是一个增强版本，它将AEM Assets上的Brand Portal激活工作流作为Cloud Service引入，将AEM Assets上的资产来源补充功能作为Cloud Service促进，改进了资产下载体验，并包含重要修复。 它还使管理员能够配置文件夹、收藏集的默认下载行为以及在租户级别批量下载资产。 还修改了Brand Portal **[!UICONTROL 使用情况报告]**，以反映活动的Brand Portal用户。 请参阅最新的[Brand Portal发行说明](brand-portal-release-notes.md)。

### 在AEM Assets上激活Brand Portal作为Cloud Service{#bp-automation-on-cloud-service}

AEM Assets作为Cloud Service，现在有权使用预配置的Brand Portal实例。 Cloud Manager用户可以在AEM Assets上以Cloud Service实例的形式激活Brand Portal。

以前，AEM Assets作为Cloud Service是使用Adobe开发人员控制台手动配置Brand Portal的。

Cloud Manager用户触发激活工作流，该工作流会在后端创建所需的配置，并激活与AEM Assets作为Cloud Service实例在同一IMS组织上的Brand Portal。

要在AEM Assets上以Cloud Service实例激活Brand Portal，请执行以下操作：

1. 登录到Adobe Cloud Manager，然后导航到&#x200B;**[!UICONTROL 环境]**。
1. 从列表中选择环境（逐个）以视图环境详细信息。 找到与Brand Portal关联的环境后，单击&#x200B;**[!UICONTROL 激活Brand Portal]**&#x200B;按钮，开始激活工作流。
1. 激活Brand Portal租户后，状态将更改为“已激活”。

![视图状态](assets/create-environment5.png)

请参阅[将AEM Assets上的Brand Portal作为Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html?lang=en)激活。

### 将AEM Assets上的资产来源补充作为Cloud Service{#asset-sourcing-on-cloud-service}

现在，在AEM Assets上，可以使用资产来源补充功能作为Cloud Service。 默认情况下，该功能为所有云服务用户启用。 允许的Brand Portal用户可以通过将新资产上传到贡献文件夹并将贡献文件夹从Brand Portal发布到AEM Assets作为Cloud Service实例，对资产来源补充。 管理员可以审核和批准Brand Portal用户的贡献，以进一步将其分发给其他Brand Portal用户。

以前，资产来源补充仅在AEM Assets（内部部署和托管服务）上可用。

请参阅[品牌门户中的资产来源补充](https://experienceleague.adobe.com/docs/experience-manager-brand-portal/using/asset-sourcing-in-brand-portal/brand-portal-asset-sourcing.html?lang=en)。

### 资源下载 {#asset-download-setting}

除了现有的&#x200B;**[!UICONTROL 下载设置]**&#x200B;之外，Brand Portal管理员现在还可以配置&#x200B;**[!UICONTROL 资产下载]**&#x200B;设置。 此设置允许管理员控制租户级别的文件夹、收藏集和资产（超过20个资产）的默认下载行为。

<!--
Earlier, all the asset renditions were directly downloaded in a zip folder in case of folder, collection, and bulk download of assets. As the **[!UICONTROL Download]** dialog is skipped for folders or collections, there was no mechanism to control the downloading behaviour of the assets. Due to this, the users were finding it difficut to search for a particular asset rendition from a folder containing huge bunch of downloaded renditions. 
-->

之前，所有资产演绎版都直接下载到了一个zip文件夹中。 文件夹和收藏集已跳过&#x200B;**[!UICONTROL 下载]**&#x200B;对话框，并且没有方法可以控制资产的下载行为，因此很难从大量下载中搜索特定的再现。

**[!UICONTROL 资产]** 下载设置现在提供了一个选项，用于在下载文件夹、收藏集或批量下载资产时为每个资产创建单独的文件夹。

如果禁用了&#x200B;**[!UICONTROL 资产下载]**&#x200B;设置，则会将文件夹或收藏集下载到一个zip文件夹中，其中包含同一文件夹下的所有资产演绎版，但使用共享链接下载资产除外。


以管理员身份登录到您的Brand Portal租户，然后导航到&#x200B;**[!UICONTROL 工具]** > **[!UICONTROL 下载]**。 管理员可以启用&#x200B;**[!UICONTROL 资产下载]**&#x200B;设置，在下载文件夹、收藏集和批量下载资产时为每个资产创建单独的文件夹。

![](assets/download-settings-new.png)

请参阅[从Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-brand-portal/using/download/brand-portal-download-assets.html?lang=en)下载资产。
<!--
### Download using Share link {#download-using-share-link}

The default behavior of downloading the assets using share link is now independent of the **[!UICONTROL Download Settings]**. A separate folder is created for each asset while downloading the assets using share link. 
-->

### 使用情况报告{#usage-report}

Brand Portal **[!UICONTROL 使用情况报告]**&#x200B;已修改，仅反映活动的品牌门户用户。 未分配给Admin Console中任何产品用户档案的品牌门户用户被视为非活动用户，不会反映在&#x200B;**[!UICONTROL 使用情况报告]**&#x200B;中。

以前，活动和不活动的用户都显示在使用情况报告中。

![](assets/usage-report.png)

## 2020.10.0 {#what-changed-in-oct-2020}中的变化

Brand Portal 2020.10.0是一个增强版本，侧重于简化资产下载体验并包含关键修复。 该增强功能包括新的和经过改进的资产下载工作流程、排除再现的其他选项、从&#x200B;**[!UICONTROL 演绎版]**&#x200B;面板直接下载、允许特定用户组访问和下载权限的配置，以及从所有品牌门户页面轻松导航到文件、集合和共享链接。 请参阅最新的[Brand Portal发行说明](brand-portal-release-notes.md)。


### 简化的下载体验{#download-dialog}

以前，会显示&#x200B;**[!UICONTROL 下载]**&#x200B;对话框，其中包含多个选项，例如为每个资产创建单独的文件夹、电子邮件资产、选择原始资产、自定义演绎版、动态演绎版、排除系统演绎版并启用下载加速，当选择下载多个资产或文件夹时，这些选项对非技术用户或新用户不明确。 此外，用户无法查看所有资产演绎版或排除特定的自定义或动态演绎版。

新的&#x200B;**[!UICONTROL 下载]**&#x200B;对话框可通用资产选择和筛选过程，使Brand Portal用户在下载资产演绎版时更轻松地做出有效决策。 它会根据[**[!UICONTROL Download]**](brand-portal-download-assets.md)配置和&#x200B;**[!UICONTROL Download]**&#x200B;设置列表所有选定的资产及其演绎版。

>[!NOTE]
>
>所有用户现在都将默认启用&#x200B;**[!UICONTROL 快速下载]**，并要求在从Brand Portal下载资源之前，在其浏览器扩展中安装[IBM Aspera Connect 3.9.9](https://www.ibm.com/support/knowledgecenter/SSXMX3_3.9.9/kc/connect_welcome.html)。

<!--
If any of the **[!UICONTROL Custom Rendition]** or **[!UICONTROL System Rendition]** is enabled in the [**[!UICONTROL Download]**](brand-portal-download-assets.md) configuration and **[!UICONTROL Download]** settings are enabled for the group users, the new **[!UICONTROL Download]** dialog appears with all the renditions of the selected assets or folders containing assets in a list view. 
-->

从&#x200B;**[!UICONTROL 下载]**&#x200B;对话框中，用户可以：

* 视图下载列表中任何资产的所有可用演绎版。
* 不包括不需要下载的资产演绎版。
* 只需一次单击即可将同一组演绎版应用于所有类似资产类型。
* 对不同资产类型应用不同的演绎版集。
* 为每个资产创建单独的文件夹.
* 下载选定的资产及其演绎版。

对于独立资产、多个资产、包含资产的文件夹、授权或未授权的资产，以及使用共享链接下载资产，下载工作流程将保持不变。 请参阅[从Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets)下载资产的步骤。

![下载对话框](assets/download-dialog-box.png)

### 快速导航{#quick-navigation}

以前，视图&#x200B;**[!UICONTROL 文件]**、**[!UICONTROL 集合]**&#x200B;和&#x200B;**[!UICONTROL 共享链接]**&#x200B;的选项是隐藏的，用户每次要切换到其他视图，都需要多次单击。

在Brand Portal 2020.10.0中，用户可以使用快速导航链接从所有Brand Portal页面单击导航到&#x200B;**[!UICONTROL 文件]**、**[!UICONTROL 集合]**&#x200B;和&#x200B;**[!UICONTROL 共享链接]**。

![collection-navigation](assets/collection-navigation.png)

### 增强的再现面板{#rendition-panel}

以前，如果在&#x200B;**[!UICONTROL 下载]**&#x200B;配置中启用了任何&#x200B;**[!UICONTROL 自定义演绎版]**&#x200B;或&#x200B;**[!UICONTROL 系统演绎版]**，则用户只能在&#x200B;**[!UICONTROL 演绎版]**&#x200B;面板中视图原始资产及其演绎版。 此外，用户还必须下载所有资产演绎版，因为没有过滤器可以排除不需要的特定自定义或动态演绎版。

<!--
Earlier, if any of the custom or system renditions was enabled in the **[!UICONTROL Download]** settings, an additional **[!UICONTROL Download]** dialog appeared on clicking the **[!UICONTROL Download]** button wherein the user had to manually select the set of renditions (original asset, custom renditions, dynamic renditions) to download.
There was no filter to exclude specific custom or dynamic renditions which were not required for download.
-->

在Brand Portal 2020.10.0中，用户可以排除特定演绎版并直接从资产详细信息页面的演绎版面板](brand-portal-download-assets.md#download-assets-from-asset-details-page)下载选定的演绎版，而无需打开&#x200B;**[!UICONTROL 下载]**&#x200B;对话框。[


<!-- 
In Brand Portal 2020.10.0, direct download and exclude renditions features are introduced in the **[!UICONTROL Renditions]** panel on the asset details page. All the renditions (original asset, custom renditions, dynamic renditions) under the rendition panel are now associated with a check box and are enabled by default. 

The user can clear the check boxes to exclude the renditions which are not required for download. And can click on the **[!UICONTROL Download]** button in the **[!UICONTROL Renditions]** panel to directly download the selected set of renditions in a zip folder without having to open the **[!UICONTROL Download]** dialog.
-->

![再现 — 面板](assets/renditions-panel.png)


### 配置下载设置{#download-permissions}

除了现有的&#x200B;**[!UICONTROL 下载]**&#x200B;配置之外，Brand Portal管理员还可以配置不同用户组的设置以进行视图，并（或）从资产详细信息页面下载原始资产及其演绎版。

以管理员身份登录到您的Brand Portal租户，然后导航到&#x200B;**[!UICONTROL 工具]** > **[!UICONTROL 用户]**。

在&#x200B;**[!UICONTROL 用户角色]**&#x200B;页中，导航到&#x200B;**[!UICONTROL 组]**&#x200B;选项卡以配置用户组的视图和（或）下载设置。

以前，这些设置仅可用于限制组用户下载原始资产。

通过&#x200B;**[!UICONTROL 用户角色]**&#x200B;页面上的&#x200B;**[!UICONTROL 组]**&#x200B;选项卡，管理员可以配置视图和下载设置：

* 如果&#x200B;**[!UICONTROL 下载原始]**&#x200B;和&#x200B;**[!UICONTROL 下载演绎版]**&#x200B;设置都已打开，则选定组的用户可以视图并下载原始资产及其演绎版。
* 如果这两个设置都处于关闭状态，则用户只能视图原始资产。 资产演绎版对资产详细信息页面上的用户不可见。
* 如果只打开了&#x200B;**[!UICONTROL 下载原件]**&#x200B;设置，则用户只能从资产详细信息页面视图和下载原始资产。
* 如果仅&#x200B;**[!UICONTROL “下载演绎版”]**&#x200B;设置处于打开状态，则用户可以视图原始资产，但无法下载它。 但是，用户可以视图和下载资产演绎版。

请参阅[配置资产下载](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions)。

![视图-download-permission](assets/download-permissions.png)

>[!NOTE]
>
>如果将用户添加到多个组，并且其中一个组具有限制，则限制将适用于用户。


<!--
>Restrictions to access the original asset and their renditions do not apply to administrators even if they are members of restricted groups.
 >
 >The users can always download assets and their renditions from the repository using a `curl` request even if the download configurations are turned-off.
 >
-->

## 6.4.7 {#what-changed-in-647}中的变化

Brand Portal 6.4.7版本引入了文档查看器，增强了下载资产的体验，并包含了关键修复。 请参阅最新的[Brand Portal发行说明](brand-portal-release-notes.md)。

<!--
Brand Portal 6.4.7 release brings in the Document Viewer, leverages the Brand Portal administrators to configure asset download, and centers top customer requests. See latest [Brand Portal Release Notes](brand-portal-release-notes.md).
-->

### 文档查看器{#doc-viewer}

文档查看器增强了PDF查看体验。 在Brand Portal中查看PDF文件时，它提供的体验与Adobe Document Cloud类似。

以前，有限的选项可用于视图PDF文件。

借助文档查看器，Brand Portal用户现在可以选择视图页面、视图书签、搜索页面文本、放大、缩小、导航到上一页和下一页、切换到页面、适合窗口、适合屏幕以及隐藏或取消隐藏工具栏。

>[!NOTE]
>
>其他文档格式的查看体验保持不变。


![](assets/doc-viewer.png)

### 下载体验{#download-configurations}

改进了资产下载过程，在[从Brand Portal](brand-portal-download-assets.md)下载资产时，提供了简化的用户体验。

从Brand Portal下载资产的现有工作流不可避免地会出现&#x200B;**[!UICONTROL 下载]**&#x200B;对话框，其中包含多个可供选择的下载选项。

在Brand Portal 6.4.7中，Brand Portal管理员可以配置资产&#x200B;**[!UICONTROL 下载]**&#x200B;设置。 可用的配置有：
* **[!UICONTROL 快速下载]**
* **[!UICONTROL 自定义呈现版本]**
* **[!UICONTROL 系统呈现版本]**

Brand Portal管理员可以启用任何组合来配置资产下载。

<!--In Brand Portal 6.4.7, fast download, custom renditions, and system renditions are the three configurations available.-->

* 如果关闭了&#x200B;**[!UICONTROL 自定义演绎版]**&#x200B;和&#x200B;**[!UICONTROL 系统演绎版]**&#x200B;配置，则下载资产的原始演绎版时无需任何其他对话框，从而简化了Brand Portal用户的下载体验。

* 如果启用了任何&#x200B;**[!UICONTROL 自定义演绎版]**&#x200B;或&#x200B;**[!UICONTROL 系统演绎版]**，将显示&#x200B;**[!UICONTROL 下载]**&#x200B;对话框，并下载原始资产以及资产演绎版。 启用&#x200B;**[!UICONTROL 快速下载]**&#x200B;配置可加快下载过程。

根据配置，独立资产、多个资产、包含资产的文件夹、授权或未授权的资产以及使用共享链接下载资产的下载工作流程将保持不变。


## 6.4.6 {#what-changed-in-646}中的变化

在Brand Portal 6.4.6中，AEM Assets与Brand Portal之间的授权渠道已更改。 AEM Assets现在作为Cloud Service、AEM Assets 6.3及更高版本支持Brand Portal。 在AEM Assets 6.3及更高版本中，Brand Portal先前已通过旧版OAuth网关在经典UI中配置，该网关使用JWT令牌交换获取IMS访问令牌以进行授权。 AEM Assets现在通过Adobe Developer Console配置了Brand Portal，后者为您的Brand Portal租户购买IMS令牌以授权。

<!-- The steps to configure integration are different depending on your AEM version, and whether you are configuring for the first-time, or upgrading the existing integration:
-->

<!--
  
   | **AEM Version** |**New Integration** |**Upgrade Integration** |
|---|---|---|
| **AEM 6.5** |[Create new integration](../using/brand-portal-configure-integration-65.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-65.md#upgrade-integration-65) | 
| **AEM 6.4** |[Create new integration](../using/brand-portal-configure-integration-64.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-64.md#upgrade-integration-64) | 
| **AEM 6.3** |[Create new integration](../using/brand-portal-configure-integration-63.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-63.md#upgrade-integration-63) | 
| **AEM 6.2** |Contact Support |Contact Support | 

   -->

配置AEM Assets与Brand Portal的步骤因AEM版本而异，具体取决于您是首次配置还是升级现有配置：

<!--| **AEM Version** |**New Configuration** |**Upgrade Configuration** |
|---|---|---|
| **AEM 6.5 (6.5.4.0 and above)** |[Create configuration](../using/brand-portal-configure-integration-65.md) |[Upgrade configuration](../using/brand-portal-configure-integration-65.md#upgrade-integration-65) | 
| **AEM 6.4 (6.4.8.0 and above)** |[Create configuration](../using/brand-portal-configure-integration-64.md) |[Upgrade configuration](../using/brand-portal-configure-integration-64.md#upgrade-integration-64) | 
| **AEM 6.3 (6.3.3.8 and above)** |[Create configuration](../using/brand-portal-configure-integration-63.md) |[Upgrade configuration](../using/brand-portal-configure-integration-63.md#upgrade-integration-63) | 
| **AEM 6.2** |Contact Support |Contact Support | 
-->


<!-- AEM Assets configuration with Brand Portal on Adobe I/O is supported on:
* AEM 6.5.4.0 and above
* AEM 6.4.8.0 and above
* AEM 6.3.3.8 and above -->

| **AEM 版本** | **新配置** | **升级配置** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [创建配置](https://docs.adobe.com/content/help/zh-Hans/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5（6.5.4.0及更高版本）** | [创建配置](https://docs.adobe.com/content/help/zh-Hans/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升级配置](https://docs.adobe.com/content/help/zh-Hans/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4（6.4.8.0及更高版本）** | [创建配置](https://docs.adobe.com/content/help/zh-Hans/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升级配置](https://docs.adobe.com/content/help/zh-Hans/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3（6.3.3.8及更高版本）** | [创建配置](https://helpx.adobe.com/cn/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [升级配置](https://helpx.adobe.com/cn/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | 联系支持 | 联系支持 |

>[!NOTE]
>
>建议将您的AEM实例更新到最新的Service Pack。

请参阅最新的[Brand Portal发行说明](brand-portal-release-notes.md)。

请参阅[Brand Portal常见问题解答](brand-portal-faqs.md)。

## 6.4.5 {#what-changed-in-645}中的变化


Brand Portal 6.4.5 是一个功能版本，其主要是为 Brand Portal 用户（外部代理/团队）提供在不需要访问作者环境的情况下将内容上传到 Brand Portal 并发布到 AEM Assets 的功能。此功能在Brand Portal中称为&#x200B;**[资产来源补充](brand-portal-asset-sourcing.md)**，通过为用户提供双向机制来与全球分布的其他Brand Portal用户共享和贡献资产，将改善客户体验。

### Brand Portal 中的资产源 {#asset-sourcing-in-bp}

资产来源补充允许AEM用户（管理员/非管理员用户）使用额外的&#x200B;**资产贡献**&#x200B;属性创建新文件夹，确保创建的新文件夹可由Brand Portal用户打开以供资产提交。 这会自动触发一个工作流，该工作流会在新创建的&#x200B;**Contribution**&#x200B;文件夹中创建另外两个子文件夹，称为NEW和SHARED。

然后，AEM用户通过将应添加到贡献文件夹的资产类型的简报上传到&#x200B;**SHARED**&#x200B;文件夹来定义要求，以确保BP用户获得所需的参考信息。 然后，管理员可以在将新创建的&#x200B;**Contribution**&#x200B;文件夹发布到Brand Portal之前，向活动的Brand Portal用户授予对贡献文件夹的访问权限。


用户在&#x200B;**NEW**&#x200B;文件夹中添加完内容后，可以将贡献文件夹发布回AEM作者环境。 请注意，完成导入并反映AEM Assets中新发布的内容可能需要几分钟时间。

此外，所有现有功能都保持不变。 Brand Portal用户可以从贡献文件夹以及其他允许的文件夹中视图、搜索和下载资产。 此外，管理员还可以进一步共享贡献文件夹、修改属性以及向收藏集添加资产。

>[!NOTE]
>
>AEM 6.5.2.0及更高版本支持品牌门户中的资产来源补充。
>
>早期版本不支持此功能 — AEM 6.3和AEM 6.4。

### 将资产上传到贡献文件夹{#upload-assets-in-bp}

拥有适当权限的Brand Portal用户可以下载资产要求，以了解贡献的需要，并将包含多个资产或文件夹的多个资产或文件夹上传到贡献文件夹。 但是，请注意，Brand Portal用户只能将资产上传到&#x200B;**NEW**&#x200B;子文件夹。 **SHARED**&#x200B;文件夹用于分配要求和基准资产。

![](assets/upload-asset6.png)

![](assets/upload-asset4.png)


### 将贡献文件夹发布到AEM Assets {#publish-assets-to-aem}

上传完成到&#x200B;**NEW**&#x200B;文件夹后，Brand Portal用户随后可以将贡献文件夹发布回AEM。 在AEM Assets中导入和反映已发布的内容/资产可能需要几分钟的时间。 请参阅[将贡献文件夹发布到AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)


![](assets/upload-asset5.png)

## 6.4.4 {#what-changed-in-644}中的变化

Brand Portal 6.4.4 版主要增强了文本搜索和常见客户请求。请参阅最新的[Brand Portal发行说明](brand-portal-release-notes.md)。

### 搜索增强功能

从Brand Portal 6.4.4开始，支持对筛选窗格中的属性谓词进行部分文本搜索。 要允许部分文本搜索，您需要在搜索表单的属性谓词中启用&#x200B;**部分搜索**。

阅读以了解有关部分文本搜索和通配符搜索的更多信息。

#### 部分短语搜索{#partial-phrase-search}

现在，您可以通过在筛选窗格中仅指定搜索的短语的一个部分（即一两个单词）来搜索资源。

**使用**
案例部分短语搜索在您不确定搜索的短语中出现的词语的确切组合时很有帮助。

例如，如果您在Brand Portal中的搜索表单使用属性谓词对资产标题进行部分搜索，则指定术语&#x200B;**camp**&#x200B;将返回标题短语中带有单词camp的所有资产。

![](assets/partialphrasesearch.png)

#### 通配符搜索{#wildcard-search}

Brand Portal允许在搜索查询中使用星号(*)，并在搜索的短语中使用部分单词。

**用**
例如果您不确定搜索的短语中出现的确切词语，可使用通配符搜索来填补搜索查询中的空白。

例如，如果品牌门户中的搜索表单使用属性谓词对资产标题进行部分搜索，则指定&#x200B;**climb***&#x200B;将返回所有包含以其标题短语中的字符&#x200B;**climb**&#x200B;开头的字词的资产。

![](assets/wildcard-prop.png)

同样，指定：

* ***** 爬升返回所有单词以字符结尾的资 **** 产，爬升其标题短语。

* ***climb*返** 回所有包含字符的资产，这些字符 **** 在其标题短语中。

>[!NOTE]
>
>在选中&#x200B;**部分搜索**&#x200B;复选框时，默认情况下会选中&#x200B;**忽略大小写**。

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-searching.md#facetedsearchbyapplyingfilterstosearch)

## 6.4.3 {#what-changed-in}中的更改

Brand Portal 6.4.3版本重点介绍 — 除了在Brand Portal访问URL中的租户ID外，为组织提供替代别名、新文件夹层次结构配置、视频支持增强、从AEM作者实例到Brand Portal的计划发布、操作增强 — 以及迎合客户请求。

### 非管理员的文件夹层次结构导航

管理员现在可以配置在登录时向非管理员用户（编辑者、查看者和客人用户）显示文件夹的方式。 [“启用文](../using/brand-portal-general-configuration.md) 件夹层次配置”将添 **加到“常规设**&#x200B;置”中的“管理工具”面板中。如果配置为：

* **启用**&#x200B;后，非管理员用户将看到从根文件夹开始的文件夹树。因此，可授予他们类似于管理员的导航体验。
* **禁用**，则登陆页上仅显示共享文件夹。

![](assets/enable-folder-hierarchy.png)

[启用文件夹层次结构](../using/brand-portal-general-configuration.md)功能（启用后）可帮助您区分从不同层次结构共享的同名文件夹。 登录时，非管理员用户现在可以看到共享文件夹的虚拟父（和祖级）文件夹。

![](assets/disabled-folder-hierarchy1-2.png)

![](assets/enabled-hierarchy1-2.png)

共享文件夹在虚拟文件夹的各个目录中进行组织。 您可以通过锁定图标识别这些虚拟文件夹。

请注意，虚拟文件夹的默认缩略图是第一个共享文件夹的缩略图。

![](assets/hierarchy1-nonadmin-2.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-general-configuration.md)

### 在特定文件夹层次结构或路径中搜索

**路径** 浏览器谓词已在搜索表单中引入，允许搜索特定目录中的资产。路径浏览器的搜索谓词的默认搜索路径为`/content/dam/mac/<tenant-id>/`，可通过编辑默认搜索表单来配置此路径。

* 管理员用户可以使用路径浏览器导航到Brand Portal上的任意文件夹目录。
* 非管理员用户可以使用路径浏览器仅导航到与他们共享的文件夹（并导航回父文件夹）。

   例如，`/content/dam/mac/<tenant-id>/folderA/folderB/folderC`与非管理员用户共享。 用户可以使用路径浏览器在folderC内搜索资产。 此用户还可以导航到folderB和folderA（因为它们是与用户共享的folderC的祖先）。

![](assets/edit-search-form.png)


您现在可以限制在已浏览到的特定文件夹中搜索资产，而不是从根文件夹开始。

请注意，在这些文件夹下进行搜索只会返回已与用户共享的资产的结果。

![](assets/filter-panel.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-search-facets.md#listofsearchpredicates)

### Dynamic Media视频再现支持

AEM作者实例处于Dynamic Media混合模式的用户除了可以下载原始视频文件外，还可以预览和下载Dynamic Media演绎版。

要允许预览和下载特定租户帐户上的Dynamic Media再现，管理员需要从管理工具面板中指定&#x200B;**Video**&#x200B;配置中的&#x200B;**Dynamic Media Configuration**(视频服务URL(DM-Gateway URL)和注册ID以获取动态视频)。


Dynamic Media视频可在以下位置预览：

* 资产详细信息页面
* 资产的卡视图
* 链接共享预览页

Dynamic Media视频编码可从以下位置下载：

* Brand Portal
* 共享链接

![](assets/edit-dynamic-media-config.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### 计划发布到Brand Portal

可以安排将资产（和文件夹）发布工作流从[AEM(6.4.2.0)](https://helpx.adobe.com/experience-manager/6-4/release-notes/sp-release-notes.html#main-pars_header_9658011)创作实例发布到Brand Portal，以后的日期和时间。

同样，通过计划从Brand Portal中取消发布工作流，可以在以后（时间）从门户中删除已发布的资产。

![](assets/schedule-publish.png)

![](assets/publishlater-workflow.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### URL中的可配置租户别名

组织可以通过在URL中具有替代前缀来自定义其门户URL。 要在其现有门户URL中获取租户名称的别名，组织需要联系Adobe支持。

请注意，只能自定义品牌门户URL的前缀，而不能自定义整个URL。\
例如，具有现有域&#x200B;**geometrix.brand-portal.adobe.com**&#x200B;的组织可以获取根据请求创建的&#x200B;**geomettrixinc.brand-portal.adobe.com**。

但是，AEM作者实例只能[配置](https://helpx.adobe.com/cn/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html)（仅使用租户ID URL），而不能使用租户别名（备用）URL。

组织可以通过自定义门户URL而不是坚持Adobe提供的URL来满足其品牌需求。

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### 下载体验增强功能

发行版优惠通过减少点击次数和警告次数简化了下载体验，具体内容如下：

* 选择仅下载演绎版（而非原始资产）。
* 当访问原始演绎版受到限制时，请下载资产。

## 6.4.2 {#what-changed-in-1}中的变化

Brand Portal 6.4.2版本提供了一系列功能，可满足组织的资产分发需求，并帮助他们接触通过访客访问和最佳下载体验在全球分发的大量用户。 Brand Portal还通过新的管理员配置、新添加的报告以及迎合客户请求，为组织提供更大的控制力。

### 客人访问

![](assets/bp-login-screen-1.png)

AEM Brand Portal允许客人访问门户。 客人用户不需要凭据即可进入门户，并可以访问和下载所有公共文件夹和集合。 客人用户可以将资产添加到其Lightbox（私人收藏集）并下载相同的资产。 他们还可以视图由管理员设置的智能标记搜索和搜索谓词。 客人会话不允许用户创建收藏集和保存的搜索，也不允许用户进一步共享这些搜索、访问文件夹和收藏集设置以及将资产共享为链接。

在组织中，允许多个并发来宾会话，此会话仅限于每个组织用户配额总额的10%。

客人会话保持活动状态2小时。 因此，灯箱的状态也会保留到会话开始时间后的两小时。 两小时后，来宾会话必须重新启动，因此lightbox状态将丢失。

### 加速下载

Brand Portal用户可以利用基于IBM Aspera Connect的快速下载，将下载速度提高25倍，并享受无缝下载体验，无论他们身处全球。 要从Brand Portal或共享链接更快地下载资源，用户需要在下载对话框中选择&#x200B;**启用下载加速**&#x200B;选项，前提是组织中启用了下载加速。

![](assets/donload-assets-dialog-2.png)

要为组织启用基于IBM Aspera的加速下载，管理员可从“管理工具”面板中的[“常规设置”中&#x200B;**“启用下载加速**”选项（默认情况下为禁用）。 ](brand-portal-general-configuration.md#allow-download-acceleration)要进一步了解从Brand Portal和共享链接更快下载资源文件的先决条件和疑难解答步骤，请参阅[指南以加快从Brand Portal](../using/accelerated-download.md#main-pars-header)的下载。

### 用户登录报告

新的报告已引入，用于跟踪用户登录。 **用户登录**&#x200B;报告有助于使组织能够审核和检查委派的管理员和品牌门户的其他用户。

在生成报告之前，报表会从Brand Portal 6.4.2部署中记录每个用户的显示姓名、电子邮件ID、角色（管理员、查看器、编辑者、客人）、用户组、上次登录、活动状态和登录计数。 管理员可以将报告导出为.csv。 “用户登录”报表与其他报表一起使组织能够更密切地监视用户与已批准品牌资源的交互，从而确保符合公司合规办公室的要求。

![](assets/user-logins-1.png)

### 访问原始演绎版

管理员可以限制用户访问原始图像文件(.jpeg、.tiff、.png、.bmp、.gif、.pjpeg、x-portable-anymap、x-portable-bitmap、x-portable-graymap、x-portable-pixmap、x-rgbitmap、x-icon、x-photoshop、.psd、image/vnd.adobe.photoshop)再现（从Brand Portal或共享链接下载）。 此访问可以在“管理工具”面板中“用户角色”页面的“组”选项卡的用户组级别控制。

![](assets/access-original-rend-1.png)

* 默认情况下，所有用户都可以下载原始演绎版，因为“访问原稿”已为所有用户启用。
* 管理员需要取消选择相应的复选框以阻止一组用户访问原始演绎版。
* 如果用户是多个用户组的成员，但只有其中一个用户组具有限制，则这些限制适用于该用户。
* 这些限制不适用于管理员，即使管理员是受限组的成员。
* 将资产共享为链接的用户的权限适用于使用共享链接下载资产的用户。

### 卡和列表视图上的文件夹层次结构路径

文件夹卡现在在卡片视图中向非管理员用户（编辑者、查看者和客人用户）显示文件夹层次结构信息。 此功能可让用户了解文件夹的位置，以及他们访问的与父层次结构相关的文件夹。

文件夹层次结构信息对于区分名称与从其他文件夹层次结构共享的其他文件夹相似的文件夹特别有用。 如果非管理员用户不知道与他们共享的资产的文件夹结构，则名称相似的资产/文件夹似乎会令人混淆。

* 相应卡上显示的路径会截断以适合卡大小。 但是，用户在将鼠标悬停在截断路径上方时可以将完整路径视为工具提示。

![](assets/folder-hierarchy1-1.png)

列表视图显示列中资产到Brand Portal所有用户的文件夹路径。

![](assets/list-view-1.png)

### 视图资产属性的概述选项

Brand Portal为非管理员用户（编辑者、查看者、客人用户）提供“概述”选项，以视图选定资产/文件夹的资产属性。 “概述”选项可见：

1. 在顶部的工具栏中，选择资产/文件夹。
2. 在下拉菜单中，选择边栏选择器。

在选择资产/文件夹时选择“概述”选项后，用户可以查看资产创建的标题、路径和时间。 但是，在资产详细信息页面上，选择“概述”选项后，用户可以查看资产的元数据。

![](assets/overview-option-2.png)

![](assets/overview-rail-selector-2.png)

## 新配置

为管理员添加了六种新配置，以针对特定租户启用/禁用以下功能：

* 允许来宾访问
* 允许用户请求访问Brand Portal
* 允许管理员从Brand Portal中删除资产
* 允许创建公共集合
* 允许创建公共智能集合
* 允许下载加速

以上配置位于管理工具面板中的“访问”和“常规”设置下。

![](assets/access-configs-1.png)
![](assets/general-configs-1.png)
![](assets/admin-tools-panel-13.png)

### Adobe I/OUI配置Auth集成

从Brand Portal 6.4.2开始，使用Adobe.io [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/)接口创建JWT应用程序，这允许配置Auth集成以允许AEM Assets与Brand Portal集成。 以前，用于配置OAuth集成的UI托管在`https://marketing.adobe.com/developer/`中。 要了解有关将AEM Assets与Brand Portal集成以将资产和集合发布到Brand Portal的更多信息，请参阅[配置AEM Assets与Brand Portal的集成](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html)。

## 搜索增强功能

管理员可以使用更新的属性谓词使属性谓词不区分大小写，该谓词已选中“忽略大小写”。 此选项可用于属性谓词和多值属性谓词。\
但是，非区分大小写的搜索比默认属性谓词搜索速度要慢。 如果搜索筛选器中存在太多非区分大小写的谓词，则搜索可能会减慢。 因此，建议审慎地使用非区分大小写的搜索。

## 6.4.1 {#what-changed-in-2}中的更改

Brand Portal 6.4.1是一个平台升级版本，它引入了多项新功能和重要增强功能，如浏览、搜索和性能增强，可提供充分的客户体验。

### 浏览增强功能

* 新建内容树边栏可快速导航资产层次结构。

![](assets/contenttree-2.png)

* 引入了新的键盘快捷键，例如&#x200B;_(p)_（用于导航到属性页面）、_(e)_（用于编辑）和&#x200B;_(ctrl+c)_（用于复制操作）。
* 改进了在卡和列表视图中滚动、延迟加载体验，以浏览大量资源。
* 增强的卡视图，支持基于视图设置的不同大小的卡。

![](assets/cardviewsettings-1.png)

* 卡视图现在可在将鼠标悬停在日期标签上方时显示日期/时间戳。

* 增强的列视图，其中&#x200B;**资产快照下的更多详细信息**，允许您导航到资产的详细信息页面。

![](assets/columnmoredetail.png)

* 列表视图现在默认显示第一列中资产的文件名，以及区域设置、资产类型、尺寸、大小、评级和发布信息。 新的&#x200B;**视图设置**&#x200B;可用于配置要在列表视图中显示的详细信息量。

* 改进了资产详细信息体验，能够使用新的导航按钮和视图资产计数在资产之间来回导航。

![](assets/navbtn.png)

* 预览资产详细信息页面中从AEM上传的音频文件的新功能。
* 资产属性中提供的新相关资产功能。 与AEM上的其他源/派生资产相关并在Brand Portal上发布的资产现在可在Brand Portal中保持其关系，并在属性页面上提供相关资产的链接。
* 新增了限制非管理员用户创建公共集合的配置。 组织可以与Adobe支持团队合作，在特定帐户上配置此功能。

### 搜索增强功能

* 引入的功能可在导航到搜索项后返回到搜索结果中的同一位置，而无需再次运行搜索查询。
* 已提供新的搜索结果计数以显示搜索结果数。
* 改进的文件类型搜索筛选器，与早期的“图像”、“文档”、“多媒体”选项相比，能够根据细粒度的MIME类型(如.jpg、.png和.psd)筛选搜索结果。
* 增强了集合的搜索过滤器，具有准确的时间戳而不是以前的时间滑块功能。
* 新的“访问”类型过滤器已引入，用于搜索公开或非公开的集合。

![](assets/accesstypefilter.png)

### 下载优化

* 直接下载单个大文件，无需创建zip文件，从而提高了速度和吞吐量。
* 链接共享功能的Zip下载限制从1GB增加到5GB。

* 用户现在可以选择仅下载自定义和原始文件，防止开箱即用的再现，同时从Brand Portal或通过共享链接功能下载资产。

![](assets/excludeautorendition.png)

### 性能增强

* 资产下载速度提高100%。
* 资产搜索响应提高40%。
* 浏览性能提高40%。

**注意**:根据实验室进行的测试，有改进之处。

### 增强的报告功能

**引入链接共**
享报告已引入新报告，用于提供共享链接的相关信息。“链接共享”报表将所有URL列表到资产，并在指定的时间范围内与组织内的内部和外部用户共享。 它还会通知链接何时共享、由谁共享以及何时过期。

![](assets/navigatereport.png)

**修改了访问使用情况报表的入**
口点。使用情况报表现在与其他报表整合，现在可以从资产报表控制台中查看。要访问“资产报表”控制台，请从管理工具面板导航到**创建/管理报表**。

![](assets/accessassetreport.png)

**通过Brand Portal上的reportingReporting界**
面改进的用户体验变得更直观，对组织实现了更大的控制。管理员现在除了创建各种报告外，还可以重新访问生成的报告并下载或删除它们，因为这些报告保存在Brand Portal中。

可通过添加或删除默认列来自定义所创建的每个报告。 此外，可向“下载”、“过期”和“发布”报表添加自定义列，以控制其粒度。

### 改进的管理工具

改进了“管理工具”中的属性选取器，可用于元数据、搜索和报表，并具有提前键入和浏览功能，可简化管理体验。

### 其他增强功能

* 现在，通过在AEM Assets Brand Portal复制对话框中标记公共文件夹发布复选框，可以将从AEM 6.3.2.1和6.4发布到Brand Portal的资产公开提供给Brand Portal的一般用户。

![](assets/public-folder-publish.png)

* 如果有人请求访问Brand Portal，则管理员会通过访问请求电子邮件获得通知，但Brand Portal通知区域中的通知除外。

## 6.3.2 {#what-changed-in-3}中的更改

Brand Portal 6.3.2包含面向热门客户请求的新增和增强功能以及一般性能增强。

### 请求访问Brand Portal {#request-access-to-brand-portal}

用户现在可以使用Brand Portal登录屏幕上新增的&#x200B;**需要访问**&#x200B;功能来请求对Brand Portal的访问。

![](assets/bplogin_request_access.png)

根据用户是否拥有Adobe ID或是否需要创建Adobe ID，用户可以按照相应的工作流提交请求。 Brand Portal产品管理员在其通知区域中接收此类请求并通过Adobe Admin Console授予访问权限。

有关详细信息，请参阅[请求访问Brand Portal](../using/brand-portal.md#requestaccesstobrandportal)。

### 资产下载报表{#enhancement-in-the-assets-downloaded-report}中的增强功能

资产下载报表现在包括指定日期和时间范围内每个用户的资产下载计数。 用户可以下载.csv格式的此报告并编译数据，如授权资产的总下载计数。

![](assets/reports_download_downloaded_by.png)

有关详细信息，请参阅[创建和管理其他报告](../using/brand-portal-reports.md#createandmanageadditionalreports)中的步骤3和步骤6。

### Brand Portal维护通知{#brand-portal-maintenance-notification}

现在，在即将进行的维护活动前几天，Brand Portal会显示通知横幅。 示例通知：

![](assets/bp_maintenance_notification-1.png)

有关详细信息，请参阅[品牌门户维护通知](https://helpx.adobe.com/experience-manager/brand-portal/using/brand-portal.html#BrandPortalmaintenancenotification)。

### 使用链接共享功能{#enhancement-for-licensed-assets-shared-using-the-link-share-feature}增强共享的许可资源

使用链接共享功能下载许可的资产时，现在会提示您同意这些资产的许可协议。

![](assets/copyright_management.png)

有关详细信息，请参阅[将资产共享为链接](../using/brand-portal-link-share.md#shareassetsasalink)中的步骤12。

### 用户拾取器增强{#user-picker-enhancement}

现在增强了用户选取器性能，以满足拥有大量用户群的客户的需求。

### Experience Cloud品牌变更{#experience-cloud-branding-changes}

Brand Portal现在符合新的Adobe Experience Cloud品牌。

![](assets/bp_solution_switcher.png)

## 6.3.1 {#what-changed-in-4}中的更改

Brand Portal 6.3.1包含面向将Brand Portal与AEM相协调的新增和增强功能。

### 升级的用户界面{#upgraded-user-interface}

要使Brand Portal用户体验与AEM保持一致，Adobe正在过渡到Coral 3用户界面。 此更改增强了整体可用性，包括导航和外观。

#### 增强的导航体验{#enhanced-navigational-experience}

* 通过新的Adobe徽标快速访问管理工具：

![](assets/aemlogo-3.png)

* 通过叠加进行产品导航：

![](assets/overlay_navigation.png)

* 快速导航到父文件夹：

![](assets/navigationparentfolders.png)

* 快速搜索和导航到所需的内容和工具：

![](assets/omnisearchicon.png)

### 增强的浏览体验{#enhanced-browsing-experience}

* 用于浏览嵌套文件夹的新列视图:

![](assets/millercolumnnavigation.png) ![](assets/multi-columnview.png)

* 在文件夹中资产的列表下，最新上传的资产会显示在顶部。

### 增强的搜索体验{#enhanced-search-experience}

* 全新的Omni搜索功能便于您在键入搜索关键字时通过自动建议快速访问相关内容、功能或标记。 Omni搜索功能适用于所有搜索功能。

![](assets/omnisearch_whatsnew.png)

* 您还可以向Omni搜索添加搜索过滤器，以进一步缩小搜索范围并加快搜索速度。

![](assets/omnisearch_withfilters.png)

* 通过基于资产评级的新搜索功能，您可以搜索包含评级的资产(如果是从AEM Assets发布的)。
* 新的多值搜索功能可通过AND运算符接受多个关键字以更快地搜索资源。
* 新的搜索提升功能可让您提高搜索相关性，以便特定资产显示在搜索结果的顶部。
* 利用新的基于路径的搜索功能，您可以提供嵌套文件夹的路径，以便能够搜索该文件夹中的资产。

#### 基于新智能标记的搜索{#new-smart-tags-based-search}

如果具有智能标记的图像从AEM Assets发布到Brand Portal，则可以在Brand Portal中使用智能标记名称作为搜索关键字搜索这些图像。 此功能仅对文件可用。

### 增强的下载体验{#enhanced-downloading-experience}

下载嵌套文件夹后，您可以保留原始文件夹层次结构。 嵌套文件夹中的资源可以通过单个文件夹下载，而不是通过单独的文件夹下载。

### 改进了性能{#improved-performance}

浏览、搜索和下载功能中的增强功能可显着提高Brand Portal的性能。

### 资产{#new-digital-rights-management-for-assets}的新数字版权管理

管理员可以在共享资产之前设置资产的到期日期和时间。 资产到期后，查看者和编辑者可以看到它，但无法下载。 当资产过期时，管理员会收到通知。

### 增强的资源排序{#enhanced-asset-sorting}

在列表视图下，对文件夹中的资产排序不再局限于在第一页上显示的资产数量。 文件夹中的所有资产都会进行排序，而不管是否在第一页中列出所有资产。

### 增强的报告{#reporting-capabilities}

管理员可以创建和管理三种类型的报告 — 已下载、过期和已发布的资产。 还可以配置报表中的列，并将报表导出为CSV格式。

![](assets/newreport.png)

### 其他元数据 {#additional-metadata}

Brand Portal 6.3.1引入了其他元数据，这与AEM Assets 6.3相同。您可以使用模式编辑器表单控制应在“资产属性”页面上可见的元数据。 外部链接共享用户看不到资产元数据，他们只能使用链接共享URL预览和下载资产。

![](assets/additionsinmetadata.png)

### 管理员{#additional-capabilities-for-administrators}的其他功能

* 在完成对登录屏幕墙纸的自定义之前，管理员可以预览更改。

![](assets/wallpaperpreview.png)

* 管理员添加新用户后，无需接受添加到Brand Portal的邀请即会自动添加这些用户。

### AEM Assets 6.3 {#new-publishing-capabilities-in-aem-assets}中的新发布功能

* AEM管理员可以使用AEM 6.3 SP 1-CFP 1(6.3.1.1)将元数据模式从AEM Assets发布到Brand Portal，该功能将于2017年第4季度推出。

![](assets/publish_metadataschemaaemassets.png)

* AEM管理员可以使用AEM 6.2 SP1-CFP7和AEM 6.3 SP 1-CFP 1(6.3.1.1)将所有标签从AEM Assets发布到Brand Portal。

![](assets/publish_tags_aemassets.png)

* 从AEM Assets，您可以发布具有标记（包括智能标记）的资产和收藏集。 然后，您可以在Brand Portal中使用这些标记作为搜索关键字搜索这些资产或收藏集。
