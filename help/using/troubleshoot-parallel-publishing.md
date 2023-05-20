---
title: 对并行发布到 Brand Portal 时出现的问题进行故障诊断
seo-title: Troubleshoot issues in parallel publishing to Brand Portal
description: 疑難排解平行發佈。
seo-description: Troubleshoot parallel publishing.
uuid: 51e45cca-8c96-4c69-84ef-2ef34f3bcde2
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: brand-portal
discoiquuid: a4801024-b509-4c51-afd8-e337417e658b
role: Admin
exl-id: 631beabc-b145-49ba-a8e4-f301497be6da
source-git-commit: 72cd0ebbf05067287d94e1dc4e1b68f5fb6c2888
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 1%

---

# 对并行发布到 Brand Portal 时出现的问题进行故障诊断 {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Brand Portal已透過Experience Manager Assets設定，以核准從Experience Manager Assets製作執行個體無縫擷取（或發佈）品牌資產。 一次 [已設定](../using/configure-aem-assets-with-brand-portal.md)，Experience Manager作者會使用復寫代理將選取的資產復寫至Brand Portal雲端服務，以供Brand Portal使用者核准使用。 Experience Manager6.2 SP1-CFP5、Experience ManagerCFP 6.3.0.2及更高版本使用多個復寫代理程式，以便允許高速平行發佈。

>[!NOTE]
>
>Adobe建議升級至Experience Manager6.4.1.0，以確保Experience Manager Assets Brand Portal成功設定為Experience Manager Assets。 Experience Manager6.4的限制會在使用Brand Portal設定Experience Manager Assets時發生錯誤，且復寫失敗。

在「 」下為Brand Portal設定雲端服務 **[!UICONTROL /etc/cloudservice]**，系統會自動產生所有必要的使用者和Token並儲存在存放庫中。 已建立雲端服務設定，也會建立復寫和復寫代理程式復寫內容所需的服務使用者。 它會建立四個復寫代理。 因此，當您從Experience Manager發佈許多資產到Brand Portal時，資產會排入佇列，並透過Round Robin在復寫代理程式之間分配。

然而，由於大量的Sling工作、增加的網路和網路等原因，發佈可能會斷斷續續失敗。 **[!UICONTROL 磁碟I/O]** 「Experience Manager作者」例項上，或「Experience Manager作者」例項效能降低。 因此，建議您在開始發佈之前，先測試與復寫代理程式的連線。

![](assets/test-connection.png)

## 疑難排解首次發佈時的失敗：驗證您的發佈設定 {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

若要驗證您的發佈設定：

1. 檢查錯誤記錄
1. 檢查是否已建立復寫代理
1. 測試連線

**建立Cloud Service時的尾端記錄**

檢查尾部記錄。 檢查是否已建立復寫代理。 如果復寫代理程式建立失敗，請在Cloud Service中進行微幅變更，以編輯雲端服務。 驗證並再次檢查復寫代理程式是否已建立。 如果沒有，請重新編輯服務。

如果重複編輯雲端服務時未正確設定，請回報Daycare票證。

**測試與復寫代理的連線**

檢視記錄（如果在復寫記錄中找到錯誤）：

1. 請聯絡客戶支援。

1. 重試 [cleanup](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) 並再次建立發佈設定。

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

## 清除現有的Brand Portal發佈設定 {#clean-up-existing-config}

