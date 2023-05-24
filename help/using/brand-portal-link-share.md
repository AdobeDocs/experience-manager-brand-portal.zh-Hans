---
title: 以链接方式共享资产
seo-title: Share assets as a link
description: Adobe Experience Manager Assets Brand Portal管理员可以与授权内部用户和外部实体（包括合作伙伴和供应商）共享多个资源的链接。 编辑者只能查看和共享与他们共享的资产。
seo-description: Adobe Experience Manager Assets Brand Portal Administrators can share links of multiple assets with authorized internal users and external entities, including partners and vendors. Editors can view and share only the assets shared with them.
uuid: 8889ac24-c56d-4a47-b792-80c34ffb5c3f
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f3573219-3c58-47ba-90db-62b003d8b9aa
exl-id: 9d254e95-a4fc-468d-ae1f-9690ddd3b4a1
source-git-commit: e3e35ad4be5c082ad7bac7bed8ea20a186d245ad
workflow-type: tm+mt
source-wordcount: '969'
ht-degree: 4%

---

# 以链接方式共享资产 {#share-assets-as-a-link}

Adobe Experience Manager Assets Brand Portal管理员可以与授权内部用户和外部实体（包括合作伙伴和供应商）共享多个资源的链接。 编辑者只能查看和共享与他们共享的资产。

通过链接共享资源是一种向外部各方提供资源的便利方法，因为接收者无需登录Brand Portal即可访问资源。

<!-- Link sharing access is restricted to editors and administrators. 
-->

