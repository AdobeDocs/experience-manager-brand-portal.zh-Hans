---
title: 管理Brand Portal上的用户访问权限
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
source-wordcount: '290'
ht-degree: 2%

---

# 管理Brand Portal上的用户访问权限 {#administer-user-access-on-brand-portal}

Adobe Experience Manager Assets Brand Portal 6.4.2及更高版本授权管理员配置Guest访问权限，并允许用户请求访问其组织的Brand Portal。 这些配置已在管理面板上作为&#x200B;**[!UICONTROL 访问设置]**&#x200B;配置提供。 默认情况下，这两个设置都处于禁用状态。

![](assets/access-configs.png)

**A**   允许使用&#x200B;**[!UICONTROL 来宾访问Brand Portal的来宾访问配置？Brand Portal欢迎屏幕上的]**&#x200B;链接。 （默认值为禁用）

**B**   配置允许用户使用&#x200B;**[!UICONTROL 需要访问权限来请求访问Brand Portal？Brand Portal欢迎屏幕上的]**&#x200B;链接。 （默认值为禁用）

## 允许来宾访问 {#allow-guest-access}

通过允许Guest访问，用户可以访问公共资源而无需登录Brand Portal。
要允许Guest访问，管理员必须执行以下步骤：

1. 从顶部的工具栏中选择AEM徽标以访问管理工具。
1. 从管理工具面板中，选择&#x200B;**[!UICONTROL 访问]**&#x200B;以打开&#x200B;**[!UICONTROL 访问设置]**&#x200B;页面。
1. 启用&#x200B;**[!UICONTROL 允许来宾访问]**&#x200B;配置。
1. **[!UICONTROL 保存]**&#x200B;更改。
1. 注销以使更改生效。

![](assets/bp-welcome-screen.png)

## 允许用户请求访问权限 {#allow-users-to-request-access}

管理员可允许组织用户从欢迎屏幕请求访问Brand Portal。 但是，管理员需要启用&#x200B;**[!UICONTROL 允许用户请求访问]**&#x200B;配置，以便在欢迎屏幕上显示请求访问链接。

要允许组织用户请求访问Brand Portal，管理员需要：

1. 从顶部的工具栏中选择AEM徽标以访问管理工具。
1. 从管理工具面板中，选择&#x200B;**[!UICONTROL 访问]**&#x200B;以打开&#x200B;**[!UICONTROL 访问设置]**&#x200B;页面。
1. 启用&#x200B;**[!UICONTROL 允许用户请求访问]**&#x200B;配置。
1. **[!UICONTROL 保存]**&#x200B;更改。
1. 注销以使更改生效。
