---
title: 上传资源并将贡献文件夹从Brand Portal发布到Experience Manager Assets
seo-title: Upload assets and publish the Contribution folder from Brand Portal to Experience Manager Assets
description: 深入了解如何上传新资源以及如何将贡献文件夹从Brand Portal发布到Experience Manager Assets。
seo-description: Get an insight into uploading new assets and publishing the contribution folder from Brand Portal to Experience Manager Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 7dcf445d-97ed-4fa5-959c-c4c48e325766
source-git-commit: 606f4389780025f5cf92b11bf8cac464e36be44a
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 0%

---

# 将贡献文件夹发布到Experience Manager Assets {#using-asset-souring-in-bp}

具有适当权限的Brand Portal用户可以将多个资源或包含多个资源的文件夹上传到contribution文件夹。 但是，Brand Portal用户只能将资源上传到 **新** 文件夹。 此 **已共享** 文件夹用于分发基线资源（参考内容），Brand Portal用户在创建新资源以进行贡献时可以使用该内容。

有权访问“贡献”文件夹的Brand Portal用户可以执行以下操作：

* [下载资源要求](#download-asset-requirements)
* [将新资产上传到贡献文件夹](#uplad-new-assets-to-contribution-folder)
* [将贡献文件夹发布到Experience Manager Assets](#publish-contribution-folder-to-aem)

## 下载资源要求 {#download-asset-requirements}

只要Brand Portal用户共享了“贡献”文件夹，Experience Manager Assets用户就会自动收到电子邮件/脉冲通知，以便他们可以从下载简短（资源要求）文档，以及下载基准资源（参考内容） **已共享** 文件夹，以确保他们了解资源要求。

Brand Portal用户会执行以下操作，以下载资源要求：

* **下载摘要**：下载附加到Contribution文件夹的摘要（资源要求文档），该文件夹包含与资源相关的信息，如资源类型、用途、支持的格式、最大资源大小等。
* **下载基线资源**：下载可用于了解所需资源类型的基线资源。 Brand Portal用户可以使用这些资源作为参考，为贡献创建新资源。

Brand Portal功能板反映了允许向Brand Portal用户发送的所有现有文件夹，以及新共享的贡献文件夹。 在此示例中，Brand Portal用户仅有权访问新创建的贡献文件夹，不会与用户共享任何其他现有文件夹。

**要下载资源要求，请执行以下操作：**

1. 登录到您的Brand Portal实例。
1. 从Brand Portal功能板中选择贡献文件夹。
1. 单击 **[!UICONTROL 属性]**. 此时将打开包含贡献文件夹详细信息的“属性”窗口。

   ![](assets/properties.png)

   ![](assets/download-asset-requirement2.png)

1. 单击 **[!UICONTROL 下载摘要]** 用于将资源要求文档下载到本地计算机上的选项。

   ![](assets/download.png)

1. 返回到Brand Portal功能板。
1. 单击以打开贡献文件夹，您可以看到两个子文件夹 — **[!UICONTROL 已共享]** 和 **[!UICONTROL 新]** 在贡献文件夹内。 “共享”文件夹包含管理员共享的所有基线资源（引用内容）。
1. 您可以下载 **[!UICONTROL 已共享]** 包含本地计算机上所有基线资产的文件夹。
或者，您可以打开 **[!UICONTROL 已共享]** 文件夹，然后单击 **下载** 图标来下载各个文件/文件夹。

   ![](assets/download.png)

   ![](assets/download-asset-requirement5.png)

浏览摘要（资产需求文档）并参考基准资产，以了解资产需求。 现在，您可以为贡献创建新资产，并将它们上传到贡献文件夹。


## 将资产上传到贡献文件夹 {#upload-new-assets-to-contribution-folder}

完成资源要求后，Brand Portal用户可以为贡献创建新资源，并将它们上传到contribution文件夹中的NEW文件夹。 用户可以将多个资产上传到资产贡献文件夹。 但是，一次只能创建一个文件夹。

>[!NOTE]
>
>Brand Portal用户可以上传资源（最多个） **2** GB（每个文件大小）。
>
>任何Brand Portal租户的最大上传限制为 **10**&#x200B;累积应用于所有贡献文件夹的GB。
>
>上传到Brand Portal的资源不会进行呈现处理，并且不包含预览。

>[!NOTE]
>
>建议在将贡献文件夹发布到Experience Manager Assets后释放上传空间，以便其他Brand Portal用户能够贡献内容。
>
>如果需要将Brand Portal租户的上传限制延长到 **10** GB，请联系客户支持部门指定要求。


**要上传新资产，请执行以下操作：**

1. 登录到您的Brand Portal实例。
Brand Portal功能板反映允许Brand Portal用户访问的所有现有文件夹以及新共享的贡献文件夹。

1. 选择贡献文件夹，然后单击以将其打开。 贡献文件夹包含两个子文件夹 —  **[!UICONTROL 已共享]** 和 **[!UICONTROL 新]**.

1. 单击 **[!UICONTROL 新]** 文件夹。

   ![](assets/upload-new-assets4.png)

1. 单击 **[!UICONTROL 创建]** > **[!UICONTROL 文件]** 上传单个文件或包含多个资产的文件夹(.zip)。

   ![](assets/upload-new-assets5.png)

1. 浏览资产（文件或文件夹）并将其上传到 **[!UICONTROL 新]** 文件夹。

   ![](assets/upload-asset4.png)

将所有资源或文件夹上传到NEW文件夹后，将贡献文件夹发布到Experience Manager Assets。


## 将贡献文件夹发布到Experience Manager Assets {#publish-contribution-folder-to-aem}

Brand Portal用户可以将contribution文件夹发布到Experience Manager Assets，而无需访问Experience Manager创作实例。

确保您已满足资产要求，并将新创建的资产上传到 **新** “贡献”文件夹中的文件夹。

**要发布贡献文件夹，请执行以下操作：**

1. 登录到您的Brand Portal实例。

1. 从Brand Portal功能板中选择贡献文件夹。
1. 单击 **[!UICONTROL 发布到AEM]**.

   ![](assets/export.png)

   ![](assets/publish-contribution-folder-to-aem1.png)

在发布工作流的不同阶段，会向Brand Portal用户和管理员发送电子邮件/脉冲通知：

1. **已排队**  — 当Brand Portal中触发发布工作流时，会向Brand Portal用户和Brand Portal管理员发送通知。

1. **完成**  — 当贡献文件夹成功发布到Experience Manager Assets时，会向Brand Portal用户和Brand Portal管理员发送通知。

将新创建的资产发布到Experience Manager Assets后，Brand Portal用户可以从“新建”文件夹中删除这些资产。 但是，Brand Portal管理员可以从NEW和SHARED文件夹中删除资源。

一旦实现了创建贡献文件夹的目标，Brand Portal管理员可以删除贡献文件夹，以释放上传空间给其他用户。

## 发布作业状态 {#publishing-job-status}

管理员可以使用两个报表来查看从Brand Portal发布到Experience Manager Assets的资源贡献文件夹的状态。

* 在Brand Portal中，导航到 **[!UICONTROL 工具]** > **[!UICONTROL 资产贡献状态]**. 此报表反映发布工作流不同阶段的所有发布作业的状态。

   ![](assets/contribution-folder-status-v2.png)

* 在Experience Manager Assets（内部部署或托管服务）中，导航到 **[!UICONTROL 资产]** > **[!UICONTROL 作业]**. 此报表反映所有发布作业的最终状态（成功或错误）。

   ![](assets/publishing-status.png)

* 在Experience Manager Assetsas a Cloud Service中，导航到 **[!UICONTROL 资产]** > **[!UICONTROL 作业]**.

   或者，您可以直接导航到 **[!UICONTROL 作业]** 从全局导航中。

   此报表反映所有发布作业的最终状态（成功或错误），包括从Brand Portal将资源导入Experience Manager Assetsas a Cloud Service。

   ![](assets/cloud-service-job-status.png)

<!--
>[!NOTE]
>
>Currently, no report is generated in AEM Assets as a Cloud Service for the Asset Sourcing workflow. 
-->

## 从Contribution文件夹中自动删除发布到Experience Manager Assets的资源 {#automatically-delete-published-assets-from-contribution-folder}

Brand Portal现在每十二小时执行一次自动作业，以扫描所有Contribution文件夹并删除发布到AEM的所有资源。 因此，您无需手动删除Contribution文件夹中的资产，即可将文件夹大小保持在 [阈值限制](#upload-new-assets-to-contribution-folder). 您还可以监视在过去七天内自动执行的删除作业的状态。 作业的报表提供以下详细信息：

* 作业开始时间
* 作业结束时间
* 作业状态
* 作业中包含的资产总数
* 在作业中成功删除的资产总数
* 作为作业运行结果提供的总存储空间

   ![删除报告](assets/deletion-reports.png)

您还可以进一步细化以查看删除作业中包含的每个资源的详细信息。 资产标题、大小、作者、删除状态和删除时间等详细信息将包含在报表中。

![详细删除报告](assets/deletion-reports-detailed.png)

>[!NOTE]
>
> * 客户可以请求Adobe客户支持禁用和重新启用自动删除作业功能，或者更改其执行频率。
> * 此功能在Experience Manager6.5.13.0及更高版本中可用。


### 查看和下载删除报告 {#view-delete-jobs}

要查看和下载删除作业的报告，请执行以下操作：

1. 在Brand Portal中，导航到 **[!UICONTROL 工具]**>**[!UICONTROL 资产贡献状态]**>**[!UICONTROL 删除报告]** 选项。

1. 选择作业并单击 **[!UICONTROL 视图]** 以查看报表。

   查看删除作业中包含的每个资源的详细信息。 资产标题、大小、作者、删除状态和删除时间等详细信息将包含在报表中。 单击 **[!UICONTROL 下载]** 以CSV格式下载作业的报告。

   报表中资产的删除状态可能具有以下值：

   * **已删除**  — 已成功从“贡献”文件夹中删除资产。

   * **未找到** - Brand Portal在“贡献”文件夹中找不到资产。 已手动从文件夹中删除资产。

   * **已跳过** - Brand Portal已跳过资源删除，因为Contribution文件夹中的资源有新版本可用，但该版本尚未发布到Experience Manager。

   * **失败** - Brand Portal无法删除资源。 有三次重试尝试删除具有的资产 `Failed` 删除状态。 如果资产第三次重试删除尝试失败，您需要手动删除资产。

### 删除报表

Brand Portal还允许您选择一个或多个报表并手动删除它们。

要删除报表，请执行以下操作：

1. 导航到 **[!UICONTROL 工具]**>**[!UICONTROL 资产贡献状态]**>**[!UICONTROL 删除报告]** 选项。

1. 选择一个或多个报告并单击 **[!UICONTROL 删除]**.


