---
title: 使用报告
seo-title: Work with reports
description: Experience Manager Assets Brand Portal管理员可以查看有关Brand Portal使用情况的报告，以及创建、管理和查看有关已下载、已过期、已发布和通过Brand Portal共享的链接的资源的报告。
seo-description: Experience Manager Assets Brand Portal Administrators can view report about Brand Portal usage, and create, manage, and view reports around assets downloaded, expired, published, and link shared through Brand Portal.
uuid: dc4e5275-a614-4b95-8c70-2b7e470c50a7
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 7683074f-b6ea-42e0-a411-3b13eb88d1f2
role: Admin
exl-id: 03d0292c-23c2-4ea0-9781-eb27768e6c33
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 2%

---

# 使用报告 {#work-with-reports}

报告功能有助于评估Brand Portal使用情况，并了解内部和外部用户如何与批准的资源进行交互。 管理员可以查看Brand Portal使用情况报表，此报表始终位于“资产报表”页面上。 但是，可以从“资产报表”页面生成和查看有关用户登录和通过链接共享的资产的已下载、已过期、已发布和资产报表。 这些报告有助于分析资产部署，从而让您获得关键成功指标以衡量组织内外的已批准资产采用情况。

报告管理界面非常直观，包括用于访问已保存报告的细粒度选项和控件。 您可以在“资产报表”页面中查看、下载或删除报表，该页面中列出了之前生成的所有报表。

## 查看报表 {#view-reports}

要查看报告，请执行以下步骤：

1. 从顶部的工具栏中，点按/单击Experience Manager徽标以访问管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击 **[!UICONTROL 创建/管理报告]** 打开 **[!UICONTROL 资产报表]** 页面。

   ![](assets/access-asset-reports.png)

1. 访问 **[!UICONTROL 使用情况]** 报告和其他生成的报告来自资产报告页面。

   >[!NOTE]
   >
   >使用情况报告是在Brand Portal中生成的默认报告。 无法创建或删除它。 但是，您可以创建、下载并删除“下载”、“过期”、“发布”、“链接共享”和“用户登录”报告。

   要查看报告，请单击报告链接。 或者，选择报表，然后点按/单击工具栏中的查看图标。

   **[!UICONTROL 使用情况报表]** 显示有关Brand Portal中活动的Brand Portal用户数、所有资源占用的存储空间以及资源总数的信息。 未分配给Admin Console中任何产品配置文件的Brand Portal用户被视为非活动用户，不会反映在 **[!UICONTROL 使用情况报表]**.
该报告还显示每个信息量度的允许容量。

   ![](assets/usage-report.png)

   **[!UICONTROL 用户登录]** 报告提供了有关登录到Brand Portal的用户的信息。 报表会显示从Brand Portal 6.4.2部署到生成报表期间每个用户的显示名称、电子邮件ID、角色（管理员、查看者、编辑者、来宾）、组、上次登录、活动状态和登录计数。

   ![](assets/user-logins.png)

   **[!UICONTROL 下载]** 报表列出了在特定日期和时间范围内下载的所有资源并提供了相关详细信息。

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >资产 **[!UICONTROL 下载]** 报表仅显示单独选择并从Brand Portal下载的资源。 如果用户下载了包含资产的文件夹，则报表不会显示该文件夹或文件夹中的资产。

   **[!UICONTROL 过期]** 报表会列出并详细描述在特定时间范围内过期的所有资产。

   ![](assets/expiration-report.png)

   **[!UICONTROL Publish]** 报表列出并提供了有关在指定时间范围内从Experience Manager Assets发布到Brand Portal的所有资源的信息。

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >发布报表不显示有关内容片段的信息，因为内容片段无法发布到Brand Portal。

   **[!UICONTROL 链接共享报表]** 列出在特定时间范围内通过来自Brand Portal界面的链接共享的所有资源。 此外，报告还会告知通过链接共享资产的时间、用户、链接的过期时间以及租户（以及与之共享资产链接的用户）的共享链接数量。 无法自定义链接共享报表的列。

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >链接共享报表不显示有权访问通过链接共享的资产或通过链接下载资产的用户。
   >
   >要通过共享链接跟踪下载，您需要在选择后生成下载报告 **[!UICONTROL 仅链接共享下载]** 选项于 **[!UICONTROL 创建报告]** 页面。 但是，在这种情况下，用户（下载者）是匿名的。