大多數情況下，發佈無法正常運作，可能是因為使用者正在發佈(例如： `mac-<tenantid>-replication` 沒有最新的私密金鑰，因此發佈會失敗，並出現「401未獲授權」錯誤，復寫代理程式記錄檔中未報告任何其他錯誤。 您可能想要避免疑難排解，改為建立設定。 為了讓新設定正確運作，請從Experience Manager作者設定中清理下列專案：

1. 前往 `localhost:4502/crx/de/` (假設您正在localhost上執行作者例項:4502:\
   i.刪除 `/etc/replication/agents.author/mp_replication`
二、 删除 
`/etc/cloudservices/mediaportal/<config_name>`

1. 前往localhost：4502/useradmin：\
   i.搜尋使用者 `mac-<tenantid>replication`
二、 刪除此使用者

現在系統已全部清除。 現在您可以嘗試建立雲端服務設定，並且仍使用現有的JWT應用程式。 不需要建立應用程式，只需從新建立的雲端設定更新公開金鑰即可。

>[!NOTE]
>
>請勿修改任何自動產生的設定。


## 開發人員連線JWT應用程式租使用者可見性問題 {#developer-connection-jwt-application-tenant-visibility-issue}

若開啟 `https://legacy-oauth.cloud.adobe.io/`，則會列出目前使用者擁有系統管理員的所有組織（租使用者）。 如果您在這裡找不到組織名稱，或無法在這裡為需要的租使用者建立應用程式，請檢查您是否有足夠的（系統管理員）許可權。

此使用者介面有一個已知問題，即對於任何租使用者而言，只會看到前十個應用程式。 建立應用程式時，請停留在頁面上並將URL加入書籤。 您不需要前往應用程式的清單頁面來尋找您建立的應用程式。 您可以直接點選此建立書籤的URL，並視需要更新/刪除應用程式。

JWT應用程式可能未正確列出。 因此，建議您在建立JWT應用程式時記下/將URL加入書籤。

## 執行組態停止運作 {#running-configuration-stops-working}

<!--
Comment Type: draft

<p>If the running configuration stops working, either of the following two possibilities
<g class="gr_ gr_15 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar multiReplace" data-gr-id="15" id="15" style="font-size: 12px;">
are
</g> there:</p>
<p>1.
<g class="gr_ gr_14 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="14" id="14">
Connection
</g> has failed, or</p>
<p>2. Publish has failed with permission to dam-replication-service denied, while connection has passed </p>
<p>If the connection has failed [1], the
<g class="gr_ gr_10 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling ins-del multiReplace" data-gr-id="10" id="10">
fail safe
</g> way to fix it is to <a href="../using/troubleshoot-parallel-publishing.md#main-pars-header-1664955658">clean up</a> the existing Brand Portal publish configuration and recreate a publish configuration. </p>
<p>However, if the
<g class="gr_ gr_18 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling" data-gr-id="18" id="18">
publish
</g> has failed with
<g class="gr_ gr_16 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="16" id="16">
permission
</g> denied to dam-replication-service, raise a support ticket.</p>
-->

如果復寫代理程式(原本可順利發佈至Brand Portal)停止處理發佈工作，請檢查復寫記錄。 Experience Manager內建自動重試，因此如果特定資產發佈失敗，則會自動重試。 如果發生網路錯誤等間歇性問題，重試期間可能會成功。

如果連續發佈失敗且佇列遭到封鎖，則應檢查 **[!UICONTROL 測試連線]** 並嘗試解決回報的錯誤。

根據錯誤，建議您記錄支援票證，以便Brand Portal工程團隊可以幫助您解決問題。

## Brand Portal IMS設定權杖已過期 {#token-expired}

如果您的Brand Portal環境突然停止，IMS設定可能會無法正常運作。 系統會顯示不正常的IMS設定，並反映您的存取權杖已到期的錯誤訊息（類似於以下內容）。

`com.adobe.granite.auth.oauth.AccessTokenProvider failed to get access token from authorization server status: 400 response: Unknown macro: {"error"}`

若要解決此問題，建議手動儲存並關閉IMS設定，然後再次檢查健全狀態。 如果組態無法運作，請刪除現有組態並建立新組態。


## 設定復寫代理以避免連線逾時錯誤 {#connection-timeout}

如果復寫佇列中有多個擱置中的請求，發佈作業通常會失敗並出現逾時錯誤。 若要解決此問題，請確保復寫代理已設定為避免逾時。

設定復寫代理程式：

1. 登入您的AEM Assets作者執行個體。
1. 從 **工具** 面板，導覽至 **[!UICONTROL 部署]** > **[!UICONTROL 復寫]**.
1. 在「復寫」頁面中，按一下 **[!UICONTROL 作者上的代理]**. 您可以看到Brand Portal租使用者的四個復寫代理。
1. 按一下復寫代理程式URL，然後按一下 **[!UICONTROL 編輯]**.
1. 在「代理程式設定」中，按一下 **[!UICONTROL 延伸]** 標籤。
1. 選取 **[!UICONTROL 關閉連線]** 核取方塊。
1. 重複步驟4到7，設定所有四個復寫代理。
1. 重新啟動伺服器。
