---
title: 常见问题解答
description: 深入了解 Adobe Experience Manager Assets Brand Portal 中的常见问题。
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: ht
source-wordcount: '1500'
ht-degree: 100%

---

# 常见问题解答 {#frequently-asked-questions}

 Brand Portal 常见问题解答主要关注最终用户在使用最新版 (6.4.6) 或更早版本的 Experience Manager Assets Brand Portal 时可能遇到的疑问和问题。


## Brand Portal 6.4.6 常见问题解答 {#faqs-bp646}

**问题：现有的旧版 OAuth 端点 (`https://legacy-oauth.cloud.adobe.io/login`) 不起作用。可能的原因是什么？**

**回答：**&#x200B;旧版 OAuth 配置已被弃用。将 Experience Manager Assets 作者实例升级到最新服务包，并通过 Adobe Developer Console 进行配置。请参阅[使用 Brand Portal 配置 Experience Manager Assets](configure-aem-assets-with-brand-portal.md)，以了解详情。但是为了让旧版 OAuth 配置能够在升级之前正常工作，请将旧版 OAuth 端点更新为 `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`。

**问题：在升级到 Adobe Developer Console 后，我无法将 Brand Portal 中的贡献文件夹的资产发布到 Experience Manager Assets。我的作者实例位于 Experience Manager Assets 6.5.4 上。可能是什么原因导致的？**

**回答：**&#x200B;是的，通过 Adobe Developer Console 将贡献文件夹的资产发布到 Experience Manager Assets 6.5.4 时，存在一个已知问题。

