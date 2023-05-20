---
title: 常见问题解答
seo-title: null
description: 深入瞭解Adobe Experience Manager Assets Brand Portal的常見問題。
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 0%

---

# 常见问题解答 {#frequently-asked-questions}

Brand Portal常見問題集專注於使用者在使用最新Experience Manager Assets Brand Portal 6.4.6版本或更早版本時可能會遇到的查詢和問題。


## Brand Portal 6.4.6常見問題集  {#faqs-bp646}

**計數。 現有的舊版OAuth端點(`https://legacy-oauth.cloud.adobe.io/login`)無法運作。 可能的原因是什麼？**

**ans.** 已棄用舊版OAuth設定。 您必須將Experience Manager Assets作者執行個體升級至最新的Service Pack，並透過Adobe Developer主控台進行設定。 另請參閱 [使用Brand Portal設定Experience Manager Assets](configure-aem-assets-with-brand-portal.md) 以取得詳細資訊。 不過，若要讓舊版OAuth設定在升級前繼續運作，請將舊版OAuth端點更新為 `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**計數。 升級至Adobe Developer主控台後，無法將貢獻資料夾的資產從Brand Portal發佈至Experience Manager Assets。 我的編寫執行個體位於Experience Manager Assets 6.5.4。可能的原因是什麼？**

**ans.** 是，透過Adobe Developer Console將貢獻資料夾的資產發佈至Experience Manager Assets 6.5.4時出現已知問題。

Experience Manager Assets 6.5.5已修正此問題。您可以將Experience Manager Assets執行個體升級至最新的Service Pack，並且 [升級您的設定](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) 在Adobe Developer Console上。

<!--
Broken link of download hotfix, comment out this section until we have the latest URL.

For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your AEM author instance.
-->

**計數。 我沒有看到從Experience Manager Assets中的Brand Portal發佈的貢獻資料夾內容。 可能的原因是什麼？**

**ans.** 請聯絡您的Experience Manager Assets管理員以驗證設定，並確保您的Brand Portal租使用者僅設定了一個Experience Manager Assets作者執行個體。

當您在多個Brand Portal作者執行個體上設定Experience Manager Assets租使用者時，可能會發生此問題。 例如，管理員會在中繼和生產環境的Experience Manager Assets製作例項上設定相同的Brand Portal租使用者。 在此情況下，資產發佈會在Brand Portal中觸發，但Experience Manager Assets作者執行個體無法匯入資產，因為復寫代理程式不會收到請求權杖。


**計數。 我無法從Experience Manager Assets發佈資產到Brand Portal。 復寫記錄檔指出連線逾時。 有快速修正方法嗎？**

**ans.** 如果復寫佇列中有多個擱置中的請求，通常發佈會失敗並出現逾時錯誤。 若要解決此問題，請確保復寫代理已設定為避免逾時。

執行以下步驟來設定復寫代理程式：

1. 登入您的Experience Manager Assets作者執行個體。
1. 從 **工具** 面板，導覽至 **[!UICONTROL 部署]** > **[!UICONTROL 復寫]**.
1. 在「復寫」頁面中，按一下 **[!UICONTROL 作者上的代理]**. 您可以看到您Brand Portal租使用者的四個復寫代理。
1. 按一下復寫代理程式URL以開啟代理程式詳細資訊。
1. 按一下 **[!UICONTROL 編輯]** 修改復寫代理程式設定。
1. 在「代理程式設定」中，按一下 **[!UICONTROL 延伸]** 標籤。
1. 選取 **[!UICONTROL 關閉連線]** 核取方塊。
1. 重複步驟4到7，設定所有四個復寫代理。
1. 重新啟動伺服器並驗證連線。


## Brand Portal 6.4.5常見問題集  {#faqs-bp645}

**計數。 Brand Portal 6.4.5版有哪些主要變更？**

**ans.** Experience Manager Assets Brand Portal 6.4.5是功能發行版本，可讓Brand Portal使用者從Brand Portal執行個體上傳內容，並將「貢獻」資料夾發佈回Experience Manager Assets，而不需要管理員許可權。
如需詳細資訊，請參閱 [Brand Portal中的Asset Sourcing](brand-portal-asset-sourcing.md).



**計數。 我是否會失去我已建立的任何現有資產、功能或設定的存取權？**

**ans.** 所有現有功能和設定均維持不變。 您的使用者不會受到影響，而您的內容會維持不變。



**計數。 何時可以改用新版Brand Portal？**

**ans.** Brand Portal 6.4.5於2019年10月發佈至生產環境。 下一版Brand Portal預計於2020年第三季度發行。
如需更新和版本變更，建議追蹤 [發行說明](brand-portal-release-notes.md) 和 [Brand Portal的新功能](whats-new.md).



**計數。 我的使用者是否會受到影響？**

**ans.** Brand Portal 6.4.5版獨佔Brand Portal，因此對一般使用者沒有影響。



**計數。 身為Brand Portal使用者，我是否需要執行任何動作？**

**ans.** Brand Portal 6.4.5版隨附名為Asset Sourcing的新功能。 管理員必須在Experience Manager Assets中設定Asset Sourcing功能，才能為Brand Portal使用者啟用該功能。 如需詳細資訊，請參閱 [啟用資產來源](brand-portal-asset-sourcing.md).



**計數。 誰可以建立「貢獻」資料夾？**

**ans.** 任何有權在Experience Manager Assets中建立新資料夾的Experience Manager Assets使用者都可以建立 **貢獻** 資料夾。 若要建立 **貢獻** 資料夾，建立型別為的新資料夾 **資產貢獻**.
此資料夾會與作用中的Brand Portal使用者共用，以取得貢獻。



**計數。 「貢獻」資料夾包含哪些內容？**

**ans.** **貢獻** 資料夾包含兩個子資料夾 **新增** 和 **已共用**. 最初，NEW資料夾是空白的，而SHARED資料夾包含Brand Portal使用者的參考內容（可重複使用的資產）。
Brand Portal使用者存取 **貢獻** 資料夾和上傳內容於 **新增** 資料夾。



**計數。  我可以修改現有「貢獻」資料夾的名稱嗎？**

**ans.** **否**，您無法修改現有名稱 **貢獻** 資料夾。



**計數。 資產需求與r.t.貢獻是什麼？**

**ans.** 此 **簡報** 附加至以下專案的檔案： **貢獻** 資料夾和參考內容（可重複使用的資產）上傳到 **已共用** 資料夾可協助Brand Portal使用者瞭解身為貢獻者的貢獻需求和期望，並統稱為資產需求。



**計數。 我可以將資產上傳到任何允許的資料夾嗎？**

**ans.** 並非所有允許的資料夾。 Brand Portal使用者只能將內容上傳至 **貢獻** Experience Manager Assets或Brand Portal管理員共用的資料夾。



**計數。 如何取得「貢獻」資料夾的存取權？**

**ans.** 您可以存取 **貢獻** 資料夾（如果已與您共用）。 每當您共用「貢獻」資料夾時，都會收到電子郵件/脈衝通知。 您可以透過電子郵件中共用的連結存取「貢獻」資料夾，或登入您的Brand Portal執行個體並導覽至鈴鐺圖示以取得通知以存取「貢獻」資料夾。

>[!NOTE]
>
>如果您不是現有的Brand Portal使用者，請要求Experience Manager Assets管理員在Admin Console中建立您的使用者，並將您的設定檔新增至Brand Portal使用者清單中的使用者設定檔。

**計數。 使用者匯入的CSV檔案格式為何？**

**ans.** 格式與Admin Console支援的大量使用者匯入格式相同。 電子郵件、名字和姓氏為必填欄位。



**計數。 什麼會填入「資產貢獻」使用者下拉式清單中的使用者(Brand Portal貢獻者)？**

**ans.** 下拉式清單中的使用者會從Experience Manager Assets中上傳的Brand Portal使用者設定(.csv)檔案填入。



**計數。 我可以在哪裡檢視匯入和發佈工作的狀態？**

**ans.** 在Experience Manager Assets中，您可以在中檢視匯入的狀態 **非同步** 工作頁面。 在Brand Portal中，您可以透過以下位置檢視發佈工作的狀態： **[!UICONTROL 工具>資產貢獻狀態]**.



**計數。 以Experience Manager定期執行的匯入作業的頻率為何？**

**ans.** 在Experience Manager Assets中，每5分鐘會執行輪詢。



**計數。 資料夾可以從Brand Portal發佈到Experience Manager Assets的次數是否有任何限制？**

**ans.** 否，此專案中的所有資產 **新增** 資料夾會發佈至Experience Manager Assets，無論這些資料夾先前是否發佈。 每次a **貢獻** 資料夾從Brand Portal發佈至Experience Manager Assets，會覆寫 **新增** 資料夾。



**計數。 如何在「貢獻」資料夾中上傳新資產？**

**ans.** 請參閱詳細檔案，瞭解 [將資產上傳至「貢獻」資料夾](brand-portal-publish-contribution-folder-to-brand-portal.md).



**計數。 我是否看不到Brand Portal使用者上傳至NEW資料夾的資產的縮圖/預覽？**

**ans.** 根據設計，Brand Portal端不會執行任何工作流程。



**計數。 如果將資料夾從Experience Manager Assets發佈至變動中的Brand Portal，會發生什麼情況？**

**ans.** 在Experience Manager Assets中，會維護每次將資料夾發佈到Brand Portal時的記錄。 發佈時，所有未發佈至Brand Portal的資產都會置於復寫佇列中。 觸發發佈工作後新增至資料夾的任何資產都不會發佈至Brand Portal。 當Experience Manager Assets使用者再次發佈資料夾時，只有先前未發佈的資產（存在於復寫佇列中）會發佈至Brand Portal。
從Experience Manager Assets發佈至Brand Portal的任何資料夾，以及「貢獻」資料夾內的「共用」資料夾，都是如此。

**計數。 如有疑問，請聯絡誰？**

**ans.** 請聯絡您的Adobe客戶經理或客戶支援。

>[!NOTE]
>
>發行排程為暫定，可能會有變動。 請聯絡您的Adobe客戶經理或客戶支援，以取得更新的發行排程。


## 產品存取與支援（受限制的網站） {#product-access-and-support-restricted-sites}

這些網站僅供客戶使用。 如果您是客戶並需要存取權，請聯絡您的Adobe客戶經理。

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Support]()
-->
