---
title: 以链接形式共享资产
description: 了解Adobe Experience Manager Assets Brand Portal管理员如何与授权内部用户和外部实体（包括合作伙伴和供应商）共享多个资源的链接。 编辑者只能查看和共享与其共享的资产。
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f3573219-3c58-47ba-90db-62b003d8b9aa
exl-id: 9d254e95-a4fc-468d-ae1f-9690ddd3b4a1
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 6%

---

# 以链接形式共享资产 {#share-assets-as-a-link}

Adobe Experience Manager Assets Brand Portal管理员可以与授权内部用户和外部实体（包括合作伙伴和供应商）共享多个资源的链接。 编辑者只能查看和共享与其共享的资产。

通过链接共享资源是一种向外部各方提供资源的便捷方法，因为接收者无需登录Brand Portal即可访问资源。

<!-- Link sharing access is restricted to editors and administrators. 
-->

有关详细信息，请参阅[管理用户、组和用户角色](../using/brand-portal-adding-users.md#manage-user-roles)。


以下是作为链接共享资产的步骤：

1. 登录到您的Brand Portal租户。 默认情况下，**[!UICONTROL 文件]**&#x200B;视图打开，其中包含所有已发布的资源和文件夹。

1. 选择要共享的资源或文件夹，或导航到&#x200B;**[!UICONTROL 收藏集]**&#x200B;视图以共享您创建的收藏集。

   ![选择多个资源](assets/select-assets-new.png)

1. 从顶部的工具栏中，单击&#x200B;**[!UICONTROL 共享链接]**&#x200B;图标。

   出现&#x200B;**[!UICONTROL 链接共享]**&#x200B;对话框。

   ![](assets/link-sharing.png)

   * 在电子邮件地址框中，键入要与其共享链接的用户的电子邮件ID。 您可以与多个用户共享该链接。 如果用户是您组织的成员，请从下拉列表中显示的建议中选择其电子邮件ID。 如果用户是外部用户，请键入完整的电子邮件ID并按&#x200B;**[!UICONTROL Enter]**；电子邮件ID将添加到用户列表中。

     ![](assets/link-sharing-text.png)

   * 在&#x200B;**[!UICONTROL 主题]**&#x200B;框中，为要共享的资源键入主题。
   * 在&#x200B;**[!UICONTROL 消息]**&#x200B;框中，根据需要键入消息。
   * 在&#x200B;**[!UICONTROL 过期]**&#x200B;字段中，使用日期选取器指定链接的过期日期和时间。 默认情况下，到期日期设置为自您共享链接之日起的7天。
   * 启用&#x200B;**[!UICONTROL 允许下载原始文件]**&#x200B;复选框，以允许收件人下载原始演绎版。

   通过链接共享的资源在超过&#x200B;**[!UICONTROL 过期]**&#x200B;字段中指定的日期和时间后过期。 有关Brand Portal中过期的资源行为和基于角色的活动更改的详细信息，请参阅[管理资源的数字权限](../using/manage-digital-rights-of-assets.md#asset-expiration)。

   >[!NOTE]
   >
   >链接的缺省过期时间为7天。 链接必须通过电子邮件发送给使用&#x200B;**[!UICONTROL 链接共享]**&#x200B;对话框的用户，请勿单独复制和共享该链接。

1. 单击&#x200B;**[!UICONTROL 共享]**。 将显示一条消息，确认该链接已与用户共享。 用户将收到包含共享链接的电子邮件。

   ![](assets/link-share-email.png)

   >[!NOTE]
   >
   >管理员可以自定义电子邮件消息，包括使用[品牌](../using/brand-portal-branding.md)功能自定义徽标、描述和页脚。

## 从共享链接下载资源 {#download-assets-from-shared-links}

单击电子邮件中的链接可访问共享资产。 将打开AEM链接共享页面。

要下载共享资源，请执行以下操作：

1. 单击资源或文件夹，然后单击工具栏中的&#x200B;**[!UICONTROL 下载]**&#x200B;图标。

   ![](assets/download-share-link.png)

   >[!NOTE]
   >
   >目前，您只能为某些资源生成预览和缩略图，具体取决于文件格式。 有关支持的文件格式的详细信息，请参阅[预览和缩略图对资源格式的支持](#preview-thumbnail-support)。

1. 出现&#x200B;**[!UICONTROL 下载]**&#x200B;对话框。

   ![下载对话框](assets/download-dialog-box-new.png)

1. 默认情况下，**[!UICONTROL 下载设置]**&#x200B;中启用了&#x200B;**[!UICONTROL 快速下载]**&#x200B;设置。 因此，会显示一个确认框，用于继续使用IBM® Aspera Connect下载。

   若要继续使用&#x200B;**[!UICONTROL 快速下载]**，请单击&#x200B;**[!UICONTROL 允许]**。

   所有选定的演绎版都将下载到一个zip文件夹中，并为每个资源包含一个单独的文件夹。

   >[!NOTE]
   >
   >从共享链接下载资产时，将为每个资产创建单独的文件夹。
   >
   >如果选择了文件夹、收藏集或超过20个资源，则会跳过&#x200B;**[!UICONTROL 下载]**&#x200B;对话框。 此外，所有可访问的资源演绎版（不包括动态资源演绎版）都将下载到一个zip文件夹中，并为每个资源单独设置文件夹。

   >[!NOTE]
   >
   >如果管理员未授权共享资产的用户，则共享链接不会下载原始演绎版。 另请参阅管理员授权的[访问原始演绎版](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges)。


>[!NOTE]
>
>Brand Portal使用链接共享来限制下载大于5 GB的文件夹或资源。

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
| TIFF | ✓ | ✕ {\f13 } |
| JPEG | ✓ | ✓ |
| BMP | ✓ | ✕ {\f13 } |
| 纳米晶* | NA | NA |
| PGM* | NA | NA |
| PBM* | NA | NA |
| PPM* | NA | NA |
| PSD | ✓ | ✕ {\f13 } |
| EPS | NA | ✕ {\f13 } |
| DNG | ✓ | ✕ {\f13 } |
| PICT | ✓ | ✕ {\f13 } |
| PSB* | ✓ | ✕ {\f13 } |
| JPG | ✓ | ✓ |
| 人工智能 | ✓ | ✕ {\f13 } |
| DOC | ✕ {\f13 } | ✕ {\f13 } |
| DOCX | ✕ {\f13 } | ✕ {\f13 } |
| ODT* | ✕ {\f13 } | ✕ {\f13 } |
| PDF | ✓ | ✕ {\f13 } |
| HTML | ✕ {\f13 } | ✕ {\f13 } |
| RTF | ✕ {\f13 } | ✕ {\f13 } |
| TXT | ✓ | ✕ {\f13 } |
| XLS | ✕ {\f13 } | ✕ {\f13 } |
| XLSX | ✕ {\f13 } | ✕ {\f13 } |
| ODS | ✕ {\f13 } | ✕ {\f13 } |
| PPT | ✓ | ✕ {\f13 } |
| PPTX | ✕ {\f13 } | ✕ {\f13 } |
| ODP | ✕ {\f13 } | ✕ {\f13 } |
| INDD | ✓ | ✕ {\f13 } |
| PS | ✕ {\f13 } | ✕ {\f13 } |
| QXP | ✕ {\f13 } | ✕ {\f13 } |
| ePub | ✓ | ✕ {\f13 } |
| AAC | ✕ {\f13 } | ✕ {\f13 } |
| MIDI | ✕ {\f13 } | ✕ {\f13 } |
| 3GP | ✕ {\f13 } | ✕ {\f13 } |
| MP3 | ✕ {\f13 } | ✕ {\f13 } |
| MP4 | ✕ {\f13 } | ✕ {\f13 } |
| OGA | ✕ {\f13 } | ✕ {\f13 } |
| OGG | ✕ {\f13 } | ✕ {\f13 } |
| RA | ✕ {\f13 } | ✕ {\f13 } |
| WAV | ✕ {\f13 } | ✕ {\f13 } |
| WMA | ✕ {\f13 } | ✕ {\f13 } |
| DVI | ✕ {\f13 } | ✕ {\f13 } |
| FLV | ✕ {\f13 } | ✕ {\f13 } |
| M4V | ✕ {\f13 } | ✕ {\f13 } |
| MPG | ✕ {\f13 } | ✕ {\f13 } |
| OGV | ✕ {\f13 } | ✕ {\f13 } |
| MOV | ✕ {\f13 } | ✕ {\f13 } |
| WMV | ✕ {\f13 } | ✕ {\f13 } |
| SWF | ✕ {\f13 } | ✕ {\f13 } |
| TGZ | NA | ✕ {\f13 } |
| JAR | ✓ | ✕ {\f13 } |
| RAR | NA | ✕ {\f13 } |
| TAR | NA | ✕ {\f13 } |
| ZIP | ✓ | ✕ {\f13 } |

下面的图例说明了矩阵中使用的符号：

| 符号 | 含义 |
|---|---|
| ✓ | 此文件格式支持此功能 |
| ✕ {\f13 } | 此文件格式不支持此功能 |
| NA | 此功能不适用于此文件格式 |
| &#42; | 此功能需要在AEM创作实例上附加支持此文件格式，但在将资产发布到Brand Portal后，需要在Brand Portal上附加支持 |

## 取消共享作为链接共享的资源 {#unshare-assets-shared-as-a-link}

要将以前共享的资产取消作为链接共享，请执行以下操作：

1. 登录到Brand Portal时，**[!UICONTROL 文件]**&#x200B;视图默认打开。 要查看您共享为链接的资源，请导航到&#x200B;**[!UICONTROL 共享链接]**&#x200B;视图。

1. 从显示的列表中查看您共享的链接。

   ![](assets/shared-links.png)

1. 要从列表中取消共享链接，请选择该链接并单击顶部工具栏中的&#x200B;**[!UICONTROL 取消共享]**&#x200B;图标。

   ![](assets/unshare-asset.png)

   >[!NOTE]
   >
   >共享链接的显示因用户而异。 此功能不显示租户的所有用户共享的所有链接。

1. 在警告消息框中，单击&#x200B;**[!UICONTROL 继续]**&#x200B;以确认取消共享。 链接的条目将从共享链接列表中删除。
