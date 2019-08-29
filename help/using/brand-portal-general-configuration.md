---
title: 管理常规租户配置
seo-title: 管理常规租户配置
description: 配置下载加速，公共智能[！UICCONTROL集合]创建，公共[！UICCONTROL集合]创建，并使管理员用户能够删除租户中的资产。
seo-description: 配置下载加速，公共智能[！UICCONTROL集合]创建，公共[！UICCONTROL集合]创建，并使管理员用户能够删除租户中的资产。
uuid: 3c46cd7c-c38 b-4bc7-b566-93f977 bc8227
contentOwner: murati
topic-tags: administration
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Brand_ Portal
discoiquuid: f4c237bc-f6 a4-4bc4-af56-3d9 c3027 df4
translation-type: tm+mt
source-git-commit: ea7fdd2df0696ed309227fa77e3f79d0141bcb58

---


# 管理常规租户配置 {#administer-general-tenant-configurations}

[!DNL AEM] 资产允许 [!DNL Brand Portal] 组织为特定租户配置以下功能：

* 管理员删除资产
* 非管理员用户创建公共 [!UICONTROL 集合]
* 非管理员用户创建公共智能 [!UICONTROL 收藏集]
* 下载加速
* 非管理员用户可见的共享文件夹的父层次结构

这些配置已在管理工具面板上作为 **常规设置** 配置提供。

![](assets/general-configs.png)

**** 允许管理员从中删除资产的配置 [!DNL Brand Portal]。(默认启用)

**B** 配置以允许非管理员用户创建公共 [!UICONTROL 集合]。(默认启用)

**C** 配置以允许非管理员用户创建公共智能 [!UICONTROL 收藏集]。(默认启用)

**D** 配置允许下载从门户下载的资源以及共享链接中下载的资源。(默认禁用)

**E** 配置用于将共享文件夹的文件夹层次结构(从根文件夹)显示给非管理员用户(编辑器、查看器、客人用户)。(默认禁用)

## 启用/禁用常规配置 {#enable-disable-general-configurations}

要启用/禁用每个配置，请执行以下操作：

1. 以管理员权限登录。
2. 从顶部工具栏中选择 [!DNL AEM] 用于访问管理工具的徽标。
3. 从管理工具面板中，选择 **常规** 以打开 **常规设置** 页面。
4. 使用相应的切换开关启用/禁用任何常规配置。
5. **保存更改。**
6. 注销以使更改生效。

## 允许管理用户从 [!DNL Brand Portal]{#allow-admin-users-to-delete-assets-from-brand-portal}

**允许用户删除** 配置允许组织允许具有管理员权限的用户从中删除资产和文件夹 [!DNL Brand Portal]。

## 允许非管理员创建公共集合 {#allow-public-collections-creation-by-non-admins}

[允许公共 [!UICONTROL 集合]创建](..// using/brand-path-share-[!UICONTROL collection]. md# main-pars-text-1915052376)配置控制非管理员能否创建公共 [!UICONTROL 集合][!DNL Brand Portal]。默认情况下，配置处于启用状态。禁用配置组织可阻止在其门户上有大量公共 [!UICONTROL 集合]，从而可以保存系统空间。

## 允许非管理员的公共智能收藏集创建 {#allow-public-smart-collections-creation-by-non-admins}

[允许公共智能收藏集创建](../using/brand-portal-searching.md#main-pars-header-500620467) 配置控制非管理员是否可以将其搜索另存为智能 [!UICONTROL 收藏集，] 并将其公开为该租户公开。默认情况下，配置处于启用状态。禁用配置组织可防止拥有大量由组织的非管理员用户创建的公共智能 [!UICONTROL 收藏集][!DNL Brand Portal]。

## 允许下载加速 {#allow-download-acceleration}

[允许下载加速](../using/accelerated-download.md) 配置允许组织通过与作为按需安装应用程序的IBM AssPera Connect集成，允许更快地从 [!DNL Brand Portal] 链接和共享链接下载资源。该应用程序使用专有技术删除TCP覆盖。

## 启用文件夹层次结构 {#enable-folder-hierarchy}

[“启用文件夹层次结构](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) ”配置允许管理员控制非管理员用户(编辑器、查看器和来宾用户)在登录后看到共享文件夹的方式。
