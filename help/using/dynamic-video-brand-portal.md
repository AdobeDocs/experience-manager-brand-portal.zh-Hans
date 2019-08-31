---
title: Brand Portal上的动态视频支持
seo-title: Brand Portal上的动态视频支持
description: Brand Portal上的动态视频支持
seo-description: Brand Portal上的动态视频支持
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: murati
products: SG_ EXPERIENCE MANAGER/Brand_ Portal
content-type: 引用
topic-tags: 下载安装
discoiquuid: e18d992a-a3 b5-45f2-9696-81693213ee
translation-type: tm+mt
source-git-commit: d605cdd0083e8e222a3c937ea91d2c04201ab99b

---


# Brand Portal上的动态视频支持 {#dynamic-video-support-on-brand-portal}

借助Dynamic Media支持在Brand Portal上自适应地预览和播放视频。还可以从门户和共享链接下载动态演绎版。
Brand Portal用户可以：

* 在“资产详细信息”页面、卡片视图和链接共享预览页面中预览视频。
* 在“资产详细信息”页面上播放视频编码。
* 在资产详细信息页面的演绎版选项卡中查看动态演绎版。
* 下载视频编码和包含视频的文件夹。

>[!NOTE]
>
>要处理视频并将其发布到Brand Portal，请确保您的AEM作者实例在Dynamic Media混合模式或Dynamic Media [!DNL Scene 7] 模式下设置。

要预览、播放和下载视频，Brand Portal向管理员展示以下两种配置：

