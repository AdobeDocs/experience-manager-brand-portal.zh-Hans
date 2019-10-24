---
title: 管理常规租户配置
seo-title: 管理常规租户配置
description: 配置下载加速、公共智 [!UICONTROL 能集合创建] 、公共集 [!UICONTROL 合创建] ，并允许管理员用户删除租户上的资产。
seo-description: 配置下载加速、公共智 [!UICONTROL 能集合创建] 、公共集 [!UICONTROL 合创建] ，并允许管理员用户删除租户上的资产。
uuid: 3c46cd7c-c38b-4bc7-b566-93f977bc8227
contentOwner: mgulati
topic-tags: 管理
content-type: 参考文件
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f4c237bc-f6a4-4bc4-af56-3d9c3027daf4
translation-type: tm+mt
source-git-commit: ff0c8c23b6c76dc9027b560b9db4af2f4b35313e

---


# 管理常规租户配置 {#administer-general-tenant-configurations}

AEM Assets Brand Portal允许组织为特定租户配置以下功能：

* 管理员删除资产
* 非管理员用户创建公共集合
* 非管理员用户创建公共智能收藏集
* 下载加速
* 对非管理员用户可见的共享文件夹的父级层次结构

这些配置已作为“常规 **[!UICONTROL 设置]** ”配置在管理工具面板上提供。

![](assets/general-configs.png)

**允许管理员** 从Brand Portal中删除资产的配置。 （默认为启用状态）

**B配置** ，允许非管理员用户创建公共集合。 （默认为启用状态）

**配置** ，允许非管理员用户创建公共智能收藏集。 （默认为启用状态）

**D** Configuration（配置），允许下载从门户和共享链接下载的资产的加速。 （默认为禁用）

**E** Configuration（配置），用于向非管理员用户（编辑器、查看器、客人用户）显示共享文件夹的文件夹层次结构（从根文件夹）。 （默认为禁用）

## 启用／禁用常规配置 {#enable-disable-general-configurations}

要启用／禁用以下各种配置：

1. 以管理员权限登录。
1. 从顶部的工具栏中选择AEM徽标以访问管理工具。
1. 从管理工具面板中，选择“ **[!UICONTROL 常规]** ”以打开“ **[!UICONTROL 常规设置]** ”页。
1. 使用相应的切换开关启用／禁用任何常规配置。
1. **[!UICONTROL 保存更改。]**
1. 注销以使更改生效。

## 允许管理员用户从Brand Portal中删除资产 {#allow-admin-users-to-delete-assets-from-brand-portal}

**[!UICONTROL 允许用户删除配置]** ，使组织能够允许（或限制）具有管理员权限的用户从Brand Portal中删除资产和文件夹。

## 允许非管理员创建公共集合 {#allow-public-collections-creation-by-non-admins}

[[!UICONTROL 允许公共集合创建]](../using/brand-portal-share-collection.md#main-pars-text-1915052376) 、配置控制非管理员是否可以在Brand Portal上创建公共集合。 默认情况下，该配置处于启用状态。 通过禁用配置，组织可以防止在其门户上拥有大量公共集合，以便保存系统空间。

## 允许非管理员创建公共智能收藏集 {#allow-public-smart-collections-creation-by-non-admins}

[[!UICONTROL 允许公共智能收藏集创建]](../using/brand-portal-searching.md#main-pars-header-500620467) ，配置控制非管理员是否可以将其搜索另存为智能收藏集，并将其公开给该租户。 默认情况下，该配置处于启用状态。 通过禁用配置，组织可以防止组织的品牌门户上有大量非管理员用户创建的公共智能集合。

## 允许下载加速 {#allow-download-acceleration}

[[!UICONTROL 允许下载加速配置]](../using/accelerated-download.md) ，使组织能够通过与IBM Aspera connect（按需安装的应用程序）集成，加快从Brand Portal和共享链接下载资产的速度。 该应用程序使用专有技术来消除TCP开销。

## 启用文件夹层次结构 {#enable-folder-hierarchy}

[[!UICONTROL 启用文件夹层次结构]](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) ，管理员可以控制非管理员用户（编辑器、查看器和来宾用户）在登录后如何查看共享文件夹。
