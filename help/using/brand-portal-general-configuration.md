---
title: 管理常规租户配置
seo-title: Administer general tenant configurations
description: 配置下载加速、公共智能收藏集创建、公共收藏集创建，并允许管理员用户删除租户上的资产。
seo-description: Configure download acceleration, public smart collection creation, public collection creation, and enable admin users to delete assets on tenants.
uuid: 3c46cd7c-c38b-4bc7-b566-93f977bc8227
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f4c237bc-f6a4-4bc4-af56-3d9c3027daf4
role: Admin
exl-id: 5607be8e-0a7f-4692-b71b-5f66eb9ac5ee
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 3%

---

# 管理常规租户配置 {#administer-general-tenant-configurations}

Experience Manager Assets Brand Portal允许组织为特定租户配置以下功能：

* 管理员删除资产
* 非管理员用户创建公共收藏集
* 非管理员用户创建公共智能收藏集
* 非管理员用户可见的共享文件夹的父层次结构

这些配置提供为 **[!UICONTROL 常规设置]** “管理工具”面板上的配置。

![](assets/general-config.png)

**A**   允许管理员从Brand Portal中删除资源的配置。 （默认启用）

**B**   允许非管理员用户创建公共收藏集的配置。 （默认启用）

**C**   允许非管理员用户创建公共智能收藏集的配置。 （默认启用）

**D**  用于向非管理员用户（编辑者、查看者、来宾用户）显示共享文件夹的文件夹层次结构（从根目录）的配置。 （默认值为禁用）

## 启用/禁用常规配置 {#enable-disable-general-configurations}

要启用/禁用每个配置，请执行以下操作：

1. 以管理员权限登录。
1. 从顶部的工具栏中选择Experience Manager徽标以访问管理工具。
1. 从管理工具面板中，选择 **[!UICONTROL 常规]** 以打开 **[!UICONTROL 常规设置]** 页面。
1. 使用相应的切换开关来启用/禁用任何常规配置。
1. **[!UICONTROL 保存更改。]**
1. 注销以使更改生效。

## 允许管理员用户从Brand Portal删除资源 {#allow-admin-users-to-delete-assets-from-brand-portal}

**[!UICONTROL 允许用户删除]** 通过配置，组织可以允许（或限制）具有管理员权限的用户从Brand Portal中删除资源和文件夹。

## 允许非管理员创建公共收藏集 {#allow-public-collections-creation-by-non-admins}

[[!UICONTROL 允许创建公共收藏集]](../using/brand-portal-share-collection.md#main-pars-text-1915052376) 配置控制非管理员是否可以在Brand Portal上创建公共收藏集。 默认启用配置。 通过禁用配置，组织可以阻止其门户上有大量公共收藏集，从而节省系统空间。

## 允许非管理员创建公共智能收藏集 {#allow-public-smart-collections-creation-by-non-admins}

[[!UICONTROL 允许创建公共智能收藏集]](../using/brand-portal-searching.md#main-pars-header-500620467) 配置控制非管理员是否可以将其搜索另存为智能收藏集，并将其为该租户公开。 默认启用配置。 通过禁用配置，组织可以阻止非管理员用户在组织的Brand Portal上创建大量公共智能收藏集。

<!-- 
## Allow download acceleration {#allow-download-acceleration}

[[!UICONTROL Allow download acceleration]](../using/accelerated-download.md) configuration lets the organizations to allow accelerated downloads of assets from Brand Portal and shared links, by integrating with IBM Aspera Connect that is an install-on-demand application. The application uses proprietary technology to remove TCP overheads.
-->

## 启用文件夹层次结构 {#enable-folder-hierarchy}

[[!UICONTROL 启用文件夹层次结构]](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) 通过配置，管理员可以控制非管理员用户（编辑者、查看者和来宾用户）在登录后查看共享文件夹的方式。
