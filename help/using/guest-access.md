---
title: 来宾访问 Brand Portal
seo-title: 来宾访问 Brand Portal
description: 允许客人访问，并节省登入大量不需要通过身份验证的用户的工作。
seo-description: 允许客人访问，并节省登入大量不需要通过身份验证的用户的工作。
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: mgulati
topic-tags: introduction
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
translation-type: tm+mt
source-git-commit: 8554b9768040b59d2b1a03a3703b2d7235e63bcb

---


# 来宾访问 Brand Portal {#guest-access-to-brand-portal}

AEM Brand门户允许客人访问门户。 客人用户无需凭据即可进入门户，并有权访问门户的公共资产（和集合）。 来宾会话中的用户可以将资产添加到其Lightbox（专用集合）并下载资产，直到其会话持续，该会话从会话开始算起2小时，除非来宾用户选择“结束会 [[!UICONTROL 话”]](#exit-guest-session)。

客人访问功能使组织能 [够快速地与目标受众批量共享获准资产](../using/brand-portal-sharing-folders.md#how-to-share-folders) ，而无需添加这些资产。 从Brand Portal 6.4.2开始，可为多个并发客人用户提供服务，这是每个组织的用户配额总数的10%。 允许客人访问可节省管理和上架大量需要在Brand Portal上使用有限功能的用户的时间。\
组织可以使用管理工具面板中的“访问”设置中的“允许客人访问 **[!UICONTROL ”选项，在组织的Brand Portal帐户上启用(或禁]****** 用)客人访问。

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## 开始客人会话 {#begin-guest-session}

要匿名进入Brand Portal，请选择“ **[!UICONTROL 单击此处]** ”与“客人访 **[!UICONTROL 问”对应？]** 在Brand Portal欢迎屏幕上。 输入catcha安全检查以授予使用Brand Portal的权限。

![](assets/bp-login-screen.png)

## 客人会话持续时间 {#guest-session-duration}

客人用户会话在2小时内保持活动状态。 这意味着 **** Lightbox的状态将保留到会话开始时间起1小时后，并且在2小时后，当前客人会话将重新启动，因此Lightbox状态将丢失。\
例如，客人用户于15时00分登录到Brand Portal，并将资产添加到Lightbox，以便于16时50分下载。 如果用户在17:00之前未下载 **[!UICONTROL Lightbox]** 集合（或其资产），则 **[!UICONTROL Lightbox]** 将变为空，因为用户将必须在1小时（即1700小时）结束时重新启动会话。

## 允许并发客人会话 {#concurrent-guest-sessions-allowed}

并发客人会话数限制为每个组织的用户配额总数的10%。 这意味着对于用户配额为200的组织，最多可以同时使用20个客人。 第21个用户被拒绝访问，并且仅当20个活动来宾用户中的任意一个的会话结束时，才能以客人身份访问。

## 客人与Brand Portal的用户交互 {#guest-user-interaction-with-brand-portal}

### 客人UI导航

在以客人身份进入Brand Portal时，用户可以查看公开共享的所 [有资产和文件夹](../using/brand-portal-sharing-folders.md#sharefolders) ，或仅与客人用户共享。 此视图是仅限内容的视图，它显示卡片、列表或列布局中的资产。

![](assets/disabled-folder-hierarchy1.png)

但是，如果管理员启用了“启用文件夹层次结构”配置，则客人用户将在登录Brand Portal时看到文件夹树（从根文件夹开始）和在各自父文件夹内排列的共享文件夹 [](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) 。

这些父文件夹是虚拟文件夹，不能对其执行任何操作。 您可以通过锁定图标识别这些虚拟文件夹。

与共享文件夹不同，在卡片视图中悬停或选择 **[!UICONTROL 操作任务时]**，不会显示任何操作任务。 **[!UICONTROL 在“列视图]** ”和“列表视图”中选择虚拟文件夹时， **[!UICONTROL 会显示“概述]** ” **[!UICONTROL 按钮]**。

>[!NOTE]
>
>请注意，虚拟文件夹的默认缩略图是第一个共享文件夹的缩略图。

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

**[!UICONTROL “查看设置]** ”选项允许客人用户调整“卡片视图”中的卡片大 **[!UICONTROL 小]** ，或调整列表视图中 **[!UICONTROL 的显示]**。

![](assets/nav-guest-user.png)

通过 **[!UICONTROL 内容树]** ，您可以在资产层次结构中移动。

![](assets/guest-login-ui.png)

Brand Portal为客人用 **[!UICONTROL 户提供]** “概述”选项，以查 **[!UICONTROL 看选定资产]** /文件夹的资产属性。 “概 **[!UICONTROL 述]** ”选项可见：

* 在顶部的工具栏中，选择资产／文件夹。
* 在下拉菜单中，选择边栏选择器。
在选择资 **[!UICONTROL 产]** /文件夹时选择“概述”选项后，用户可以查看资产创建的标题、路径和时间。 但是，在资产详细信息页面上，选 **[!UICONTROL 择“概述]** ”选项可让用户查看资产的元数据。

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)<br />

**[!UICONTROL 通过]** 左边栏中的导航选项，可在来宾会话中从文件导航到集合，然后返回，以便用户浏览文件或集合中的资产。

**[!UICONTROL “筛选]** ”选项允许客人用户使用管理员设置的搜索谓词筛选资产文件和文件夹。

### 客人用户功能

客人用户可以访问Brand Portal上的公共资源，并且还没有进一步讨论的限制。

**客人用户可以**:

* 访问所有Brand Portal用户专用的所有公共文件夹和集合。
* 浏览成员、详细信息页面，并拥有所有公共文件夹和集合成员的完整资产视图。
* 在公共文件夹和收藏集中搜索资产。
* 将资产添加到Lightbox收藏集。 对集合的这些更改会在会话期间持续。
* 直接或通过Lightbox集合下载资产。

**客人用户不能**:

* 创建集合和保存的搜索，或进一步共享它们。
* 访问文件夹和收藏集设置。
* 将资产共享为链接。

### 在客人会话中下载资源

客人用户可以直接在Brand Portal上下载与客人用户公开共享或仅共享的资源。 客人用户还可以将资产添加到 **[!UICONTROL Lightbox]** （公共集合），并在其会话过期之前下载 **[!UICONTROL Lightbox]** 集合。

要下载资产和集合，请使用下载图标：

* 将鼠标悬停在资产或集合上时显示的快速操作缩略图
* 顶部的工具栏，在选择资产或收藏集时显示

![](assets/download-on-guest.png)

选择“ **[!UICONTROL 在下载]** ”对话框 [!UICONTROL 上启用下载加速] ”可 [以增强下载性能](../using/accelerated-download.md)。

## 退出客人会话 {#exit-guest-session}

要退出客人会话，请使用 **[!UICONTROL 标题中可用的选项]** “结束会话”。 但是，如果用于来宾会话的浏览器选项卡处于非活动状态，则会话在两小时不活动后将自动过期。

![](assets/end-guest-session.png)

## 监视客人用户活动 {#monitoring-guest-user-activities}

管理员可以监视客人与Brand Portal的交互。 在Brand Portal中生成的报告可提供对客人用户活动的重要洞察。 例如，“ **[!UICONTROL 下载]** ”报告可用于跟踪客人用户下载的资产计数。 **[!UICONTROL “用户登录]** ”报告可通知客人用户上次登录门户的时间以及指定持续时间内的登录频率。
