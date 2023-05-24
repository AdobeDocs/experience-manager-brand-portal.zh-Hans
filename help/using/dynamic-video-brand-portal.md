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
source-git-commit: f56918ea8eb14ba04b7e141f4f1cae318e532512
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 4%

---

# Brand Portal 上的动态视频支持 {#dynamic-video-support-on-brand-portal}

借助Dynamic Media支持，可在Brand Portal上自适应预览和播放视频。 此外，还可以从门户和共享链接下载动态演绎版。
Brand Portal用户可以：

* 在“资产详细信息”页面、“卡片视图”和链接共享预览页面中预览视频。
* 在“资源详细信息”页面上播放视频编码。
* 在“资源详细信息”页面的“演绎版”选项卡中查看动态演绎版。
* 下载视频编码和包含视频的文件夹。

>[!NOTE]
>
>要使用视频并将其发布到Brand Portal，请确保在Dynamic Media混合模式或Dynamic Media上设置了您的Experience Manager创作实例 **[!DNL Scene7]** 模式。

要预览、播放和下载视频，Brand Portal向管理员公开以下两个配置：

* [Dynamic Media混合配置](#configure-dm-hybrid-settings)
如果Experience Manager创作实例在Dynamic Media混合模式下运行。
* [Dynamic Media [!DNL Scene7] 配置](#configure-dm-scene7-settings)
如果Experience Manager创作实例在Dynamic Media上运行 — **[!DNL Scene7]** 模式。
根据您在Brand Portal租户复制的Experience Manager创作实例中设置的配置，设置这些配置中的任意一个。

>[!NOTE]
>
>运行Experience Manager创作的Brand Portal租户不支持动态视频 **[!UICONTROL Scene7Connect]** 运行模式。

## 如何播放动态视频？ {#how-are-dynamic-videos-played}

![从云中获取视频编码](assets/VideoEncodes.png)

如果Dynamic Media配置([混合](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) 或 [[!DNL Scene7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) Brand Portal配置)，动态演绎版获取自 **[!DNL Scene7]** 服务器。 因此，视频编码被预览和播放，没有延迟和质量失真。

由于视频编码不存储在Brand Portal存储库中，而是从中获取 **[!DNL Scene7]** 服务器，请确保Adobe Experience Manager创作实例和Brand Portal上的Dynamic Media配置相同。

>[!NOTE]
>
>Brand Portal不支持视频查看器和查看器预设。 在Brand Portal中的默认查看者上预览和播放视频。

## 前提条件 {#prerequisites}

要在Brand Portal上使用动态视频，请确保：

* **在Dynamic Media模式下启动Experience Manager创作**
在中启动Experience Manager创作实例(已配置Brand Portal) [DYNAMIC MEDIA - [!DNL Scene7] 模式](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=en#enabling-dynamic-media-in-scene-mode) 或位于 [Dynamic Media — 混合模式](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) 或
* **在Experience Manager创作中配置Dynamic MediaCloud Services**
根据“创作”运行所在的Dynamic Media模式(Scene7Experience Manager模式或混合模式)，设置 [Dynamic MediaCloud Services([!DNL Scene7] mode)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=zh-Hans#configuring-dynamic-media-cloud-services) 或 [Dynamic MediaCloud Services（混合模式）](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html?lang=en#configuring-dynamic-media-cloud-services) Experience Manager创作自 **工具** | **Cloud Services** | **Dynamic Media**.
* **在Brand Portal上配置Dynamic Media**
根据Experience Manager作者的Dynamic Media云配置，配置 [Dynamic Media设置](#configure-dm-hybrid-settings) 或 [[!DNL Scene7] 设置](#configure-dm-scene7-settings) 从Brand Portal管理工具。
确保 [单独的Brand Portal租户](#separate-tenants) 用于在Dynamic Media中配置的Experience Manager创作实例 —  **[!UICONTROL Scene7]** 模式和Dynamic Media — 混合模式。 特别是如果您使用Dynamic Media的功能 **[!UICONTROL S7]** 和Dynamic Media Hybrid。
* **将视频编码应用于Brand Portal的发布文件夹**
应用 [视频编码](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) 并将包含富媒体资产的文件夹从Experience Manager创作实例发布到Brand Portal。
* **如果启用了安全预览，则SPS中的允许列表出口IP**
如果使用Dynamic Media-**[!DNL Scene7]** (带 [已启用安全预览](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) （对于公司），则建议 **[!DNL Scene7]** 公司管理员 [允许列表公共出口IP](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) 对于使用SPS的各个区域(**[!UICONTROL Scene7]** Publishing System) flash UI。
出口IP如下所示：

| **区域** | **出口IP** |
|--- |--- |
| NA | 130.248.160.68,  20.94.203.130 |
| EMEA | 185.34.189.3,  51.132.146.75 |
| 亚太地区 | 63.140.44.54 |

要将其中任意一个出口IP列入允许列表，请参见 [为安全测试服务准备帐户](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## 最佳实践

要确保从Brand Portal（和共享链接）成功预览、播放和下载您的动态视频资产，请遵循以下实践：

### 分隔Dynamic Media的租户 — Scene7和Dynamic Media — 混合模式 {#separate-tenants}

如果您同时使用两个Dynamic Media - **[!DNL Scene7]** 模式和Dynamic Media — 混合模式功能，为使用Dynamic Media配置的Experience Manager创作实例使用不同的Brand Portal租户 —  **[!DNL Scene7]** 和Dynamic Media — 混合模式。


![作者和BP一对一映射](assets/BPDynamicMedia.png)

### Experience Manager创作实例和Brand Portal中的相同配置详细信息

确保Brand Portal中的配置详细信息与 **[!UICONTROL Experience Manager云配置]**. 相同的配置详细信息包括：

* **[!UICONTROL 标题]**
* **[!UICONTROL 注册 ID]**
* **[!UICONTROL 视频服务URL]** 在 **[!UICONTROL Dynamic Media — 混合模式]**
* **[!UICONTROL 标题]**
* 凭据(**[!UICONTROL 电子邮件]** 和密码)
* **[!UICONTROL 区域]**
* **[!UICONTROL 公司]** 在Dynamic Media中 —  **[!DNL Scene7]** 模式

### Dynamic Media Scene7模式的允许列表公共出口IP

如果Dynamic Media **[!UICONTROL Scene7]** — 具有 [已启用安全预览](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) — 用于向Brand Portal提供视频资源，然后 **[!UICONTROL Scene7]** 为暂存环境或内部应用程序建立专用映像服务器。 对此服务器的任何请求都会检查原始IP地址。 如果传入请求不在已批准的IP地址列表中，则会返回失败响应。
此 **[!UICONTROL Scene7]** 因此，公司管理员为其公司的IP地址配置一个经批准的IP地址列表 **[!UICONTROL 安全测试]** 环境，通过 **[!UICONTROL SPS]** (Scene7 Publishing System) flash UI。 确保将相应区域（来自以下位置）的出口IP添加到该批准列表中。
要将其中任意一个出口IP列入允许列表，请参见 [为安全测试服务准备帐户](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
出口IP如下所示：

| **区域** | **出口IP** |
|--- |--- |
| NA | 130.248.160.66, 20.94.203.130 |
| EMEA | 51.132.146.75, 130.248.244.202, 130.248.244.203, 130.248.244.204, 130.248.244.210, 130.248.244.211, 130.248.244.212 |
| 亚太地区 | 63.140.44.54 |

## 配置Dynamic Media（混合）设置 {#configure-dm-hybrid-settings}

如果Experience Manager创作实例在Dynamic Media混合模式下运行，则使用 **[!UICONTROL 视频]** 从“管理工具”面板中拼贴，以配置Dynamic Media网关设置。

>[!NOTE]
>
>此 [视频编码配置文件](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) 不会发布到Brand Portal，而是会从 **[!UICONTROL Scene7]** 服务器。 因此，对于要在Brand Portal中成功播放的视频编码，请确保配置详细信息与 [Dynamic MediaCloud Services([!DNL Scene7] mode)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=zh-Hans#configuring-dynamic-media-cloud-services) 在您的Experience Manager创作实例中。

要在Brand Portal租户上设置Dynamic Media配置，请执行以下操作：

1. 选择Experience Manager徽标，以便您可以从顶部工具栏的Brand Portal中访问管理工具。
1. 从管理工具面板中，选择 **[!UICONTROL 视频]** 图块。

   ![Brand Portal上的Dynamic Media混合配置](assets/DMHybrid-Video.png)

   **[!UICONTROL 编辑Dynamic Media配置]** 页面打开。

   ![Brand Portal上的Dynamic Media混合配置](assets/edit-dynamic-media-config.png)

1. 指定 **[!UICONTROL 注册ID]** 和 **[!UICONTROL 视频服务URL]** (DM-Gateway URL)。 确保这些详细信息与中的这些详细信息相同 **[!UICONTROL “工具”>“Cloud Services”]** 在您的Experience Manager创作实例中。
1. 选择 **保存** 以保存配置。

## 配置Dynamic Media Scene7设置 {#configure-dm-scene7-settings}

如果Experience Manager创作实例在Dynamic Media上运行 —  **[!UICONTROL Scene7]** 模式，然后使用 **[!UICONTROL Dynamic Media配置]** 从“管理工具”面板中拼贴以配置 **[!UICONTROL Scene7]** 服务器设置。

设置Dynamic Media **[!UICONTROL Scene7]** Brand Portal租户上的配置：

1. 选择Experience Manager徽标，以便您可以从顶部工具栏的Brand Portal中访问管理工具。

2. 从管理工具面板中，选择 **[!UICONTROL Dynamic Media配置]** 图块。

   ![DM [!UICONTROL 场景7] Brand Portal上的配置](assets/DMS7-Tile.png)

   **[!UICONTROL 编辑Dynamic Media配置]** 页面打开。

   ![Brand Portal上的Scene 7配置](assets/S7Config.png)

3. 提供：

   * **[!UICONTROL 标题]**
   * 凭据(**[!UICONTROL 电子邮件ID]** 和 **[!UICONTROL 密码]**)以访问Scene7服务器
   * **[!UICONTROL 区域]**

   确保这些值与在Experience Manager创作实例中找到的值相同。

4. 选择 **[!UICONTROL 连接到Dynamic Media]**.

5. 提供 **[!UICONTROL 公司名称]**、和 **[!UICONTROL 保存]** 配置。
