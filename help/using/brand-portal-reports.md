---
title: 使用报告
seo-title: 使用报告
description: AEM Assets Brand Portal管理员可以查看有关Brand Portal使用情况的报表，以及创建、管理和查看有关通过Brand Portal共享的已下载、过期、已发布和链接资产的报表。
seo-description: AEM Assets Brand Portal管理员可以查看有关Brand Portal使用情况的报表，以及创建、管理和查看有关通过Brand Portal共享的已下载、过期、已发布和链接资产的报表。
uuid: dc4e5275-a614-4b95-8c70-2b7e470c50a7
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 7683074f-b6ea-42e0-a411-3b13eb88d1f2
role: Admin
exl-id: 03d0292c-23c2-4ea0-9781-eb27768e6c33
source-git-commit: 26b009fec800d9b437bde5838009c71b1b3b7ac6
workflow-type: tm+mt
source-wordcount: '1023'
ht-degree: 2%

---

# 使用报告 {#work-with-reports}

报告功能有助于评估Brand Portal的使用情况，并了解内部和外部用户如何与已批准的资产进行交互。 管理员可以查看Brand Portal使用情况报表，该报表始终在资产报表页面上提供。 但是，可以从资产报表页面生成和查看用户登录以及通过链接共享的资产、已下载、过期、已发布和资产的报表。 这些报表有助于分析资产部署，从而让您获得关键成功量度来衡量组织内外已批准资产的采用情况。

报表管理界面是直观的，包括用于访问已保存报表的细粒度选项和控件。 您可以从资产报表页面中查看、下载或删除报表，资产报表页面中会列出所有之前生成的报表。

## 查看报表 {#view-reports}

要查看报表，请执行以下步骤：

1. 在顶部的工具栏中，点按/单击AEM徽标以访问管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，单击&#x200B;**[!UICONTROL 创建/管理报表]**&#x200B;以打开&#x200B;**[!UICONTROL 资产报表]**&#x200B;页面。

   ![](assets/access-asset-reports.png)

1. 访问&#x200B;**[!UICONTROL 使用情况]**&#x200B;报表和从资产报表页面生成的其他报表。

   >[!NOTE]
   >
   >“使用情况”报表是在Brand Portal中生成的默认报表。 无法创建或删除。 但是，您可以创建、下载和删除“下载”、“过期”、“发布”、“链接共享”和“用户登录”报表。

   要查看报表，请单击报表链接。 或者，选择报表，然后点按/单击工具栏中的查看图标。

   **[!UICONTROL 使用]** 情况报表显示有关Brand Portal活动用户数、所有资产所占用的存储空间以及Brand Portal中的资产总数的信息。未分配到Admin Console中任何产品配置文件的Brand Portal用户将被视为不活动用户，并且不会反映在&#x200B;**[!UICONTROL 使用情况报表]**中。
此报表还显示每个信息量度的允许容量。

   ![](assets/usage-report.png)

   **[!UICONTROL “用]** 户登录”报表提供有关登录到Brand Portal的用户的信息。在生成报表之前，报表会显示Brand Portal 6.4.2部署中每个用户的显示名称、电子邮件ID、角色（管理员、查看者、编辑者、来宾）、群组、上次登录、活动状态以及登录计数。

   ![](assets/user-logins.png)

   **** 下载报表列表以及有关在特定日期和时间范围内下载的所有资产的详细信息。

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >资产&#x200B;**[!UICONTROL 下载]**&#x200B;报表仅显示从Brand Portal单独选择和下载的资产。 如果用户下载了包含资产的文件夹，则报表不会显示该文件夹或文件夹内的资产。

   **** 到期报表会列出并详细列出特定时间范围内到期的所有资产。

   ![](assets/expiration-report.png)

   **** 发布报表列出并提供有关指定时间范围内从AEM发布到Brand Portal的所有资产的信息。

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >发布报表不显示有关内容片段的信息，因为内容片段无法发布到Brand Portal。

   **[!UICONTROL 链接共]** 享报表列出了特定时间范围内通过Brand Portal界面链接共享的所有资产。此报表还会通知通过链接共享资产的时间、用户、链接的过期时间以及租户（以及共享资产链接的用户）的共享链接数量。 链接共享报表的列不可自定义。

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >链接共享报表不会显示有权访问通过链接共享的资产或已通过链接下载资产的用户。
   >
   >要跟踪通过共享链接的下载，您需要在选择&#x200B;**[!UICONTROL 创建报表]**&#x200B;页面上的&#x200B;**[!UICONTROL 仅链接共享下载]**&#x200B;选项后生成下载报告。 但是，在这种情况下，用户（下载者）是匿名的。

