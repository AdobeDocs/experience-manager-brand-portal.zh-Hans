---
title: 管理常规租户配置
seo-title: 管理常规租户配置
description: 配置下载加速、公共智能集合创建、公共集合创建，并允许管理员用户删除租户上的资产。
seo-description: 配置下载加速、公共智能集合创建、公共集合创建，并允许管理员用户删除租户上的资产。
uuid: 3c46cd7c-c38b-4bc7-b566-93f977bc8227
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f4c237bc-f6a4-4bc4-af56-3d9c3027daf4
role: 管理员
translation-type: tm+mt
source-git-commit: 263653916e4bc183827c197c3beb137c9e59ccb1
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 4%

---


# 管理常规租户配置 {#administer-general-tenant-configurations}

AEM Assets Brand Portal允许组织为特定租户配置以下功能：

* 管理员删除资产
* 非管理员用户创建公共集合
* 非管理员用户创建公共智能收藏集
* 对非管理员用户可见的共享文件夹的父层次结构

这些配置已作为&#x200B;**[!UICONTROL “一般设置”]**&#x200B;配置在管理工具面板上提供。

![](assets/general-config.png)

**允**   许管理员从Brand Portal中删除资源的配置。（默认为启用）

**允许**   非管理员用户创建公共集合的BConfiguration。（默认为启用）

**配**   置允许非管理员用户创建公共智能集合。（默认为启用）

**配置**  ：向非管理员用户（编辑器、查看器、来宾用户）显示共享文件夹的文件夹层次结构（从根文件夹）。（默认为禁用）

## 启用/禁用常规配置{#enable-disable-general-configurations}

要启用/禁用以下各种配置：

1. 以管理员权限登录。
1. 从顶部的工具栏中选择AEM徽标以访问管理工具。
1. 从管理工具面板中，选择&#x200B;**[!UICONTROL 常规]**&#x200B;以打开&#x200B;**[!UICONTROL 常规设置]**&#x200B;页。
1. 使用相应的切换开关启用/禁用任何常规配置。
1. **[!UICONTROL 保存更改。]**
1. 注销以使更改生效。

## 允许管理员用户从Brand Portal {#allow-admin-users-to-delete-assets-from-brand-portal}中删除资产

**[!UICONTROL 允许用户删]** 除配置使组织能够允许（或限制）具有管理员权限的用户从Brand Portal中删除资产和文件夹。

## 允许非管理员创建公共集合{#allow-public-collections-creation-by-non-admins}

[[!UICONTROL 允许创建公共]](../using/brand-portal-share-collection.md#main-pars-text-1915052376) 集合配置控制非管理员是否可以在Brand Portal上创建公共集合。默认情况下，配置处于启用状态。 通过禁用配置，组织可以阻止在其门户上拥有大量公共集合，以便保存系统空间。

## 允许非管理员创建公共智能集合{#allow-public-smart-collections-creation-by-non-admins}

[[!UICONTROL 允许公共智能集]](../using/brand-portal-searching.md#main-pars-header-500620467) 合创建配置控制非管理员是否可以将其搜索另存为智能集合并公开给该租户。默认情况下，配置处于启用状态。 通过禁用配置，组织可以防止组织的Brand Portal上存在大量由非管理员用户创建的公共智能集合。

<!-- 
## Allow download acceleration {#allow-download-acceleration}

[[!UICONTROL Allow download acceleration]](../using/accelerated-download.md) configuration lets the organizations to allow accelerated downloads of assets from Brand Portal and shared links, by integrating with IBM Aspera Connect that is an install-on-demand application. The application uses proprietary technology to remove TCP overheads.
-->

## 启用文件夹层次结构 {#enable-folder-hierarchy}

[[!UICONTROL “启用文]](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) 件夹分层结构”配置允许管理员控制非管理员用户（编辑者、查看者和来宾用户）在登录后如何查看共享文件夹。
