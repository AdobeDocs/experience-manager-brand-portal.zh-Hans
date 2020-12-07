---
title: Brand Portal 上的动态视频支持
seo-title: Brand Portal 上的动态视频支持
description: Brand Portal 上的动态视频支持
seo-description: Brand Portal 上的动态视频支持
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
translation-type: tm+mt
source-git-commit: b69025074080b83ac699da434fc525fea1cb100a
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 3%

---


# Brand Portal 上的动态视频支持 {#dynamic-video-support-on-brand-portal}

借助Dynamic Media支持，在品牌门户上自适应地预览和播放视频。 同时从门户和共享链接下载动态演绎版。
Brand Portal用户可以：

* 预览资产详细信息页面、卡片视图和链接共享预览页面中的视频。
* 在“资产详细信息”页面上播放视频编码。
* 视图资产详细信息页面的演绎版选项卡中的动态演绎版。
* 下载包含视频的视频编码和文件夹。

>[!NOTE]
>
>要处理视频并将其发布到Brand Portal，请确保在Dynamic Media Hybrid模式或Dynamic Media **[!DNL Scene 7]**&#x200B;模式上设置AEM作者实例。

为了预览、播放和下载视频，Brand Portal向管理员公开以下两种配置：

* [动态媒体混](#configure-dm-hybrid-settings)
合配置如果AEM作者实例在动态媒体混合模式下运行。
* [动态 [!DNL Scene 7] ](#configure-dm-scene7-settings)
媒体配置如果AEM作者实例在动态媒体模式下**[!DNL Scene 7]** 运行。根据您在AEM作者实例中设置的配置设置其中任一配置，该实例中将复制Brand Portal租户。

>[!NOTE]
>
>Brand Portal租户不支持使用在&#x200B;**[!UICONTROL Scene7Connect]**&#x200B;运行模式上运行的AEM作者配置的动态视频。

## 动态视频如何播放？{#how-are-dynamic-videos-played}

![从云中获取视频编码](assets/VideoEncodes.png)

如果在Brand Portal上设置了Dynamic Media配置（[Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings)或[[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings)配置），则从&#x200B;**[!DNL Scene 7]**&#x200B;服务器获取动态演绎版。 因此，视频编码在质量上没有延迟和扭曲地被预览和播放。

由于视频编码不存储在Brand Portal存储库中，并从&#x200B;**[!DNL Scene 7]**&#x200B;服务器获取，请确保AEM作者实例和Brand Portal上的Dynamic Media配置相同。

>[!NOTE]
>
>Brand Portal不支持视频查看器和查看器预设。 视频在品牌门户的默认查看器上预览和播放。

## 前提条件 {#prerequisites}

要在Brand Portal上处理动态视频，请确保：

* **在DM(Dynamic Media)模式下开始AEM作**
者在Dynamic Media Hybrid模式或Dynamic Mediamode上启 [动AEM作者实例(配](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) 置了Brand  [Portal) [!DNL Scene 7] ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode)。
* **在AEM上配置Dynamic Media云服**
务基于Dynamic Media模式，AEM作者正在运行，设置 [Dynamic Media ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) Cloud服务或Dynamic Cloud服务 [[!DNL Scene 7] 从AEM工具Cloud Services的Dynamic Cloud Cloud服务或Dynamic Media ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices)  ****  ****  **** Author的动态媒体|
* **在Brand Portal上配置Dynamic Media根**
据AEM Author上的Dynamic Media云配置，从Brand Portal管 [理工](#configure-dm-hybrid-settings) 具中配 [[!DNL Scene 7] ](#configure-dm-scene7-settings)  置Dynamic Media设置或设置。如果您使用Dynamic Media Hybrid和Dynamic Media的功能&#x200B;**[!UICONTROL S7]**，请确保将[单独的Brand Portal租户](#separate-tenants)用于配置有Dynamic Media Hybrid和Dynamic Media **[!UICONTROL Scene7]**&#x200B;模式的AEM作者实例。
* **使用应用于Brand Portal的视频编码发**
布文件夹应 [用视](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) 频编码，并将包含富媒体资产的文件夹从AEM Author实例发布到Brand Portal。
* **启允许列表用安全预览允许列表时，在SPS中出口IP如果使用Dynamic Media**
-(启用安全**[!DNL Scene 7]** 预览来 [公司)，建议管理员使用SPS Publishing Scene 7Flash System Ui对公共出](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)  **[!DNL Scene 7]**  [](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) **** 口IP进行公司。出口IP如下所示：

| **区域** | **出口IP** |
|--- |--- |
| NA | 130.248.160.66, 52.151.32.108 |
| EMEA | 185.34.189.1 |
| APAC | 63.140.44.54 |

要允许列出其中任何一个输出IP，请参阅[准备安全测试服务的帐户](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)。

## 最佳实践

要确保您的动态视频资产能够从Brand Portal（和共享链接）中成功预览、播放和下载，请遵循以下惯例：

### Dynamic Media Hybrid和Dynamic Media Scene 7模式的单独租户{#separate-tenants}

如果您同时使用Dynamic Media **[!DNL Scene 7]**&#x200B;和Dynamic Media Hybrid功能，建议您对使用Dynamic Media Hybrid和Dynamic Media **[!DNL Scene 7]**&#x200B;模式配置的AEM作者实例使用不同的Brand Portal租户。<br />

![作者与BP一对一映射](assets/BPDynamicMedia.png)

### AEM作者实例和Brand Portal中的相同配置详细信息

确保配置详细信息——如&#x200B;**[!UICONTROL 标题]**、**[!UICONTROL 注册ID]**、**[!UICONTROL 视频服务URL]**（在&#x200B;**[!UICONTROL 动态媒体混合]**&#x200B;中）和&#x200B;**[!UICONTROL 标题]**、凭据（**[!UICONTROL 电子邮件]**&#x200B;和密码）、**[!UICONTROL 区域]**、**[!UICONTROL 公司]**（在Dynamic Media **[!DNL Scene 7]**&#x200B;中）-在Brand Portal和&#x200B;**[!UICONTROL AEM云配置]**&#x200B;中是相同的。

### 为允许列表Dynamic Media Scene 7模式管理公共出口IP

如果使用启用[安全预览的Dynamic Media **[!UICONTROL Scene 7]**&#x200B;将视频资产提供给Brand Portal，则&#x200B;**[!UICONTROL Scene 7]**&#x200B;将建立专用的图像服务器来暂存环境或内部应用程序。 ](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)对此服务器的任何请求都检查来源IP地址。 如果传入请求不在IP地址的批准列表内，则返回失败响应。
因此，**[!UICONTROL Scene-7]**&#x200B;公司管理员通过&#x200B;**[!UICONTROL SPS]**(Scene-7 Publishing System)flash UI为公司的&#x200B;**[!UICONTROL 安全测试]**环境配置IP地址的批准列表。 确保将您各自区域的出口IP（来自以下区域）添加到该批准的列表。
要允许列出其中任何一个输出IP，请参阅[准备安全测试服务的帐户](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)。
输出IP如下：

| **区域** | **出口IP** |
|--- |--- |
| NA | 130.248.160.66, 52.151.32.108 |
| EMEA | 185.34.189.1 |
| APAC | 63.140.44.54 |

## 配置Dynamic Media(Hybrid)设置{#configure-dm-hybrid-settings}

如果AEM作者实例在Dynamic Media混合模式下运行，则使用管理工具面板中的&#x200B;**[!UICONTROL 视频]**&#x200B;拼贴来配置Dynamic Media网关设置。

>[!NOTE]
>
>[视频编码用户档案](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html)未发布到Brand Portal，而是从&#x200B;**[!UICONTROL Scene 7]**&#x200B;服务器获取。 因此，要在Brand Portal中成功播放视频编码，请确保配置详细信息与AEM作者实例中的[[!UICONTROL Scene7云配置]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices)相同。

要在Brand Portal租户上设置Dynamic Media配置，请执行以下操作：

1. 从顶部的工具栏中选择AEM徽标以访问品牌门户中的管理工具。
1. 从管理工具面板中，选择&#x200B;**[!UICONTROL 视频]**&#x200B;拼贴。

   ![Brand Portal上的Dynamic Media混合配置](assets/DMHybrid-Video.png)

   **[!UICONTROL “编辑Dynamic Media]** 配置”页打开。

   ![品牌门户上的动态媒体混合配置](assets/edit-dynamic-media-config.png)

1. 指定&#x200B;**[!UICONTROL 注册ID]**&#x200B;和&#x200B;**[!UICONTROL 视频服务URL]**（DM-网关URL）。 确保这些详细信息与AEM作者实例中的&#x200B;**[!UICONTROL 工具>Cloud Services]**&#x200B;中的详细信息相同。
1. 选择&#x200B;**保存**&#x200B;以保存配置。

## 配置Dynamic MediaScene7设置{#configure-dm-scene7-settings}

如果AEM作者实例在Dynamic Media- **[!UICONTROL Scene 7]**&#x200B;模式下运行，则使用管理工具面板中的&#x200B;**[!UICONTROL Dynamic Media配置]**&#x200B;磁贴来配置&#x200B;**[!UICONTROL Scene 7]**&#x200B;服务器设置。

要在Brand Portal租户上设置Dynamic Media **[!UICONTROL Scene 7]**&#x200B;配置，请执行以下操作：

1. 从顶部的工具栏中选择AEM徽标以访问品牌门户中的管理工具。

2. 从管理工具面板中，选择&#x200B;**[!UICONTROL Dynamic Media配置]**&#x200B;拼贴。<br />
   ![品牌 [!UICONTROL 门户] 上的DM Scene 7配置](assets/DMS7-Tile.png)
   **[!UICONTROL “编辑Dynamic Media]** 配置”页打开。<br />
   ![Brand Portal上的Scene 7配置](assets/S7Config.png)

3. 提供：
   * **[!UICONTROL 标题]**
   * 访问Scene 7服务器的凭据（**[!UICONTROL 电子邮件ID]**&#x200B;和&#x200B;**[!UICONTROL 密码]**）
   * **[!UICONTROL 区]**
域确保这些值与AEM作者实例中的值相同。

4. 选择&#x200B;**[!UICONTROL 连接到Dynamic Media]**。

5. 提供&#x200B;**[!UICONTROL 公司名称]**&#x200B;和&#x200B;**[!UICONTROL 保存]**&#x200B;配置。
