---
title: 配置资产来源补充
seo-title: 配置资产来源补充
description: 深入了解在AEM资产中配置资产来源补充功能。
seo-description: 深入了解在AEM资产中配置资产来源补充功能。
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: aa6bd187124888cd62ca1f5c7192f9d65ac6ca8a

---


# 配置资产来源补充 {#configure-asset-sourcing}

AEM管理员可以从 **AEM作者实例中配置资产来源补充** 。 管理员从 **AEM Web Console配置中启用资产来源补充功能标志配置** ，并在 **AEM资产中上传活动的Brand Portal用户列表**。

>[!NOTE]
>
>在开始配置之前，请确保AEM资产实例已配置Brand Portal。 请参阅， [配置AEM资产与Brand Portal](../using/configure-aem-assets-with-brand-portal.md)。


以下视频演示了如何在AEM作者实例上配置资产来源补充：

>[!VIDEO](https://video.tv.adobe.com/v/29771)

## 启用资产来源补充 {#enable-asset-sourcing}

AEM管理员可以从AEM Web控制台配置（即配置管理器）中启用资产来源补充。

**要启用资产来源补充，请执行以下操作：**
1. 登录AEM作者实例并打开配置管理器默认URL:http://本地主机：4502/system/console/configMgr
1. 使用关键字“资 **产来源补充** ”搜索以查 **[!UICONTROL 找“资产来源补充”功能标志配置]**
1. 单击 **[!UICONTROL 资产来源补充功能标记配置]** ，以打开配置窗口
1. 启用复 **[!UICONTROL 选框feature.flag.active.status]**
1. 单击&#x200B;**[!UICONTROL 保存]**。

![](assets/enable-asset-sourcing.png)

## 上传Brand Portal用户列表 {#upload-bp-user-list}

AEM管理员可以上传Brand Portal用户配置(.csv)文件，其中包含AEM资产中的活动Brand Portal用户列表。 贡献文件夹只能与用户列表中定义的活动Brand Portal用户共享。 管理员还可以在配置文件中添加新用户并上传修改后的用户列表。

>[!NOTE]
>
>CSV文件的格式与Admin Console支持的批量用户导入格式相同。 电子邮件、名字和姓氏是必填项。

管理员可以在AEM Admin Console中添加新用户，有关详细信 [息，请参阅](brand-portal-adding-users.md) “管理用户”。 在Admin Console中添加用户后，这些用户可以添加到Brand Portal用户配置文件，然后为其分配访问贡献文件夹的权限。

**要上传Brand Portal用户列表，请执行以下操作：**
1. 登录AEM作者实例默认URL:http://本地主机：4502/aem/start.html
1. 从“工 **具** ”面板 ![](assets/tools.png) ，导航到“资产”>“Brand Portal用 **[!UICONTROL 户”]**
   ![](assets/upload-user-list1.png)
1. Brand Portal上传参与者窗口将打开。
从您的本地计算机浏览并上 **传包含活动Brand Portal用户列表的配置(** .csv)文件。
1. 单击&#x200B;**[!UICONTROL 保存]**。
   ![](assets/upload-user-list2.png)


管理员可以在配置贡献文件夹时从此用户列表提供对特定用户／组的访问。

有关详细信息，请参阅 [配置贡献文件夹](brand-portal-contribution-folder.md)。