## 生成报告 {#generate-reports}

管理员可以生成和管理以下标准报告，生成后，这些报告将保存为 [已访问](../using/brand-portal-reports.md#main-pars-header) 稍后：

* 用户登录
* 下载
* 到期时间
* 发布
* 链接共享

可以自定义“下载”、“过期”和“发布”报告中的列以供查看。 要生成报表，请执行以下步骤：

1. 在顶部的工具栏中，点按/单击Experience Manager徽标以访问管理工具。

1. 在管理工具面板中，点按/单击 **[!UICONTROL 创建/管理报告]** 打开 **[!UICONTROL 资产报表]** 页面。

   ![](assets/asset-reports.png)

1. 在资产报表页面中，点按/单击&#x200B;**[!UICONTROL 创建]**。
1. 从 **[!UICONTROL 创建报告]** 页面，选择要创建的报表，然后点按/单击 **[!UICONTROL 下一个]**.

   ![](assets/crete-report.png)

1. 配置报表详细信息。 指定标题、描述、文件夹结构（需要运行报表并生成统计信息的位置）和日期范围 **[!UICONTROL 下载]**， **[!UICONTROL 过期]**、和 **[!UICONTROL Publish]** 报告。

   ![](assets/create-report-page.png)

   但是， **[!UICONTROL 链接共享报表]** 只需要标题、描述和日期范围参数。

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >报告标题中的特殊字符#和%在报告生成时将被连字符(-)替换。

1. 点按/单击 **[!UICONTROL 下一个]**，以配置下载、过期和发布报表的列。
1. 根据需要选中或取消选中相应的复选框。 例如，在中查看用户（已下载资产）的名称 **[!UICONTROL 下载]** 报表，选择 **[!UICONTROL 下载者]**. 下图说明了如何在“下载”报表中选择默认列。

   ![](assets/createdownloadreport.png)

   您还可以向这些报表添加自定义列，以显示符合自定义要求的更多数据。

   要将自定义列添加到下载、发布或到期报告，请执行以下步骤：

   1. 要显示自定义列，请点按/单击 **[!UICONTROL 添加]** 范围 [!UICONTROL 自定义列].
   1. 在中指定列的名称 **[!UICONTROL 列名称]** 字段。
   1. 使用属性选取器选择列需要映射到的属性。

      ![](assets/property-picker.png)
或者，在属性路径字段中键入路径。

      ![](assets/property-path.png)

      要添加更多自定义列，请点按/单击 **添加** 并重复步骤2和3。

1. 点按/单击&#x200B;**[!UICONTROL 创建]**。此时将显示一条消息，通知已开始生成报告。

## 下载报表 {#download-reports}

要将报表保存并下载为.csv文件，请执行以下操作之一：

* 在“资产报表”页面上选择一个报表，然后点按/单击 **[!UICONTROL 下载]** 从顶部的工具栏中。

![](assets/download-asset-report.png)

* 在“资产报表”页面中，打开报表。 选择 **[!UICONTROL 下载]** 选项。

![](assets/download-report-fromwithin.png)

## 删除报告 {#delete-reports}

要删除现有报表，请从中选择该报表 **[!UICONTROL 资产报表]** 页面并点按/单击 **[!UICONTROL 删除]** 从顶部的工具栏中。

>[!NOTE]
>
>**[!UICONTROL 使用情况]** 无法删除报告。
