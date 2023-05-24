---
title: 来宾访问 Brand Portal
seo-title: Guest Access to Brand Portal
description: 允许Guest访问，无需身份验证即可载入大量用户。
seo-description: Allow guest access and save the effort to onboard numerous users without authentication.
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: VG
topic-tags: introduction
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
exl-id: ecce0a45-abae-41c4-9ea7-5dfdcf19e5ea
source-git-commit: 51dc6f9c3b3a59751d7910513279e52906d97b88
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 0%

---

# 来宾访问 Brand Portal {#guest-access-to-brand-portal}

Experience Manager Assets Brand Portal允许Guest访问该门户。 来宾用户无需凭据即可进入门户，并且有权访问门户的公共资产（和收藏集）。 来宾会话中的用户可以将资产添加到Lightbox（专用收藏集）并下载这些资产，直到其会话持续为止，也就是从会话开始算起2小时，除非来宾用户选择 [[!UICONTROL 结束会话]](#exit-guest-session).

来宾访问功能使组织能够 [快速共享批准的资产](../using/brand-portal-sharing-folders.md#how-to-share-folders) 让目标受众规模化，而无需加入他们。 从Brand Portal 6.4.2开始，已配备多个并发来宾用户，这相当于每个组织总用户配额的10%。 允许Guest访问可节省在Brand Portal上管理功能有限的用户和板载用户的时间。\
对于组织的Brand Portal帐户，组织可以使用启用（或禁用）来宾访问 **[!UICONTROL 允许Guest访问]** 选项自 **[!UICONTROL 访问]** “管理工具”面板中的设置。

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## 开始来宾会话 {#begin-guest-session}

要匿名进入Brand Portal，请选择 **[!UICONTROL 单击此处]** 对应于 **[!UICONTROL 来宾访问？]** 在Brand Portal欢迎屏幕上。 输入captcha安全检查以授予使用Brand Portal的访问权限。

![](assets/bp-login-screen.png)

## 来宾会话持续时间 {#guest-session-duration}


访客用户会话保持活动状态15分钟。
这意味着 **[!UICONTROL 灯箱]** 从会话开始时间起保留15分钟，之后将重新启动当前来宾会话，从而丢失Lightbox状态。

例如，访客用户在15时登录到Brand Portal，然后将资源添加到 **[!UICONTROL 灯箱]** 可在15时05分下载。 如果用户不下载 **[!UICONTROL 灯箱]** 收藏集（或其资产）的时间早于15:15（登录后15分钟内），用户必须重新启动会话。 此 **[!UICONTROL 灯箱]** 为空，这意味着如果会话丢失，上传的资产不再可用。

## 允许的并发来宾会话 {#concurrent-guest-sessions-allowed}

每个组织的并发来宾会话数限制为总用户配额的10%。 这意味着对于用户配额为200的组织，最多可同时工作20个访客用户。 拒绝第21位用户访问，只有在20位活动来宾用户的会话结束时，才能以来宾身份访问。

>[!NOTE]
>
>如果获得许可的用户数量超过约定的值（配额），Brand Portal不会发送通知。 此外，它不会限制许可用户的任何活动。

## 访客用户与Brand Portal的交互 {#guest-user-interaction-with-brand-portal}

### 访客UI导航

以访客身份进入Brand Portal后，用户可以看到所有 [共享的资产和文件夹](../using/brand-portal-sharing-folders.md#sharefolders) 公开或仅与访客用户一起使用。 此视图是仅内容视图，它以卡片、列表或列布局显示资产。

![](assets/disabled-folder-hierarchy1.png)

但是，在登录到Brand Portal时，来宾用户会看到文件夹树（从根文件夹开始）以及在其各自的父文件夹内排列的共享文件夹（如果管理员已启用） [启用文件夹层次结构](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) 配置。

这些父文件夹是虚拟文件夹，不能对它们执行任何操作。 您可以使用锁图标来识别这些虚拟文件夹。

悬停或选择操作任务时不会显示任何操作任务 **[!UICONTROL 卡片视图]**，与共享文件夹不同。 **[!UICONTROL 概述]** 选择中的虚拟文件夹时显示按钮 **[!UICONTROL 列视图]** 和 **[!UICONTROL 列表视图]**.

>[!NOTE]
>
>虚拟文件夹的默认缩略图是第一个共享文件夹的缩略图图像。

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

**[!UICONTROL 查看设置]** 选项允许来宾用户调整卡片大小 **[!UICONTROL 卡片视图]** 或要显示的列 **[!UICONTROL 列表视图]**.

![](assets/nav-guest-user.png)

此 **[!UICONTROL 内容树]** 允许您在资源层次结构中移动。

![](assets/guest-login-ui.png)

Brand Portal提供 **[!UICONTROL 概述]** 来宾用户查看的选项 **[!UICONTROL 资产属性]** 个资源/文件夹中的。 此 **[!UICONTROL 概述]** 选项可见：

* ，位于顶部工具栏中选择资产/文件夹。
* 在下拉菜单中选择边栏选择器。

选择 **[!UICONTROL 概述]** 选项选中某个资源/文件夹后，用户可以查看资源创建的标题、路径和时间。 而在资产详细信息页面上，选择 **[!UICONTROL 概述]** 选项允许用户查看资源的元数据。

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

**[!UICONTROL 导航]** 左侧边栏中的选项允许从文件导航到收藏集，然后再导航回guest会话，以便用户可以浏览文件或收藏集中的资产。

**[!UICONTROL 筛选条件]** 选项允许来宾用户使用管理员设置的搜索谓词筛选资源文件和文件夹。

### 来宾用户功能

Guest用户可以访问Brand Portal上的公共资源，并且几乎没有限制，具体如下所述。

**来宾用户可以**：

* 访问适用于所有Brand Portal用户的所有公共文件夹和收藏集。
* 浏览成员、详细信息页面，并拥有所有公用文件夹和收藏集成员的完整资产视图。
* 在公共文件夹和收藏集中搜索资产。
* 将资产添加到Lightbox收藏集。 对收藏集的这些更改将在会话期间保留。
* 直接或通过Lightbox收藏集下载资产。

**来宾用户不能**：

* 创建收藏集和保存的搜索，或进一步共享它们。
* 访问文件夹和收藏集设置。
* 将资产作为链接共享。

### 在来宾会话中下载资产

访客用户可以直接下载在Brand Portal上公开或专门与访客用户共享的资源。 访客用户还可以将资源添加到 **[!UICONTROL 灯箱]** （公共收藏集），并下载 **[!UICONTROL 灯箱]** 收藏集。

要下载资源和收藏集，请使用以下位置的下载图标：

* 快速操作缩略图，将鼠标悬停在资产或收藏集上时显示
* 顶部的工具栏，在选择资源或收藏集时显示

![](assets/download-on-guest.png)

选择 **[!UICONTROL 启用下载加速]** 日期 [!UICONTROL 下载] 对话框允许您 [提高下载性能](../using/accelerated-download.md).

## 退出来宾会话 {#exit-guest-session}

要退出来宾会话，请使用 **[!UICONTROL 结束会话]** 从标题中可用的选项中找到。 但是，如果用于来宾会话的浏览器选项卡处于非活动状态，则会话将在处于非活动状态两小时后自动过期。

![](assets/end-guest-session.png)

## 监视来宾用户活动 {#monitoring-guest-user-activities}

管理员可以监视来宾用户与Brand Portal的交互。 在Brand Portal中生成的报表可以提供有关访客用户活动的关键见解。 例如， **[!UICONTROL 下载]** 报告可用于跟踪访客用户下载的资产计数。 **[!UICONTROL 用户登录]** 报告可以告知访客用户上次登录门户的时间以及在指定持续时间内登录的频率。
