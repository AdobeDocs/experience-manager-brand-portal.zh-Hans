---
title: 管理资产的数字权限
seo-title: Manage digital rights of assets
description: 授權資產和設定資產和共用連結的到期日，可確保控制這些資產的使用並保護它們。
seo-description: Licensing assets and setting expiration for assets and shared links ensure controlled usage of these assets and safeguard them.
uuid: ce30e398-0109-41bf-a4d2-2fcca476f499
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: f77003ba-31fe-4a9e-96c8-dbc4c2eba79e
role: Admin
exl-id: 86c31891-0627-41ca-b571-8dac3a074d55
source-git-commit: d1487434b10b01eaf55f34672267490fd8fd907e
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 2%

---

# 管理资产的数字权限 {#manage-digital-rights-of-assets}

確保創意資產和品牌資料的安全發佈和使用對於保護您的品牌至關重要。 您可以將到期日（和時間）與從AEM發佈至Brand Portal的已核准資產建立關聯，或授權這些資產供條件式使用，藉此在整個組織內外強制執行此作業。 此外，Brand Portal可讓您指定從Brand Portal共用之資產的連結到期日。

請閱讀下文，瞭解如何在Brand Portal上保護資產，並瞭解相關的使用許可權。

## 資產有效期 {#asset-expiration}

資產到期是控制組織內對Brand Portal上已核准資產之使用方式的有效方式。 從AEM Assets發佈至Brand Portal的所有資產都可以有到期日，這會限制不同使用者角色對這些資產的使用。

### 與過期資產相關的使用許可權 {#usage-permissions-expired-assets}

在Brand Portal中，管理員可以檢視、下載過期的資產，並將其新增至收藏集。 而編輯者和檢視者只能檢視過期的資產，並將其新增至收藏集。

管理員可以將過期的資產從AEM Assets發佈到Brand Portal。 不過，過期資產無法透過Brand Portal的連結共用。 如果您從包含過期和未過期資產的檔案夾中選取任何過期資產，則 **[!UICONTROL 共用連結]** 動作無法使用。 但是，如果您選取的資料夾中包含已過期和未過期的資產，則 [!UICONTROL 共用] 和 **[!UICONTROL 共用連結]** 動作可供使用。

>[!NOTE]
>
>即使資料夾包含過期的資產，資料夾仍可以連結形式共用。 在此情況下，連結不會列出過期的資產，只會共用未過期的資產。

下表顯示過期資產的使用許可權：

|  | **[!UICONTROL 連結共用]** | **[!UICONTROL 下载]** | **[!UICONTROL 属性]** | **[!UICONTROL 新增至集合]** | **[!UICONTROL 删除]** |
|---|---|---|---|---|---|
| **[!UICONTROL 管理员]** | 無法使用 | 可用 | 可用 | 可用 | 可用 |
| **[!UICONTROL 编辑器]** | 無法使用 | 無法使用 | 可用 | 可用 | 無法使用 |
| **[!UICONTROL 查看者]** | 無法使用 | 無法使用 | 可用 | 可用 | 無法使用 |
| **[!UICONTROL 訪客使用者]** | 無法使用 | 無法使用 | 可用 | 可用 | 無法使用 |

>[!NOTE]
>
>如果「檢視者和編輯器」下載的資料夾中包含已過期和未過期的資產，則只會下載未過期的資產。 如果資料夾僅包含過期的資產，則會下載空白資料夾。

### 資產的到期狀態 {#expiration-status-of-assets}

您可以檢視中資產的到期狀態 **[!UICONTROL 卡片檢視]**. 卡片上的紅色旗標表示資產已過期。

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>清單和欄檢視不會顯示資產的到期狀態。

## 資產連結有效期 {#asset-link-expiration}

透過連結共用資產時，管理員和編輯人員可以使用 **[!UICONTROL 有效期]** 中的欄位 **[!UICONTROL 連結共用]** 對話方塊。 連結的預設到期日是從共用連結的日期起七天。

![](assets/asset-link-sharing.png)

它可確保共用為連結的資產會在Brand Portal管理員和編輯人員設定的日期和時間過期，並在過期日期後無法再檢視和下載。 由於透過連結共用的資產也可由不屬於組織的外部使用者檢視，透過指定有效期，您可以確保您的已核准資產受到保護，不會在指定時間後向未知實體公開。

如需連結共用的詳細資訊，請參閱 [以連結形式共用資產](../using/brand-portal-link-share.md).

## 授權資產 {#licensed-assets}

授權資產在從Brand Portal下載前，必須先接受授權合約。 授權資產的本合約於您直接從Brand Portal下載資產，或透過共用連結下載資產時提供。 無論是否已過期，所有使用者都可以檢視受授權保護的資產。 不過，已過期授權資產的下載和使用受到限制。 若要瞭解已過期授權資產的行為以及根據使用者角色而允許的活動，請參閱 [過期資產的使用許可權](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets).

受授權保護的資產具有 [已附加授權合約](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/drm.html) ，方法是設定資產的中繼資料屬性 [!DNL Experience Manager Assets].

如果資產包含下列（或兩者）中繼資料屬性，則視為受保護：

* `xmpRights:WebStatement`：此屬性是指包含資產授權合約的頁面路徑。 `xmpRights:WebStatement` 應為存放庫中的有效路徑。
* `adobe_dam:restrictions`：此屬性的值是指定授權合約的原始HTML。


如果您選擇下載受授權保護的資產，則會將您重新導向至 **[!UICONTROL 版權管理]** 頁面（視中繼資料屬性而定）。

| `adobe_dam:restrictions` | `xmpRights:WebStatement` | 版权管理 |
| --- | --- | --- |
| 是 | - | 介面會顯示在Assets和Brand Portal中 |
| - | 是（無效路徑） | 無介面 |
| 是 | 是（無效路徑） | 無介面 |
| 是 | 是（有效路徑） | 介面會顯示在「資產」或Brand Portal中 </br> 視路徑是否對Assets或Brand Portal （或兩者）有效而定。 |

![](assets/asset-copyright-mgmt.png)

您必須在此處選取要下載的資產，並接受相關的授權合約。 如果您不接受授權合約，則 **[!UICONTROL 下載]** 按鈕未啟用。

![](assets/licensed-asset-download-2.png)

如果選取範圍包含多個受保護的資產，請一次選取一個資產、接受授權合約，然後繼續下載資產。

## 產生過期資產的相關報告 {#generate-report-about-expired-assets}

管理員可以產生並下載報表，列出特定時間範圍內所有已到期的資產。 此報表包含有關過期資產的詳細資訊（例如大小、型別、在資產階層中指定資產位置的路徑、資產過期時間以及資產發佈時間）。 可自訂此報告的欄，以根據使用者需求顯示更多資料。

![](assets/assets-expired.png)

如需有關報表功能的詳細資訊，請參閱 [使用報告](../using/brand-portal-reports.md#work-with-reports).
