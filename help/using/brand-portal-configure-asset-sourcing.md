---
title: 配置资产来源补充
seo-title: 配置资产来源补充
description: 深入了解在AEM Assets配置资产来源补充功能。
seo-description: 深入了解在AEM Assets配置资产来源补充功能。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 0a3f1a4379398730e92e9ac85b04134f92af9d23
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 1%

---


# 配置资产来源补充{#configure-asset-sourcing}

AEM管理员可以从AEM作者实例中配置&#x200B;**资产来源补充**。 管理员从&#x200B;**AEM Web控制台配置**&#x200B;启用资产来源补充功能标志配置，并上传&#x200B;**AEM Assets**&#x200B;中的活动品牌门户用户列表。

>[!NOTE]
>
>在开始配置之前，请确保您的AEM Assets实例已配置Brand Portal。 请参阅[使用Brand Portal配置AEM Assets](../using/configure-aem-assets-with-brand-portal.md)。

以下视频演示了如何在AEM作者实例上配置资产来源补充：

>[!VIDEO](https://video.tv.adobe.com/v/29771)

## 启用资产来源补充{#enable-asset-sourcing}

AEM管理员可以从AEM Web控制台配置（即配置管理器）中启用资产来源补充。

**要启用资产来源补充，请执行以下操作：**
1. 登录到AEM作者实例并打开Configuration Manager
默认URL:http:// localhost:4502/system/console/configMgr
1. 使用关键字&#x200B;**资产来源补充**&#x200B;搜索以找到&#x200B;**[!UICONTROL 资产来源补充功能标志配置]**
1. 单击&#x200B;**[!UICONTROL 资产来源补充功能标志配置]**&#x200B;以打开配置窗口
1. 选中&#x200B;**[!UICONTROL feature.flag.active.status]**&#x200B;复选框。
1. 单击&#x200B;**[!UICONTROL 保存]**。

![](assets/enable-asset-sourcing.png)

## 上传Brand Portal用户列表{#upload-bp-user-list}

AEM管理员可以上传包含AEM Assets活动Brand Portal用户列表的Brand Portal用户配置(.csv)文件。 贡献文件夹只能与用户列表中定义的活动Brand Portal用户共享。 管理员还可以在配置文件中添加新用户并上传修改后的用户列表。

>[!NOTE]
>
>CSV文件的格式与批量用户导入Admin Console中支持的格式相同。 电子邮件、名字和姓氏是必填项。

管理员可以在AEMAdmin Console中添加新用户，有关详细信息，请参阅[管理用户](brand-portal-adding-users.md)。 在Admin Console中添加用户后，可将这些用户添加到Brand Portal用户配置文件，然后为其分配访问贡献文件夹的权限。

**要上传Brand Portal用户列表，请执行以下操作：**
1. 登录到AEM作者实例
默认URL:http://本地主机：4502/aem/start.html
1. 从&#x200B;**工具**&#x200B;面板，导航到&#x200B;**[!UICONTROL 资产>品牌门户用户]**

   ![](assets/upload-user-list1.png)

1. 将打开“品牌门户上传参与者”窗口。
从本地机器浏览并上传包含活动Brand Portal用户列表的**配置(.csv)文件**。
1. 单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/upload-user-list2.png)


管理员可以在配置贡献文件夹时，通过此用户列表提供对特定用户的访问。

有关详细信息，请参阅[配置贡献文件夹](brand-portal-contribution-folder.md)。
