---
title: 管理 Brand Portal 上的用户访问权限
seo-title: Administer user access on Brand Portal
description: 在Brand Portal上配置Guest访问和新用户访问。
seo-description: Configure guest access and new users access on brand portal.
uuid: 522b499d-33a0-455f-ac7e-719face48009
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 393025b4-722d-4e81-8a47-f83415d0b9b6
role: Admin
exl-id: 27a9cd26-9bb3-473b-b1ac-37f77975c912
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 9%

---

# 管理 Brand Portal 上的用户访问权限 {#administer-user-access-on-brand-portal}

Adobe Experience Manager Assets Brand Portal 6.4.2及更高版本授权管理员配置guest访问权限，并允许用户请求访问其组织的Brand Portal。 这些配置提供为 **[!UICONTROL 访问设置]** 配置。 默认情况下，这两个设置都处于禁用状态。

![](assets/access-configs.png)

**A**   允许来宾使用以下方式访问Brand Portal的配置 **[!UICONTROL 来宾访问？]** Brand Portal欢迎屏幕上的链接。 （默认值为禁用）

**B**   允许用户使用以下方式请求访问Brand Portal的配置 **[!UICONTROL 需要访问？]** Brand Portal欢迎屏幕上的链接。 （默认值为禁用）

## 允许来宾访问 {#allow-guest-access}

通过允许Guest访问，用户无需登录Brand Portal即可访问公共资源。
要允许Guest访问，管理员必须执行以下步骤：

1. 从顶部的工具栏中选择AEM徽标以访问管理工具。
1. 从管理工具面板中，选择 **[!UICONTROL 访问]** 打开 **[!UICONTROL 访问设置]** 页面。
1. 启用 **[!UICONTROL 允许Guest访问]** 配置。
1. **[!UICONTROL 保存更改。]**
1. 注销以使更改生效。

![](assets/bp-welcome-screen.png)

## 允许用户请求访问权限 {#allow-users-to-request-access}

管理员可以允许组织用户从欢迎屏幕请求访问Brand Portal。 但是，管理员需要启用 **[!UICONTROL 允许用户请求访问权限]** 配置，以便在欢迎屏幕上显示请求访问链接。

要允许组织用户请求访问Brand Portal，管理员需要：

1. 从顶部的工具栏中选择AEM徽标以访问管理工具。
1. 从管理工具面板中，选择 **[!UICONTROL 访问]** 打开 **[!UICONTROL 访问设置]** 页面。
1. 启用 **[!UICONTROL 允许用户请求访问权限]** 配置。
1. **[!UICONTROL 保存更改。]**
1. 注销以使更改生效。