## 生成报表 {#generate-reports}

管理员可以生成并管理以下标准报表，生成后，这些报表将保存为[accessed](../using/brand-portal-reports.md#main-pars-header)之后：

* 用户登录
* 下载
* 到期时间
* 发布
* 链接共享

可以自定义下载、过期和发布报表中的列以供查看。 要生成报表，请执行以下步骤：

1. 在顶部的工具栏中，点按/单击AEM徽标以访问管理工具。

1. 在管理工具面板中，点按/单击&#x200B;**[!UICONTROL 创建/管理报表]** ，以打开&#x200B;**[!UICONTROL 资产报表]**&#x200B;页面。

   ![](assets/asset-reports.png)

1. 在资产报表页面中，点按/单击&#x200B;**[!UICONTROL 创建]**。
1. 从&#x200B;**[!UICONTROL 创建报表]**&#x200B;页面中，选择要创建的报表，然后点按/单击&#x200B;**[!UICONTROL 下一个]**。

   ![](assets/crete-report.png)

1. 配置报表详细信息。 为&#x200B;**[!UICONTROL Download]**、**[!UICONTROL Expiration]**&#x200B;和&#x200B;**[!UICONTROL Publish]**&#x200B;报表指定标题、描述、文件夹结构（其中报表需要运行并生成统计信息）和日期范围。

   ![](assets/create-report-page.png)

   而&#x200B;**[!UICONTROL 链接共享报表]**&#x200B;只需要标题、描述和日期范围参数。

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >在报表生成时，报表标题中的特殊字符#和%将替换为连字符(-)。

1. 点按/单击&#x200B;**[!UICONTROL Next]**，以配置“下载”、“过期”和“发布”报表的列。
1. 根据需要选择或取消选择相应的复选框。 例如，要在&#x200B;**[!UICONTROL Download]**&#x200B;报表中查看下载资产的用户名称，请选择&#x200B;**[!UICONTROL Downloaded By]**。 下图说明了如何在下载报表中选择默认列。

   ![](assets/createdownloadreport.png)

   您还可以向这些报表添加自定义列，以根据您的自定义要求显示更多数据。

   要向“下载”、“发布”或“过期”报表添加自定义列，请执行以下步骤：

   1. 要显示自定义列，请点按/单击[!UICONTROL 自定义列]中的&#x200B;]**添加。**[!UICONTROL 
   1. 在&#x200B;**[!UICONTROL 列名称]**&#x200B;字段中指定列的名称。
   1. 使用属性选取器，选择列需要映射到的属性。

      ![](assets/property-picker.png)
或者，在属性路径字段中键入路径。

      ![](assets/property-path.png)

      要添加更多自定义列，请点按/单击&#x200B;**添加**，然后重复步骤2和3。

1. 点按/单击&#x200B;**[!UICONTROL 创建]**。系统会显示一条消息，通知已开始生成报告。

## 下载报表 {#download-reports}

要将报表保存并下载为.csv文件，请执行以下操作之一：

* 在资产报表页面上选择一个报表，然后点按/单击顶部工具栏中的&#x200B;**[!UICONTROL 下载]** 。

![](assets/download-asset-report.png)

* 从资产报表页面中，打开一个报表。 从报表页面顶部选择&#x200B;**[!UICONTROL Download]**&#x200B;选项。

![](assets/download-report-fromwithin.png)

## 删除报表 {#delete-reports}

要删除现有报表，请从&#x200B;**[!UICONTROL 资产报表]**&#x200B;页面中选择报表，然后点按/单击顶部工具栏中的&#x200B;**[!UICONTROL 删除]** 。

>[!NOTE]
>
>**** 无法删除使用报告。