有关更多信息，请参阅 [管理用户、组和用户角色](../using/brand-portal-adding-users.md#manage-user-roles).


以下是作为链接共享资产的步骤：

1. 登录到您的Brand Portal租户。 默认情况下， **[!UICONTROL 文件]** 视图打开，其中包含所有已发布的资源和文件夹。

1. 选择要共享的资源或文件夹，或导航到 **[!UICONTROL 收藏集]** 查看以共享您已创建的收藏集。

   ![select-multi-assets](assets/select-assets-new.png)

1. 在顶部的工具栏中，单击 **[!UICONTROL 共享链接]** 图标。

   此 **[!UICONTROL 链接共享]** 对话框。

   ![](assets/link-sharing.png)

   * 在电子邮件地址框中，键入要与其共享链接的用户的电子邮件ID。 您可以与多个用户共享该链接。 如果用户是您组织的成员，请从下拉列表中显示的建议中选择其电子邮件ID。 如果用户是外部用户，请键入完整的电子邮件ID并按 **[!UICONTROL 输入]**；电子邮件ID将添加到用户列表。

      ![](assets/link-sharing-text.png)

   * 在 **[!UICONTROL 主题]** 框中，为要共享的资产键入主题。
   * 在 **[!UICONTROL 消息]** 框中，根据需要键入消息。
   * 在 **[!UICONTROL 过期]** 字段中，使用日期选取器指定链接的到期日期和时间。 默认情况下，到期日期设置为自您共享链接之日起的7天。
   * 启用 **[!UICONTROL 允许下载原始文件]** 复选框，允许收件人下载原始演绎版。

   通过链接共享的资产会在超过 **[!UICONTROL 过期]** 字段。 有关已过期资源的行为以及根据Brand Portal中的用户角色而允许的活动中的更改的信息，请参阅 [管理资产的数字权限](../using/manage-digital-rights-of-assets.md#asset-expiration).

   >[!NOTE]
   >
   >链接的默认到期时间为7天。 必须通过电子邮件将链接发送给使用 **[!UICONTROL 链接共享]** 对话框中，不要单独复制和共享链接。

1. 单击 **[!UICONTROL 共享]**. 将显示一条消息，确认该链接已与用户共享。 用户将收到包含共享链接的电子邮件。

   ![](assets/link-share-email.png)

   >[!NOTE]
   >
   >管理员可以自定义电子邮件消息，其中包括自定义徽标、描述和页脚 [品牌化](../using/brand-portal-branding.md) 功能。

## 从共享链接下载资源 {#download-assets-from-shared-links}

单击电子邮件中的链接可访问共享资产。 将打开AEM链接共享页面。

要下载共享资产，请执行以下操作：

1. 单击资源或文件夹，然后单击 **[!UICONTROL 下载]** 图标。

   ![](assets/download-share-link.png)

   >[!NOTE]
   >
   >目前，您只能为某些资源生成预览和缩略图，具体取决于文件格式。 有关支持的文件格式的详细信息，请参见 [对资源格式的预览和缩略图支持](#preview-thumbnail-support).

1. 此 **[!UICONTROL 下载]** 对话框。

   ![download-dialog](assets/download-dialog-box-new.png)

1. 默认情况下， **[!UICONTROL 快速下载]** 在中启用设置 **[!UICONTROL 下载设置]**. 因此，将显示一个确认框，确认继续使用IBM Aspera Connect下载。

   继续使用 **[!UICONTROL 快速下载]**，单击 **[!UICONTROL 允许]**.

   所有选定的演绎版都将下载到一个zip文件夹中，该文件夹中为每个资源包含一个单独的文件夹。

   >[!NOTE]
   >
   >从共享链接下载资源时，会为每个资源创建一个单独的文件夹。
   >
   >如果选择下载一个文件夹、收藏集或超过20个资产，则 **[!UICONTROL 下载]** 将跳过对话框，并且用户可访问的所有资源演绎版（不包括动态演绎版）都将下载到包含每个资源的单独文件夹的zip文件夹中。

   >[!NOTE]
   >
   >如果作为链接共享资产的用户未使用共享链接下载原始演绎版，则不会使用共享链接下载原始演绎版 [管理员授权有权访问原始演绎版](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges).


>[!NOTE]
>
>Brand Portal使用链接共享来限制下载大小大于5 GB的文件夹或资源。

<!--
1. The **[!UICONTROL Download]** dialog box appears.

   ![](assets/download-linkshare.png)

    * To speed up the download of asset files shared as the link, select **[!UICONTROL Enable download acceleration]** option and [follow the wizard](../using/accelerated-download.md#download-workflow-using-file-accelerator). To know more about the fast download of assets on Brand Portal refer [Guide to accelerate downloads from Brand Portal](../using/accelerated-download.md).
    
1. To download the renditions of assets in addition to the assets from the shared link, select **[!UICONTROL Rendition(s)]** option. When you do so, **[!UICONTROL Exclude System Renditions]** option appears that is selected by default. This prevents the download of out-of-the-box renditions along with approved assets or their custom renditions.

   However, to allow auto-generated renditions to download along with custom renditions, deselect the **[!UICONTROL Exclude System Renditions]** option.

   >[!NOTE]
   >
   >Original renditions are not downloaded using the shared link if the user who shared the assets as a link is not [authorized by the administrator to have access to the original renditions](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges).

   ![](assets/download-linkshare-autoren.png)

1. Click **[!UICONTROL Download]**. The assets (and renditions if selected) are downloaded as a ZIP file to your local folder. However, no zip file is created if a single asset is downloaded without any of the renditions, thereby ensuring speedy download.

-->

## 对资源格式的预览和缩略图支持 {#preview-thumbnail-support}

下表列出了Brand Portal支持缩略图和预览的资源格式：

| 资源格式 | 缩略图支持 | 预览支持 |
|--------------|-------------------|-----------------|
| PNG | ✓ | ✓ |
| GIF | ✓ | ✓ |
| TIFF | ✓ | ✕ “ ”标签 |
| JPEG | ✓ | ✓ |
| BMP | ✓ | ✕ |
| 凤凰新媒体* | NA | NA |
| PGM* | NA | NA |
| PBM* | NA | NA |
| PPM* | NA | NA |
| PSD | ✓ | ✕ |
| EPS | NA | ✕ |
| DNG | ✓ | ✕ |
| PICT | ✓ | ✕ |
| PSB* | ✓ | ✕ |
| JPG | ✓ | ✓ |
| 人工智能 | ✓ | ✕ |
| DOC | ✕ | ✕ |
| DOCX | ✕ | ✕ |
| ODT* | ✕ | ✕ |
| PDF | ✓ | ✕ |
| HTML | ✕ | ✕ |
| RTF | ✕ | ✕ |
| TXT | ✓ | ✕ |
| XLS | ✕ | ✕ |
| XLSX | ✕ | ✕ |
| ODS | ✕ | ✕ |
| PPT | ✓ | ✕ |
| PPTX | ✕ | ✕ |
| ODP | ✕ | ✕ |
| INDD | ✓ | ✕ |
| PS | ✕ | ✕ |
| QXP | ✕ | ✕ |
| ePub | ✓ | ✕ |
| AAC | ✕ | ✕ |
| MIDI | ✕ | ✕ |
| 3GP | ✕ | ✕ |
| MP3 | ✕ | ✕ |
| MP4 | ✕ | ✕ |
| OGA | ✕ | ✕ |
| OGG | ✕ | ✕ |
| RA | ✕ | ✕ |
| WAV | ✕ | ✕ |
| WMA | ✕ | ✕ |
| DVI | ✕ | ✕ |
| FLV | ✕ | ✕ |
| M4V | ✕ | ✕ |
| MPG | ✕ | ✕ |
| OGV | ✕ | ✕ |
| MOV | ✕ | ✕ |
| WMV | ✕ | ✕ |
| SWF | ✕ | ✕ |
| TGZ | NA | ✕ |
| JAR | ✓ | ✕ |
| RAR | NA | ✕ |
| TAR | NA | ✕ |
| ZIP | ✓ | ✕ |

下面的图例说明了矩阵中使用的符号：

| 符号 | 含义 |
|---|---|
| ✓ | 此文件格式支持此功能 |
| ✕ | 此文件格式不支持此功能 |
| NA | 此功能不适用于此文件格式 |
| &#42; | 此功能需要在AEM创作实例上对此文件格式提供加载项支持，但在将资产发布到Brand Portal后，不会在Brand Portal上提供此支持 |

## 取消共享作为链接共享的资产 {#unshare-assets-shared-as-a-link}

要将以前共享的资产取消作为链接共享，请执行以下操作：

1. 登录Brand Portal时， **[!UICONTROL 文件]** 默认情况下打开视图。 要查看您以链接形式共享的资源，请导航到 **[!UICONTROL 共享链接]** 视图。

1. 从显示的列表中查看您共享的链接。

   ![](assets/shared-links.png)

1. 要从列表中取消共享链接，请选择该链接并单击 **[!UICONTROL 取消共享]** 图标。

   ![](assets/unshare-asset.png)

   >[!NOTE]
   >
   >共享链接的显示因用户而异。 此功能不显示租户的所有用户共享的所有链接。

1. 在警告消息框中，单击 **[!UICONTROL 继续]** 以确认取消共享。 链接的条目将从共享链接列表中删除。
