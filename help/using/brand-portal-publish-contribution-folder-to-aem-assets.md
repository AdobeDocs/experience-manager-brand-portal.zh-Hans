---
title: 将资产从Brand Portal上传并将Contribution文件夹发布到Experience Manager Assets
seo-title: Upload assets and publish the Contribution folder from Brand Portal to Experience Manager Assets
description: 深入了解上传新资产并将贡献文件夹从Brand Portal发布到Experience Manager Assets。
seo-description: Get an insight into uploading new assets and publishing the contribution folder from Brand Portal to Experience Manager Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 7dcf445d-97ed-4fa5-959c-c4c48e325766
source-git-commit: 443ead94da2f253e28c438f1238a4667ca0d5d29
workflow-type: tm+mt
source-wordcount: '1053'
ht-degree: 0%

---

# 将贡献文件夹发布到Experience Manager Assets {#using-asset-souring-in-bp}

具有相应权限的Brand Portal用户可以将多个资产或包含多个资产的文件夹上传到“贡献”文件夹。 但是，Brand Portal用户只能将资产上传到 **新建** 文件夹。 的 **共享** 文件夹用于分发基线资产（参考内容），Brand Portal用户在创建新资产以进行贡献时可使用该基线资产。

Brand Portal用户（具有访问贡献文件夹的权限）可以执行以下活动：