该问题已在 Experience Manager Assets 6.5.5 中得到修复。您可以将您的 Experience Manager Assets 实例升级到最新服务包，并在 Adobe Developer Console 上[升级您的配置](https://experienceleague.adobe.com/zh-hans/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal#upgrade-integration-65)。


**问题：我没有在 Experience Manager Assets 中看到从 Brand Portal 发布的贡献文件夹的内容。可能的原因是什么？**

**回答：**&#x200B;请联系您的 Experience Manager Assets 管理员以验证配置情况，并确保您的 Brand Portal 租户仅配置了一个 Experience Manager Assets 作者实例。

如果您在多个 Experience Manager Assets 作者实例上配置了 Brand Portal 租户，可能会出现此问题。例如，管理员在暂存和生产环境的 Experience Manager Assets 作者实例上配置相同的 Brand Portal 租户。在这种情况下，Brand Portal 中会触发资产发布，但由于复制代理未收到请求令牌，Experience Manager Assets 作者实例无法导入资产。


**问题：我无法将资产从 Experience Manager Assets 发布到 Brand Portal。复制日志显示连接已超时。有快速解决办法吗？**

**回答：**&#x200B;如果复制队列中有多个待处理的请求，则发布通常会因超时错误而失败。要解决此问题，请确保将复制代理配置为避免超时。

执行以下步骤来配置复制代理：

1. 登录到您的 Experience Manager Assets 作者实例。
1. 从&#x200B;**工具**&#x200B;面板中，导航至&#x200B;**[!UICONTROL 部署]** > **[!UICONTROL 复制]**。
1. 在复制页面中点击 **[!UICONTROL `Agents on author`]**。您可以看到 Brand Portal 租户的四个复制代理。
1. 点击复制代理 URL 以打开代理详细信息。
1. 点击&#x200B;**[!UICONTROL 编辑]**&#x200B;来编辑复制代理设置。
1. 在代理设置中，点击&#x200B;**[!UICONTROL 扩展]**&#x200B;选项卡。
1. 选择&#x200B;**[!UICONTROL 关闭连接]**&#x200B;复选框。
1. 重复步骤 4 到 7，配置所有四个复制代理。
1. 重新启动服务器并验证连接。


## Brand Portal 6.4.5 常见问题解答 {#faqs-bp645}

**问题：Brand Portal 6.4.5 版本的主要变化是什么？**

**回答：** Experience Manager Assets Brand Portal 6.4.5 允许用户直接从 Brand Portal 上传内容并将贡献文件夹发布回 Experience Manager Assets，而无需管理员权限。有关详细信息，请参阅[ Brand Portal 中的资产搜寻](brand-portal-asset-sourcing.md)。



**问题：我是否无法再访问自己创建的任何现有资产、功能或配置了？**

**回答：** 您现有的所有功能和配置都保持不变。您的最终用户不会受到影响，您的内容也保持不变。



**问题：我什么时候可以迁移到新版本的 Brand Portal？**

**回答：** Brand Portal 6.4.5 于 2019 年 10 月正式发布。下一个 Brand Portal 版本预计将于 2020 年 3 月发布。关于更新和版本变更，Adobe 建议您关注[发行说明](brand-portal-release-notes.md)和[ Brand Portal 新增功能](whats-new.md)。



**问题：我的用户是否受到影响？**

**回答：** Brand Portal 6.4.5 版本仅在 Brand Portal 内发布，因此不会对您的最终用户产生影响。



**问题：作为 Brand Portal 用户，我需要采取什么行动吗？**

**回答：** Brand Portal 6.4.5 版本附带一项名为资产搜寻的新功能。管理员需在 Experience Manager Assets 中配置资产搜寻功能，以便为 Brand Portal 用户启用该功能。有关详细信息，请参阅[启用资产搜寻](brand-portal-asset-sourcing.md)。



**问题：谁可以创建贡献文件夹？**

**回答：** 任何拥有在 Experience Manager Assets 中创建文件夹权限的 Experience Manager Assets 用户，都可以创建一个&#x200B;**贡献**&#x200B;文件夹。要创建一个&#x200B;**贡献**&#x200B;文件夹，请创建一个类型为&#x200B;**资产贡献**的文件夹。
此文件夹与活跃的 Brand Portal 用户共享，以便他们进行贡献。



**问题：贡献文件夹包含什么？**

**回答：** **贡献**&#x200B;文件夹包含两个子文件夹，即&#x200B;**新的**&#x200B;和&#x200B;**共享**文件夹。最初，新的文件夹为空，而共享文件夹则包含 Brand Portal 用户的引用内容（可重复使用的资产）。
Brand Portal 用户访问**贡献**&#x200B;文件夹，并在&#x200B;**新的**&#x200B;文件夹中上传内容。



**问题：我可以更改现有贡献文件夹的名称吗？**

**回答：** **不可以**，您无法更改现有&#x200B;**贡献**&#x200B;文件夹的名称。



**问题：相对于贡献，资产要求是什么？**

**回答：****贡献**&#x200B;文件夹中的&#x200B;**简介**&#x200B;文档和&#x200B;**共享**&#x200B;文件夹中的引用内容有助于 Brand Portal 用户了解贡献需求和期望。它们合在一起被称为资产要求。

**问题：我可以将资产上传到任何允许的文件夹吗？**

**回答：**&#x200B;不是所有允许的文件夹。Brand Portal 用户只能将内容上传至由 Experience Manager Assets 或 Brand Portal 管理员共享的&#x200B;**贡献**&#x200B;文件夹。



**问题：我该如何获取对“贡献”文件夹的访问权限？**

**回答：**&#x200B;只有当&#x200B;**贡献**&#x200B;文件夹已共享给您时，您才能访问该文件夹。每当有“贡献”文件夹共享给您时，您都会收到一封电子邮件/推送通知。您可以通过电子邮件中共享的链接访问“贡献”文件夹。或者，您可以登录到您的 Brand Portal 实例，并导航至通知的铃铛图标，以访问“贡献”文件夹。

>[!NOTE]
>
>如果您不是 Brand Portal 用户，可以请求 Experience Manager Assets 管理员在 Admin Console 中为您创建用户。然后，将您的轮廓添加到 Brand Portal 用户列表中的用户配置文件中。


**问题：用户导入的 CSV 文件格式是什么？**

**回答：**&#x200B;该格式符合 Admin Console 支持的大批量用户导入格式。电子邮件、名和姓是必填项。



**问题：资产贡献用户下拉菜单中的用户列表（Brand Portal 贡献者）由什么填充？**

**回答：**&#x200B;下拉菜单中的用户是根据在 Experience Manager Assets 中上传的 Brand Portal 用户配置 (.csv) 文件填充的。



**问题：在哪里可以查看导入和发布任务的状态？**

**回答：**&#x200B;在 Experience Manager Assets 中，您可以在&#x200B;**异步**&#x200B;任务页面中查看导入状态。在 Brand Portal 中，您可以在&#x200B;**[!UICONTROL 工具 > 资产贡献状态]**&#x200B;中查看发布任务的状态。



**问题：在 Experience Manager 中，导入任务定期运行的频率是多少？**

**回答：**&#x200B;在 Experience Manager Assets 中，每五分钟进行一次轮询。



**问题：从 Brand Portal 向 Experience Manager Assets 发布文件夹的次数是否有上限？**

**回答：**&#x200B;没有，无论之前是否已发布过，**新的**&#x200B;文件夹中的所有资产都将发布到 Experience Manager Assets。每当从 Brand Portal 向 Experience Manager Assets 发布一个&#x200B;**贡献**&#x200B;文件夹时，该文件夹的内容将取代&#x200B;**新的**&#x200B;文件夹的内容。



**问题：如何在贡献文件夹中上传新资产？**

**回答：**&#x200B;请参阅有关[将资产上传至贡献文件夹](brand-portal-publish-contribution-folder-to-brand-portal.md)的详细文档。



**问题：我无法看到上传到新的文件夹的资产的缩略图或预览。**

**回答：**&#x200B;这是这样设计的，因为 Brand Portal 端不运行任何工作流。



**问题：如果一个文件夹从 Experience Manager Assets 发布到处于变动中的 Brand Portal，会发生什么？**

**回答：**&#x200B;在 Experience Manager Assets 中，每次将文件夹发布到 Brand Portal 时，都会保留相关日志。在发布时，所有未发布到 Brand Portal 的资产都将被添加到复制队列中。在发布任务触发后添加到该文件夹的任何资产都不会发布到 Brand Portal。当 Experience Manager Assets 用户再次发布该文件夹时，只有之前未发布过的（存在于复制队列中的）资产才会发布到 Brand Portal。对于从 Experience Manager Assets 发布到 Brand Portal 的任何文件夹，以及“贡献”文件夹中的“共享”文件夹，此流程均适用。

**问题：如果我有问题应该联系谁？**

**回答：**&#x200B;请联系您的 Adobe 客户经理或客户支持部门。

>[!NOTE]
>
>发布计划是暂定的，可能会有所变动。请联系您的 Adobe 客户经理或客户支持部门，以获取更新的发布计划。


## 产品访问和支持（受限网站） {#product-access-and-support-restricted-sites}

这些网站仅对客户开放。如果您是客户且需要访问权限，请联系您的 Adobe 客户经理。

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Support]()
-->
