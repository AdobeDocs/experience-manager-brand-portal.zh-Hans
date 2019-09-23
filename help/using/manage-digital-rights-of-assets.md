---
title: 管理资产的数字权限
seo-title: 管理资产的数字权限
description: 为资产和共享链接授权和设置过期时间可确保对这些资产进行有控制的使用并予以保护。
seo-description: 为资产和共享链接授权和设置过期时间可确保对这些资产进行有控制的使用并予以保护。
uuid: ce30e398-0109-41bf-a4d2-2fcca476f499
contentOwner: bdhar
topic-tags: 下载安装
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: 引用
discoiquuid: f77003ba-31fe-4a9e-96c8-dbc4c2eba79e
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 管理资产的数字权限 {#manage-digital-rights-of-assets}

确保创意资产和品牌资料的安全分发和使用对于保护您的品牌至关重要。 通过将到期日（和时间）与从AEM发布到Brand Portal的已批准资产相关联，或通过授权许可这些资产以便有条件地使用，可以在组织内外强制实施此操作。 此外，Brand Portal还允许您为从Brand Portal共享的资产链接指定到期日。

阅读以了解资产如何在Brand Portal上得到保护，并了解相关的使用权限。

## 资产过期 {#asset-expiration}

资产到期是控制组织内品牌门户上已批准资产的使用的有效方式。 从AEM资产发布到Brand Portal的所有资产都可以具有到期日期，这将限制按不同用户角色使用这些资产。

### 与过期资产相关的使用权限 {#usage-permissions-expired-assets}

在Brand Portal中，管理员可以查看、下载过期的资产并将其添加到收藏集。 但是，编辑人员和查看器只能查看过期的资产并将其添加到收藏集。

管理员可以将过期的资产从AEM资产发布到Brand Portal。 但是，无法通过Brand Portal中的链接共享过期的资产。 如果您从同时包含已过期和未过期资产的文件夹中选择任何已过期的资产，则共享链 **[!UICONTROL 接操作将不可用]** 。 但是，如果您选择的文件夹包含已过期和未过期的资产，则可以执 [!UICONTROL 行“共享] ”和“ **[!UICONTROL 共享链接]** ”操作。

>[!NOTE]
>
>即使文件夹包含过期的资产，仍可以将其共享为链接。 在这种情况下，链接不会列出已过期的资产，并且只共享未过期的资产。

下表显示了过期资产的使用权限：

|  | **[!UICONTROL 链接共享]** | **[!UICONTROL 下载]** | **[!UICONTROL 属性]** | **[!UICONTROL 添加到集合]** | **[!UICONTROL 删除]** |
|---|---|---|---|---|---|
| **[!UICONTROL 管理员]** | 不可用 | 可用 | 可用 | 可用 | 可用 |
| **[!UICONTROL 编辑器]** | 不可用 | 不可用 | 可用 | 可用 | 不可用 |
| **[!UICONTROL 查看器]** | 不可用 | 不可用 | 可用 | 可用 | 不可用 |
| **[!UICONTROL 客人用户]** | 不可用 | 不可用 | 可用 | 可用 | 不可用 |

>[!NOTE]
>
>如果查看器和编辑人员下载了包含已过期和未过期资产的文件夹，则仅下载未过期的资产。 如果文件夹仅包含过期的资产，则会下载一个空文件夹。

### 资产的到期状态 {#expiration-status-of-assets}

您可以在资产的卡片视图中查看资产的 [!UICONTROL 到期状态]。 卡上的红色标记表示资产已过期。

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>列表视图和列视图不显示资产的到期状态。

## 资产链接到期 {#asset-link-expiration}

通过链接共享资产时，管理员和编辑人员可以使用“链接共享”对话框的“ **[!UICONTROL 到期]** ”字段设置 **[!UICONTROL 到期日期和时间]** 。 链接的默认过期时间为共享链接之日起七天。

![](assets/asset-link-sharing.png)

它可确保作为链接共享的资产在Brand Portal管理员和编辑人员设置的日期和时间过期，并且在过期日期后将无法再查看和下载。 由于通过链接共享的资产也可以由不属于组织的外部用户查看，通过指定过期时间，您可以确保已批准的资产受到保护，并且在指定时间后不会暴露给未知实体。

有关链接共享的详细信息，请参阅将 [资产共享为链接](../using/brand-portal-link-share.md)。

## 许可资产 {#licensed-assets}

从Brand Portal下载许可资产前，须接受许可协议。 当您直接从Brand Portal或通过共享链接下载资产时，即会签订此许可资产协议。 无论是否已过期，受许可证保护的资产都可供所有用户查看。 但是，过期的许可资产的下载和使用受到限制。 要了解过期的授权资产的行为以及基于用户角色的允许活动，请参阅过期资 [产的使用权限](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets)。

受许可证保护的资 [产附加了许可协议](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) ，可通过在AEM资产中设置资产的元数据属 [性](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) 来完成此操作。

如果您选择下载受许可证保护的资产，则会将您重定向到“版权 [!UICONTROL 管理] ”页面。

![](assets/asset-copyright-mgmt.png)

您需要在此选择要下载的资产并接受关联的许可协议。 如果您不接受许可协议，则“下 [!UICONTROL 载] ”按钮不启用。

![](assets/licensed-asset-download-2.png)

如果选择包含多个受保护的资产，则一次选择一个资产，接受许可协议，然后继续下载该资产。

## 生成有关过期资产的报告 {#generate-report-about-expired-assets}

管理员可以生成并下载一个报告，其中列出在特定时间范围内过期的所有资产。 此报告包括详细信息— 例如，大小、类型、在资产层次结构中指定资产位置的路径、资产的过期时间以及资产的发布时间— 关于过期的资产。 可以自定义此报告的列，以根据用户要求显示更多数据。

![](assets/assets-expired.png)

有关报告功能的详细信息，请参阅 [使用报告](../using/brand-portal-reports.md#work-with-reports)。