* [下载资产要求](#download-asset-requirements)
* [将新资产上传到贡献文件夹](#uplad-new-assets-to-contribution-folder)
* [将贡献文件夹发布到Experience Manager Assets](#publish-contribution-folder-to-aem)

## 下载资产要求 {#download-asset-requirements}

Brand Portal用户在Experience Manager Assets用户共享贡献文件夹时会自动收到电子邮件/脉冲通知，以便他们能够从以下位置下载简要（资产要求）文档以及下载基线资产（参考内容）： **共享** 文件夹，以确保他们了解资产要求。

Brand Portal用户可通过执行以下活动来下载资产要求：

* **下载摘要**:下载附加到贡献文件夹的简短（资产要求文档），其中包含与资产相关的信息，如资产类型、用途、支持的格式、最大资产大小等。
* **下载基准资产**:下载可用于了解所需资产类型的基准资产。 Brand Portal用户可以将这些资产用作参考，以创建新资产供贡献。

Brand Portal功能板反映允许Brand Portal用户使用的所有现有文件夹以及新共享的贡献文件夹。 在此示例中，Brand Portal用户只能访问新创建的贡献文件夹，不会与用户共享任何其他现有文件夹。

**要下载资产要求，请执行以下操作：**

1. 登录到Brand Portal实例。
1. 从Brand Portal功能板中选择Contribution文件夹。
1. 单击&#x200B;**[!UICONTROL 属性]**. 此时将打开包含贡献文件夹详细信息的属性窗口。

   ![](assets/properties.png)

   ![](assets/download-asset-requirement2.png)

1. 单击 **[!UICONTROL 下载摘要]** 选项，在本地计算机上下载资产要求文档。

   ![](assets/download.png)

1. 返回到Brand Portal仪表板。
1. 单击以打开贡献文件夹，您可以看到两个子文件夹 — **[!UICONTROL 共享]** 和 **[!UICONTROL 新建]** 中。 SHARED文件夹包含管理员共享的所有基线资产（引用内容）。
1. 您可以下载 **[!UICONTROL 共享]** 包含本地计算机上所有基线资产的文件夹。
或者，您可以打开 **[!UICONTROL 共享]** 文件夹，然后单击 **下载** 图标下载单个文件/文件夹。

   ![](assets/download.png)

   ![](assets/download-asset-requirement5.png)

阅读简介（资产要求文档），并参考基准资产，以了解资产要求。 现在，您可以创建新资产以进行贡献，并将其上传到贡献文件夹。


## 将资产上传到贡献文件夹 {#uplad-new-assets-to-contribution-folder}

完成资产要求后，Brand Portal用户可以创建新资产以进行贡献，并将其上传到贡献文件夹的NEW文件夹。 用户可以将多个资产上传到资产贡献文件夹。 但是，一次只能创建一个文件夹。

>[!NOTE]
>
>Brand Portal用户可以上传资产(最大 **2** GB（每个文件大小）转到新文件夹。
>
>任何Brand Portal租户的上载上限均为 **10** GB，用于累计应用于所有贡献文件夹。
>
>上传到Brand Portal的资产不会进行演绎版处理，也不会包含预览。

>[!NOTE]
>
>建议在将贡献文件夹发布到Experience Manager Assets后释放上传空间，以便其他Brand Portal用户可以使用该文件夹进行贡献。
>
>如果需要将Brand Portal租户的上载限制扩展到 **10** GB，请联系客户支持部门以指定要求。


**要上传新资产，请执行以下操作：**

1. 登录到Brand Portal实例。
Brand Portal功能板反映允许Brand Portal用户使用的所有现有文件夹以及新共享的贡献文件夹。

1. 选择贡献文件夹，然后单击以将其打开。 贡献文件夹包含两个子文件夹 —  **[!UICONTROL 共享]** 和 **[!UICONTROL 新建]**.

1. 单击 **[!UICONTROL 新建]** 文件夹。

   ![](assets/upload-new-assets4.png)

1. 单击 **[!UICONTROL 创建]** > **[!UICONTROL 文件]** 上传包含多个资产的单个文件或文件夹(.zip)。

   ![](assets/upload-new-assets5.png)

1. 浏览资产（文件或文件夹）并将其上传到 **[!UICONTROL 新建]** 文件夹。

   ![](assets/upload-asset4.png)

将所有资产或文件夹上传到NEW文件夹后，将Contribution文件夹发布到Experience Manager Assets。


## 将贡献文件夹发布到Experience Manager Assets {#publish-contribution-folder-to-aem}

Brand Portal用户可以将贡献文件夹发布到Experience Manager Assets，而无需访问Experience Manager创作实例。

确保您已完成资产要求，并且已在 **新建** 文件夹中。

**要发布贡献文件夹，请执行以下操作：**

1. 登录到Brand Portal实例。

1. 从Brand Portal功能板中选择Contribution文件夹。
1. 单击 **[!UICONTROL 发布到AEM]**.

   ![](assets/export.png)

   ![](assets/publish-contribution-folder-to-aem1.png)

将在发布工作流程的不同阶段向Brand Portal用户和管理员发送电子邮件/脉冲通知：

1. **已排队**  — 在Brand Portal中触发发布工作流程时，会向Brand Portal用户和Brand Portal管理员发送通知。

1. **完成**  — 将贡献文件夹成功发布到Brand Portal时，系统会向Experience Manager Assets用户和Brand Portal管理员发送通知。

将新创建的资产发布到Experience Manager Assets后，Brand Portal用户可以从NEW文件夹中删除这些资产。 然而，Brand Portal管理员可以从NEW文件夹和SHARED文件夹中删除资产。

实现创建贡献文件夹的目标后，Brand Portal管理员可以删除贡献文件夹，以便为其他用户释放上传空间。

## 发布作业状态 {#publishing-job-status}

管理员可以使用两个报表来查看从Brand Portal发布到Experience Manager Assets的资产贡献文件夹的状态。

* 在Brand Portal中，导航到 **[!UICONTROL 工具]** > **[!UICONTROL 资产贡献状态]**. 此报表反映发布工作流程不同阶段的所有发布作业的状态。

   ![](assets/contribution-folder-status.png)

* 在Experience Manager Assets（内部部署或托管服务）中，导航到 **[!UICONTROL 资产]** > **[!UICONTROL 作业]**. 此报表反映所有发布作业的最终状态（成功或错误）。

   ![](assets/publishing-status.png)

* 在Experience Manager Assetsas a Cloud Service中，导航到 **[!UICONTROL 资产]** > **[!UICONTROL 作业]**.

   或者，您也可以直接导航到 **[!UICONTROL 作业]** 中。

   此报表反映所有发布作业的最终状态（成功或错误），包括将资产从Brand Portal导入Experience Manager Assetsas a Cloud Service。

   ![](assets/cloud-service-job-status.png)

<!--
>[!NOTE]
>
>Currently, no report is generated in AEM Assets as a Cloud Service for the Asset Sourcing workflow. 
-->
