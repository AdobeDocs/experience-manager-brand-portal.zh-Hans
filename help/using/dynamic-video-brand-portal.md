---
title: Brand Portal 上的动态视频支持
seo-title: Dynamic video support on Brand Portal
description: Brand Portal 上的动态视频支持
seo-description: Dynamic video support on Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
exl-id: 08d6a0fb-061e-4bef-b8e2-bb8522e7482e
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 2%

---

# Brand Portal 上的动态视频支持 {#dynamic-video-support-on-brand-portal}

在支持Dynamic Media的Brand Portal上自适应预览和播放视频。 此外，还可以从门户和共享链接下载动态演绎版。
Brand Portal用户可以：

* 在“资产详细信息”页面、卡片视图和链接共享预览页面中预览视频。
* 在“资产详细信息”页面上播放视频编码。
* 在资产详细信息页面的演绎版选项卡中查看动态演绎版。
* 下载视频编码和包含视频的文件夹。

>[!NOTE]
>
>要处理视频并将它们发布到Brand Portal，请确保在Dynamic Media混合模式或Dynamic Media **[!DNL Scene 7]**&#x200B;模式上设置了Experience Manager创作实例。

为了预览、播放和下载视频，Brand Portal向管理员提供了以下两种配置：

* [Dynamic Media混合](#configure-dm-hybrid-settings)
配置如果Experience Manager创作实例在Dynamic Media混合模式下运行。
* [Dynamic  [!DNL Scene 7] ](#configure-dm-scene7-settings)
Mediaconfiguration如果Experience Manager创作实例在Dynamic Media模式下运**[!DNL Scene 7]** 行。根据您在用于复制Brand Portal租户的Experience Manager创作实例中设置的配置，设置这些配置中的任一配置。

>[!NOTE]
>
>配置了在&#x200B;**[!UICONTROL Scene7Connect]**&#x200B;运行模式上运行“Experience Manager作者”的Brand Portal租户上不支持动态视频。

## 动态视频的播放方式是如何？ {#how-are-dynamic-videos-played}

![从云中获取视频编码](assets/VideoEncodes.png)

如果在Brand Portal上设置了Dynamic Media配置（[Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings)或[[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings)配置），则会从&#x200B;**[!DNL Scene 7]**&#x200B;服务器获取动态演绎版。 因此，视频编码可以在质量上没有延迟和失真地预览和播放。

由于视频编码未存储在Brand Portal存储库中，而是从&#x200B;**[!DNL Scene 7]**&#x200B;服务器获取，因此请确保AEM创作实例和Brand Portal上的Dynamic Media配置相同。

>[!NOTE]
>
>Brand Portal不支持视频查看器和查看器预设。 在Brand Portal的默认查看器上预览和播放视频。

## 前提条件 {#prerequisites}

要处理有关Brand Portal的动态视频，请确保：

* **在DM(Dynamic Media)模式下启动AEM创作**
在Dynamic Media混合模式或动态媒体模式下启动AEM创作实例( [已配](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) 置Brand Portal) [ [!DNL Scene 7] ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html)。
* **在AEM作者上配置**
Dynamic Media云服务根据运行AEM作者的Dynamic Media模式，从工具中设置 [Dynamic Media ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) 云服务或 [[!DNL Scene 7] ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html) 在AEM作者上 **设置云服务** |  **Cloud Services** |  **Dynamic Media**。
* **在Brand Portal上配置**
Dynamic Media基于AEM Author上的Dynamic Media云配置，从Brand Portal管理工具 [中配](#configure-dm-hybrid-settings) 置Dynamic Media [[!DNL Scene 7] ](#configure-dm-scene7-settings)  设置或设置。如果您使用的是Brand Portal Hybrid和Dynamic Media **[!UICONTROL S7]**&#x200B;的功能，请确保将[单独的Dynamic Media租户](#separate-tenants)用于配置了Dynamic Media Hybrid和Dynamic Media **[!UICONTROL Scene7]**&#x200B;模式的AEM创作实例。
* **发布应用了视频编码的文件夹**
应用 [视频](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) 编码，并将包含富媒体资产的文件夹从AEM创作实例发布到Brand Portal。
* **如果启允许列表用了安全预览，则在SPS中出口IP如果使**
用Dynamic Media- **[!DNL Scene 7]** (为公司启用 [安全](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) 预览)，则建议公司管理员使用SPS( **[!DNL Scene 7]** Scene 7 [Publishing System)闪存UI来](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) 为相应地区&#x200B;**[!UICONTROL 允许列表域]** 公共出口IP。出口IP如下：

| **区域** | **出口IP** |
|--- |--- |
| NA | 130.248.160.66, 52.151.32.108 |
| 欧洲、中东和非洲 | 185.34.189.1 |
| APAC | 63.140.44.54 |

要允许列出这些出口IP中的任一IP，请参阅[为安全测试服务准备帐户](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)。

## 最佳实践

要确保您的动态视频资产能够从Brand Portal（和共享链接）成功预览、播放和下载，请遵循以下实践：

### Dynamic Media混合和Dynamic Media Scene 7模式的单独租户 {#separate-tenants}

如果您同时使用Dynamic Media **[!DNL Scene 7]**&#x200B;和Dynamic Media混合功能，建议对于使用Dynamic Media混合和Dynamic Media **[!DNL Scene 7]**&#x200B;模式配置的AEM创作实例，使用不同的Brand Portal租户。


![作者与BP一对一映射](assets/BPDynamicMedia.png)

### 与AEM创作实例和Brand Portal中的配置详细信息相同

确保配置详细信息(如&#x200B;**[!UICONTROL 标题]**、**[!UICONTROL 注册ID]**、**[!UICONTROL 视频服务URL]**(在&#x200B;**[!UICONTROL Dynamic Media Hybrid]**&#x200B;中)和&#x200B;**[!UICONTROL 标题]**、凭据（**[!UICONTROL 电子邮件]**&#x200B;和密码）、**[!UICONTROL 区域]**、**[!UICONTROL 中的]**&#x200B;公司&#x200B;**[!DNL Scene 7]**) — 在Brand Portal和&#x200B;**[!UICONTROL AEM云配置]**&#x200B;中是相同的。

### 允许列表为Dynamic Media Scene 7模式管理公共出口IP

如果使用Dynamic Media **[!UICONTROL 具有[已启用安全预览的Scene 7]**&#x200B;将视频资产提供给Brand Portal，则&#x200B;**[!UICONTROL Scene 7]**&#x200B;会为暂存环境或内部应用程序建立专用的图像服务器。 ](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)对此服务器的任何请求都会检查源IP地址。 如果传入的请求不在批准的IP地址列表中，则返回失败响应。
因此， **[!UICONTROL Scene-7]**&#x200B;公司管理员通过&#x200B;**[!UICONTROL SPS]**(Scene-7 Publishing System)闪存UI为其公司的&#x200B;**[!UICONTROL Secure Testing]**环境配置一个已批准的IP地址列表。 确保将相应区域的出口IP（从以下来源）添加到该批准列表。
要允许列出这些出口IP中的任一IP，请参阅[为安全测试服务准备帐户](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)。
出口IP如下：

| **区域** | **出口IP** |
|--- |--- |
| NA | 130.248.160.66, 52.151.32.108 |
| 欧洲、中东和非洲 | 185.34.189.1 |
| APAC | 63.140.44.54 |

## 配置Dynamic Media（混合）设置 {#configure-dm-hybrid-settings}

如果AEM创作实例在Dynamic Media混合模式下运行，则使用管理工具面板中的&#x200B;**[!UICONTROL 视频]**&#x200B;拼贴来配置Dynamic Media网关设置。

>[!NOTE]
>
>[视频编码配置文件](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html)未发布到Brand Portal，而是从&#x200B;**[!UICONTROL Scene 7]**&#x200B;服务器获取。 因此，要在Brand Portal中成功播放视频编码，请确保配置详细信息与AEM创作实例中的[Scene7云配置](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html)相同。

要在Brand Portal租户上设置Dynamic Media配置，请执行以下操作：

1. 从顶部的Brand Portal工具栏中选择AEM徽标以访问管理工具。
1. 从管理工具面板中，选择&#x200B;**[!UICONTROL 视频]**&#x200B;拼贴。

   ![Dynamic Media Hybrid Config on Brand Portal](assets/DMHybrid-Video.png)

   **[!UICONTROL 编辑Dynamic Media]** 配置页面打开。

   ![Dynamic Media Brand Portal上的混合配置](assets/edit-dynamic-media-config.png)

1. 指定&#x200B;**[!UICONTROL 注册ID]**&#x200B;和&#x200B;**[!UICONTROL 视频服务URL]**(DM-Gateway URL)。 确保这些详细信息与AEM创作实例中的&#x200B;**[!UICONTROL 工具>Cloud Services]**&#x200B;中的相同。
1. 选择&#x200B;**Save**&#x200B;以保存配置。

## 配置Dynamic Media Scene7设置 {#configure-dm-scene7-settings}

如果AEM创作实例在Dynamic Media- **[!UICONTROL Scene 7]**&#x200B;模式下运行，则使用管理工具面板中的&#x200B;**[!UICONTROL Dynamic Media配置]**&#x200B;磁贴来配置&#x200B;**[!UICONTROL Scene 7]**&#x200B;服务器设置。

要在Brand Portal租户上设置Dynamic Media **[!UICONTROL Scene 7]**&#x200B;配置，请执行以下操作：

1. 从顶部的Brand Portal工具栏中选择AEM徽标以访问管理工具。

2. 从管理工具面板中，选择&#x200B;**[!UICONTROL Dynamic Media配置]**&#x200B;磁贴。

   ![Brand Portal [!UICONTROL 上的DM Scene 7] 配置](assets/DMS7-Tile.png)

   **[!UICONTROL 编辑Dynamic Media]** 配置页面打开。

   ![Brand Portal上的Scene 7配置](assets/S7Config.png)

3. 提供：

   * **[!UICONTROL 标题]**
   * 用于访问Scene 7服务器的凭据（**[!UICONTROL 电子邮件ID]**&#x200B;和&#x200B;**[!UICONTROL 密码]**）
   * **[!UICONTROL 区域]**

   确保这些值与AEM创作实例中的值相同。

4. 选择&#x200B;**[!UICONTROL 连接到Dynamic Media]**。

5. 提供&#x200B;**[!UICONTROL 公司名称]**&#x200B;和&#x200B;**[!UICONTROL 保存]**&#x200B;配置。
