---
title: 来宾访问 Brand Portal
seo-title: 来宾访问 Brand Portal
description: 允许客人访问并节省下载大量不需要通过身份验证的用户的工作。
seo-description: 允许客人访问并节省下载大量不需要通过身份验证的用户的工作。
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: mgulati
topic-tags: introduction
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
translation-type: tm+mt
source-git-commit: e0f54b9a709d9414208bc6150e75a03f1d322cba
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 1%

---


# 来宾访问 Brand Portal {#guest-access-to-brand-portal}

AEM Brand Portal允许客人访问门户。 客人用户无需凭据即可进入门户，并有权访问门户的公共资产（和集合）。 来宾会话中的用户可以将资产添加到其lightbox（专用集合）并下载相同的资产，直到其会话持续。除非来宾用户选择“结束会话”，否则会话从会话开始算起2 [[!UICONTROL 小时]](#exit-guest-session)。

客人访问功能使组织 [能够快速大规模地与](../using/brand-portal-sharing-folders.md#how-to-share-folders) 目标受众共享获准资产，而无需加入这些资产。 从Brand Portal 6.4.2开始，可为多个并发来宾用户提供服务，这是每个组织的用户配额总数的10%。 允许客人访问可节省管理和安装大量需要在Brand Portal上使用有限功能的用户的时间。\
组织可以使用管理工具面板中的“访问”设置中的“允许客人访 **[!UICONTROL 问]** ”选项， **[!UICONTROL 在组织的Brand Portal帐户上启]** 用（或禁用）客人访问。

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## 开始来宾会话 {#begin-guest-session}

要匿名进入Brand Portal，请选择“ **[!UICONTROL 单击此处]** ”，与“客人 **[!UICONTROL 访问”对应？]** 在Brand Portal欢迎屏幕上。 输入catcha安全检查以授予使用Brand Portal的访问权限。

![](assets/bp-login-screen.png)

## 来宾会话持续时间 {#guest-session-duration}

客人用户会话在2小时内保持活动状态。 这意味着Lightbox的状态将保 **[!UICONTROL 留到]** 会话开始时间起1小时后，当前来宾会话将在2小时后重新启动，因此Lightbox状态将丢失。\
例如，客人用户在15时登录Brand Portal，并将资产添加到Lightbox，然后在16时50分下载。 如果用户在17:00 **[!UICONTROL 小时]** （或其资产）之前未下载Lightbox集合（或其资产），则 **** Lightbox将变为空，因为用户将必须在1小时结束时（即1700小时）重新启动会话。

## 允许并发来宾会话 {#concurrent-guest-sessions-allowed}

并发来宾会话数限制为每个组织用户配额总数的10%。 这意味着对于用户配额为200的组织，最多可以同时使用20个来宾用户。 第21个用户被拒绝访问，并且仅当20个活动来宾用户中的任意一个的会话结束时，才能以客人身份访问。

## 与Brand Portal的客人用户交互 {#guest-user-interaction-with-brand-portal}

### 来宾UI导航

在以客人身份进入Brand Portal时，用户可以公开或仅与 [客人用户共享的所有资](../using/brand-portal-sharing-folders.md#sharefolders) 源和文件夹。 此视图是仅限内容的视图，它在卡、列表或列布局中显示资产。

![](assets/disabled-folder-hierarchy1.png)

但是，如果管理员已启用“启用文件夹层次结构”配置，则来宾用户将在登录到Brand Portal时看到文件夹树（从根文件夹开始）和在各自父文件夹内排 [列的共享文件夹](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) 。

这些父文件夹是虚拟文件夹，不能对其执行任何操作。 您可以通过锁定图标识别这些虚拟文件夹。

与共享文件夹不同，在卡片任务中悬停或选 **[!UICONTROL 择操作]**&#x200B;时，不会显示任何操作视图。 **[!UICONTROL 在列]** 视图和列表视图中选择虚拟文件 **[!UICONTROL 夹时]** ，将显示 **[!UICONTROL 概述按钮]**。

>[!NOTE]
>
>虚拟文件夹的默认缩略图是第一个共享文件夹的缩略图。

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

**[!UICONTROL 视图设置]** 选项允许客人用户调整卡视图中的卡 **[!UICONTROL 大小]** ，或调整列以 **[!UICONTROL 列表视图显示]**。

![](assets/nav-guest-user.png)

通过 **[!UICONTROL 内容树]** ，您可以在资产层次结构中移动。

![](assets/guest-login-ui.png)

Brand Portal为客人 **[!UICONTROL 用户提]** 供了“概述”选项， **[!UICONTROL 以便将选定资]** 产／文件夹的资产属性进行视图。 “概 **[!UICONTROL 述]** ”选项可见：

* 在顶部的工具栏中，选择资产／文件夹。
* 在下拉菜单中，选择边栏选择器。
在选择资 **[!UICONTROL 产]** /文件夹时选择概述选项，用户可以查看资产创建的标题、路径和时间。 但是，在资产详细信息页面上，选 **[!UICONTROL 择概述]** 选项可让用户查看资产的元数据。

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)<br />

**[!UICONTROL 左边栏]** 中的导航选项允许在来宾会话中从文件导航到集合，然后返回，以便用户浏览文件或集合中的资产。

**[!UICONTROL “筛选]** ”选项允许客人用户使用管理员设置的搜索谓词筛选资产文件和文件夹。

### 客人用户功能

客人用户可以在Brand Portal上访问公共资产，并且如进一步讨论的那样，限制很少。

**客人用户可以**:

* 访问适用于所有Brand Portal用户的所有公共文件夹和集合。
* 浏览成员、详细信息页面，并拥有所有公共文件夹和集合成员的完整资产视图。
* 在公共文件夹和收藏集中搜索资产。
* 将资产添加到Lightbox收藏集。 对集合的这些更改会在会话期间持续存在。
* 直接或通过Lightbox收集下载资产。

**客人用户不能**:

* 创建集合和保存的搜索，或进一步共享它们。
* 访问文件夹和收藏集设置。
* 将资产共享为链接。

### 在客人会话中下载资源

客人用户可以直接在Brand Portal上下载公共或专供客人用户共享的资源。 客人用户还可以将资产添 **[!UICONTROL 加到Lightbox]** （公共收藏集），并在 **[!UICONTROL Lightbox收藏集过]** 期前下载Lightbox收藏集。

要下载资产和集合，请使用下载图标：

* 快速操作缩略图，将指针悬停在资产或集合上方时显示
* 顶部的工具栏，在选择资产或收藏集时显示该工具栏

![](assets/download-on-guest.png)

选择 **[!UICONTROL “在下载]** ”对话 [!UICONTROL 框上启] 用下载加速 [”可](../using/accelerated-download.md)以增强下载性能。

## 退出来宾会话 {#exit-guest-session}

要退出来宾会话，请 **[!UICONTROL 从标题中]** 可用的选项中使用“结束会话”。 但是，如果用于来宾会话的浏览器选项卡处于非活动状态，则会话在两小时不活动后自动过期。

![](assets/end-guest-session.png)

## 监视来宾用户活动 {#monitoring-guest-user-activities}

管理员可以监视来宾用户与Brand Portal的交互。 在Brand Portal中生成的报告可以提供对客人用户活动的重要洞察。 例如，“ **[!UICONTROL 下载]** ”报告可用于跟踪来宾用户下载的资产计数。 **[!UICONTROL “用户登录]** ”报告可以通知来宾用户上次登录到门户的时间以及指定持续时间内的登录频率。
