---
title: 配置资产来源补充
seo-title: 配置资产来源补充
description: 深入了解在AEM Assets中配置资产来源补充功能。
seo-description: 深入了解在AEM Assets中配置资产来源补充功能。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 1%

---


# 配置资产来源补充 {#configure-asset-sourcing}

AEM管理员可以从 **AEM作者实例** 中配置资产来源补充。 管理员从AEM Web Console配置中启用资产来源补充功 **能标志配置** ，并以列表形式上传活动的Brand **Portal用**&#x200B;户AEM Assets。

>[!NOTE]
>
>在开始配置之前，请确保AEM Assets实例已配置Brand Portal。 See, [Configure AEM Assets with Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

以下视频演示了如何在AEM作者实例上配置资产来源补充：

>[!VIDEO](https://video.tv.adobe.com/v/29771)

## 启用资产来源补充 {#enable-asset-sourcing}

AEM管理员可以从AEM Web控制台配置（又称配置管理器）中启用资产来源补充。

**要启用资产来源补充，请执行以下操作：**
1. 登录到AEM作者实例并打开Configuration Manager默认URL: http:// localhost:4502/system/console/configMgr
1. 使用关键字“资 **产来源补充** ”进行搜 **[!UICONTROL 索以查找资产来源补充功能标志配置]**
1. 单击 **[!UICONTROL 资产来源补充功能标志]** 配置以打开配置窗口
1. 启用复 **[!UICONTROL 选框feature.flag.active.status]**
1. 单击&#x200B;**[!UICONTROL 保存]**。

![](assets/enable-asset-sourcing.png)

## 上传Brand Portal用户列表 {#upload-bp-user-list}

AEM管理员可以上传包含AEM Assets中活动Brand Portal用户列表的Brand Portal用户配置(.csv)文件。 贡献文件夹只能与用户列表中定义的活动Brand Portal用户共享。 管理员还可以在配置文件中添加新用户并上传修改后的用户列表。

>[!NOTE]
>
>CSV文件的格式与批量用户导入Admin Console支持的格式相同。 电子邮件、名字和姓氏是必填项。

管理员可以在AEMAdmin Console中添加新用户，有关详细 [信息，请](brand-portal-adding-users.md) 参阅管理用户。 在Admin Console中添加用户后，可将这些用户添加到Brand Portal用户配置文件，然后为其分配访问贡献文件夹的权限。

**要上传Brand Portal用户列表，请执行以下操作：**
1. 登录AEM作者实例默认URL: http://本地主机：4502/aem/start.html
1. 从“工 **具** ”面板 ![](assets/tools.png) 中，导航到“资产”>“ **[!UICONTROL Brand Portal用户”]**
   ![](assets/upload-user-list1.png)
1. 将打开“品牌门户上传参与者”窗口。
从您的本地机器浏览并上 **传包含活动Brand Portal用户列表** 的配置(.csv)文件。
1. 单击&#x200B;**[!UICONTROL 保存]**。
   ![](assets/upload-user-list2.png)


管理员可以在配置贡献文件夹时，从此用户列表提供对特定用户／组的访问。

有关详细信息，请参 [阅配置贡献文件夹](brand-portal-contribution-folder.md)。
