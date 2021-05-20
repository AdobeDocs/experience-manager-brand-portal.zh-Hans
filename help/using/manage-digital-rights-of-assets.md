---
title: 管理资产的数字权限
seo-title: 管理资产的数字权限
description: 为资产授予许可并为资产和共享链接设置过期时间，可确保对这些资产进行受控的使用并保护它们。
seo-description: 为资产授予许可并为资产和共享链接设置过期时间，可确保对这些资产进行受控的使用并保护它们。
uuid: ce30e398-0109-41bf-a4d2-2fcca476f499
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: f77003ba-31fe-4a9e-96c8-dbc4c2eba79e
role: Administrator
exl-id: 86c31891-0627-41ca-b571-8dac3a074d55
source-git-commit: d2bfd06f8cd8a9e78efbc8dd92880e0faae39176
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 2%

---

# 管理资产的数字权限 {#manage-digital-rights-of-assets}

确保创意资产和品牌材料的安全分发和使用对保护您的品牌至关重要。 通过将过期日期（和时间）与从AEM发布到Brand Portal的已批准资产关联，或通过授权这些资产以条件使用，可以在组织内外强制执行此操作。 此外，Brand Portal还允许您为从Brand Portal共享的资产链接指定到期日期。

阅读并了解资产如何在Brand Portal上受到保护，并了解相关的使用权限。

## 资产过期 {#asset-expiration}

资产到期是控制组织内批准资产在Brand Portal上的使用的有效方式。 从AEM Assets发布到Brand Portal的所有资产都可以具有过期日期，这会限制不同用户角色对这些资产的使用。

### 与过期资产相关的使用权限{#usage-permissions-expired-assets}

在Brand Portal中，管理员可以查看、下载过期的资产并将其添加到收藏集。 然而，编辑器和查看器只能查看过期的资产并将其添加到收藏集。

管理员可以将过期的资产从AEM Assets发布到Brand Portal。 但是，无法通过Brand Portal中的链接共享已过期的资产。 如果您从包含已过期和未过期资产的文件夹中选择任何已过期的资产，则&#x200B;**[!UICONTROL 共享链接]**&#x200B;操作将不可用。 但是，如果您选择包含已过期和未过期资产的文件夹，则可以使用[!UICONTROL 共享]和&#x200B;**[!UICONTROL 共享链接]**&#x200B;操作。

>[!NOTE]
>
>即使文件夹包含已过期的资产，仍可以将其作为链接共享。 在这种情况下，链接不会列出已过期的资产，并且只会共享未过期的资产。

下表显示了已过期资产的使用权限：

|  | **[!UICONTROL 链接共享]** | **[!UICONTROL 下载]** | **[!UICONTROL 属性]** | **[!UICONTROL 添加到收藏集]** | **[!UICONTROL 删除]** |
|---|---|---|---|---|---|
| **[!UICONTROL 管理员]** | 不可用 | 可用 | 可用 | 可用 | 可用 |
| **[!UICONTROL 编辑者]** | 不可用 | 不可用 | 可用 | 可用 | 不可用 |
| **[!UICONTROL 查看者]** | 不可用 | 不可用 | 可用 | 可用 | 不可用 |
| **[!UICONTROL 来宾用户]** | 不可用 | 不可用 | 可用 | 可用 | 不可用 |

>[!NOTE]
>
>如果查看器和编辑器下载包含已过期和未过期资产的文件夹，则只会下载未过期的资产。 如果文件夹仅包含已过期的资产，则会下载一个空文件夹。

### 资产的过期状态{#expiration-status-of-assets}

您可以在资产的&#x200B;**[!UICONTROL 卡片视图]**&#x200B;中查看资产的过期状态。 卡片上的红色标记表示资产已过期。

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>列表视图和列视图不显示资产的过期状态。

## 资产链接到期{#asset-link-expiration}

在通过链接共享资产时，管理员和编辑人员可以使用&#x200B;**[!UICONTROL 链接共享]**&#x200B;对话框中的&#x200B;**[!UICONTROL 过期]**&#x200B;字段设置过期日期和时间。 链接的默认过期时间为共享链接之日起七天。

![](assets/asset-link-sharing.png)

它可确保作为链接共享的资产在Brand Portal管理员和编辑者设置的日期和时间过期，并且在过期日期之后无法再查看和下载资产。 由于通过链接共享的资产也可以由不属于组织的外部用户查看，因此通过指定到期时间，您可以确保已批准的资产受到保护，并且不会在指定时间后向未知实体显示。

有关链接共享的更多信息，请参阅[将资产共享为链接](../using/brand-portal-link-share.md)。

## 授权资产{#licensed-assets}

授权资产在从Brand Portal下载之前必须接受许可协议。 当您直接从Brand Portal或通过共享链接下载资产时，即表示您同意使用此许可资产协议。 无论是否过期，受许可证保护的资产都可由所有用户查看。 但是，过期的授权资产的下载和使用受到限制。 要了解过期的授权资产的行为以及基于用户角色允许的活动，请参阅已过期资产的[使用权限](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets)。

受许可证保护的资产具有附加的[许可协议](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets)，这可通过在AEM Assets中设置资产的[元数据属性](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets)来完成。

如果您选择下载受许可证保护的资产，则会将您重定向到&#x200B;**[!UICONTROL 版权管理]**&#x200B;页面。

![](assets/asset-copyright-mgmt.png)

在此，您需要选择要下载的资产并接受关联的许可协议。 如果您不接受许可协议，则&#x200B;**[!UICONTROL Download]**&#x200B;按钮将不启用。

![](assets/licensed-asset-download-2.png)

如果选择的资产包含多个受保护的资产，请一次选择一个资产，接受许可协议，然后继续下载资产。

## 生成有关已过期资产的报告{#generate-report-about-expired-assets}

管理员可以生成并下载一个报表，其中列出了在特定时间范围内过期的所有资产。 此报表包含有关已过期资产的详细信息，例如大小、类型、在资产层次结构中指定资产位置的路径、资产何时过期以及资产何时发布。 可根据用户要求自定义此报表的列以显示更多数据。

![](assets/assets-expired.png)

有关报告功能的更多信息，请参阅[使用报告](../using/brand-portal-reports.md#work-with-reports)。