* [Dynamic Media混合配置](#configure-dm-hybrid-settings)(如果AEM作者实例正在动态媒体混合模式下运行)。
* [Dynamic Media[！DNL Scene7]配置(](#configure-dm-scene7-settings)如果AEM作者实例正在动态媒体模式[!DNL Scene 7] 上运行)。
根据您在AEM作者实例中设置的配置(复制Brand Portal租户)设置这些配置之一。

>[!NOTE]
>
>Brand Portal租户在 [!UICONTROL Scene Connect] 运行模式上运行的AEM作者上不支持动态视频。

## 动态视频是如何播放的？ {#how-are-dynamic-videos-played}

![从云获取视频编码](assets/VideoEncodes.png)

如果Dynamic Media配置([混合](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) 或 [[！DNL Scene7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) 配置设置在Brand Portal上，从 [!DNL Scene 7] 服务器获取动态演绎版。因此，视频编码可以在不延迟和扭曲的情况下预览和播放。

由于视频编码不存储在Brand Portal存储库中并从 [!DNL Scene 7] 服务器获取，因此请确保AEM作者实例和Brand Portal上的Dynamic Media配置相同。

>[!NOTE]
>
>Brand Portal不支持视频查看器和查看器预设。在Brand Portal的默认查看器上预览和播放视频。

## 先决条件 {#prerequisites}

要在Brand Portal上处理动态视频，请确保：

* **在DM(Dynamic Media)模式**&#x200B;启动AEM作者实例(通过 [Dynamic
Media混合模式启动AEM作者实例)](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) 或 [Dynamic Media[！DNL Scene7]模式](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode)。
* **根据AEM作者在运行的动态媒体模式在AEM作者**上配置Dynamic
Media云服务，设置 [Dynamic Media云服务](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) 或 [[！从工具上AEM作者](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) 上的DNL **Scene]云服务** || **云服务** || **Dynamic Media**。
* **在品牌门户**上配置Dynamic
Media基于AEM作者上的动态媒体云配置，配置 [Dynamic Media设置](#configure-dm-hybrid-settings) 或 [[！DNL Scene7]来自](#configure-dm-scene7-settings) Brand Portal管理工具的设置。
如果您使用Dynamic Media混合和Dynamic Media S的功能， [请确保单独的Brand Portal租户](#separate-tenants) 用于使用Dynamic Media混合和Dynamic Media [!UICONTROL Scene] 模式配置的AEM作者实例 。
* **使用应用于Brand Portal的视频编码发布文件夹**，应用 [视频编码](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) 并将包含多媒体资源的文件夹从AEM作者实例发布到Brand
Portal。
* **如果在启用了安全预览的情况下**启用了SPS中的白名单IP，则如果使用Dynamic
Media-[!DNL Scene 7] (为 [某公司启用](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) 安全预览)，建议 [!DNL Scene 7] 公司管理员 [白名单使用SPS(](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)[!UICONTROL Scene] Publishing System) flash UI为各个区域添加公共退出IP。
Egles IPS如下所示：

| **区域** | **EgleS IP** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

要列入上述电子邮件地址之一，请参阅 [准备用于安全测试服务](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)的帐户。

## 最佳实践

要确保您的动态视频资产在“品牌门户”(和共享链接)中成功预览、播放和下载，请遵循以下做法：

### Dynamic Media混合和Dynamic Media Scene模式的单独租户 {#separate-tenants}

如果您同时使用Dynamic Media [!DNL Scene 7] 和Dynamic Media混合功能，建议对使用Dynamic Media混合和Dynamic Media [!DNL Scene 7] 模式配置的AEM作者实例使用不同的Brand Portal租户。
![作者和BP一至一映射](assets/BPDynamicMedia.png)

### AEM作者实例和Brand Portal中的相同配置详细信息

确保配置详细信息( [!UICONTROL 如标题]、 [!UICONTROL 注册ID]、 [!UICONTROL 视频服务URL] (在 [!UICONTROL Dynamic Media混合中])和 [!UICONTROL 标题]、凭据([!UICONTROL 电子邮件] 和密码)、 [!UICONTROL 区域]、 [!UICONTROL 公司] (Dynamic Media [!DNL Scene 7]中)在Brand Portal和 [!UICONTROL AEM云配置]中)相同)。

### 针对Dynamic Media Scene模式的白名单公共退出IP

如果已使用Dynamic Media [Scene7-have安全预览功能](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)向Brand Portal提供视频资源， [!UICONTROL 则Scene会] 为stage环境或内部应用程序建立专用的图像服务器。对此服务器发出的任何请求都将检查源IP地址。如果传入请求未在IP地址的批准列表内，则返回失败响应。
因此 [!UICONTROL ，Scene-7] Company管理员通过SPS(Scene-7Publishing System) Flash UI为其公司 [!UICONTROL 的安全测试] 环境配置  已批准的IP地址列表。确保您的相应区域(来自以下)的退出IP已添加到该批准列表。
要列入上述电子邮件地址之一，请参阅 [准备用于安全测试服务](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)的帐户。
退出IP如下所示：

| **区域** | **EgleS IP** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## 配置Dynamic Media(混合)设置 {#configure-dm-hybrid-settings}

如果AEM作者实例在动态媒体混合模式上运行，则使用 [!UICONTROL 来自管理工具面板的视频] 拼贴，以配置Dynamic Media网关设置。
>[!NOTE]
>
>[视频编码配置文件](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) 未发布到Brand Portal，而是从 [!UICONTROL Scene] 服务器获取。因此，要在Brand Portal中成功播放视频编码，请确保配置详细信息与[ [！UICCONTRL Scene云配置]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) 在AEM作者实例中。
要在Brand Portal租户上设置Dynamic Media配置，请执行以下操作：

1. 从Brand Portal顶部的工具栏中选择AEM徽标以访问管理工具。

2. 从管理工具面板中，选择 **[!UICONTROL 视频]** 拼贴。<br />
   ![Brand Portal上的动态媒体混合配置](assets/DMHybrid-Video.png)
   **[!UICONTROL 此时将打开“编辑Dynamic Media配置]** ”页面。<br />
   ![Brand Portal上的动态媒体混合配置](assets/edit-dynamic-media-config.png)

3. 指定 **[!UICONTROL 注册ID]** 和 **[!UICONTROL 视频服务URL]** (DM-Gateway URL)。确保这些详细信息与AEM创作实例中 **[!UICONTROL 工具&gt;云服务]** 中的详细信息相同。

4. 选择 **保存** 以保存配置。

## 配置Dynamic Media Scene设置 {#configure-dm-scene7-settings}

如果AEM作者实例在Dynamic Media- [!UICONTROL Scene] 模式下运行，则使用 **[!UICONTROL 管理工具面板中的Dynamic Media配置]** 拼贴配置 [!UICONTROL Scene] 服务器设置。

要在Brand Portal租户上设置Dynamic Media [!UICONTROL Scene] 配置，请执行以下操作：

1. 从Brand Portal顶部的工具栏中选择AEM徽标以访问管理工具。

2. 从管理工具面板中，选择 **[!UICONTROL Dynamic Media配置]** 拼贴。<br />
   ![Brand Portal上的DM [!UICONTROL Scene] 配置](assets/DMS7-Tile.png)
   [!UICONTROL 此时将打开“编辑Dynamic Media配置] ”页面。<br />
   ![Scene在Brand Portal上的配置](assets/S7Config.png)

3. 提供：
   * [!UICONTROL 标题]
   * 用于访问Scene服务器的凭据([!UICONTROL 电子邮件ID] 和 [!UICONTROL 密码])
   * [!UICONTROL 区域]确保这些值与AEM作者实例中的值相同。

4. Select **[!UICONTROL Connect to Dynamic Media]**.

5. 提供 **[!UICONTROL 公司名称]**&#x200B;并 **[!UICONTROL 保存]** 配置。
