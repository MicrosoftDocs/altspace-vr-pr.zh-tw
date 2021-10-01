---
title: AltspaceVR 應用程式的常見問題
description: AltspaceVR 應用程式的疑難排解和支援。
ms.date: 8/16/2021
author: qianw211
ms.author: v-qianwen
ms.topic: article
keywords: vr、AltspaceVR、疑難排解、支援
ms.openlocfilehash: a0df1e100ef8511fe3c9129548529577964c2336
ms.sourcegitcommit: 5c452a9092297c0bfbc8efabebf395e7ee31853f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/30/2021
ms.locfileid: "129311848"
---
# <a name="frequently-asked-questions-about-the-altspacevr-app"></a>AltspaceVR 應用程式的常見問題

## <a name="finding-the-altspacevr-app-version"></a>尋找 AltspaceVR 應用程式版本

在針對問題進行疑難排解的過程中，系統可能會詢問您目前正在執行的 AltspaceVR 應用程式版本。

### <a name="in-altspacevr"></a>在 AltspaceVR 中

若要在 AltspaceVR 中尋找應用程式版本，請流覽至 [ **設定] 功能表** ，並在左側導覽列中選取 [ **關於** ]。 這裡會報告 [應用程式版本]，如下列螢幕擷取畫面所示。

![開啟時開啟的 [關於] 面板開啟的設定功能表](images/app-version-img-01.png)

### <a name="in-windows-system-settings"></a>在 Windows 系統設定

如果您是透過 Microsoft Store 安裝 AltspaceVR，您可以在 Windows 系統設定中另外尋找應用程式版本。  如果您無法成功登入用戶端，此案例適合用來報告應用程式版本。

若要在 Windows 系統設定中尋找應用程式版本，請開啟 [**開始] 功能表**，輸入 **應用程式 & 功能**，然後選取結果。 流覽至應用程式清單中的 **AltspaceVR** 。 以滑鼠左鍵按一下 [AltspaceVR]，然後從出現的功能表中選取 [ **Advanced Options** ]。

![[應用程式和功能] 功能表開啟時已醒目提示 [advanced] 選項](images/app-version-img-02.png)

在 [ **Advanced] 選項** 的 [ **規格** ] 標頭下， **應用程式版本** 應該會列在 [ **版本** ] 標籤的右邊。

![醒目提示應用程式版本開啟的 Advanced options](images/app-version-img-03.png)

### <a name="app-version-in-client-logs"></a>用戶端記錄中的應用程式版本

AltspaceVR 會在應用程式啟動期間，將用戶端記錄檔中的應用程式版本報告為「Altspace 版本」。 如果您無法成功登入用戶端，但它在失敗之前嘗試啟動，這會是取得應用程式版本的絕佳選項。

### <a name="windows"></a>Windows

在 Windows 上，您可以透過 Windows 檔案總管找到用戶端記錄檔：

```
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player.log
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player-prev.log
```

每次啟動 AltspaceVR 時，都會覆寫此檔案。 ' Player. log ' 代表您最新的會話，而 ' Player-prev ' 代表前一個會話。

### <a name="via-powershell"></a>透過 PowerShell

Advanced users 可以透過 PowerShell 搜尋此字串的用戶端記錄檔，如下所示：

輸入：

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

輸出：

[2.047] AltspaceVR 版本： 3.2.23. e66c2

## <a name="how-do-i-upload-my-client-logs"></a>如何? 上傳我的用戶端記錄？

AltspaceVR 用戶端應用程式會保存診斷資料的記錄，以及使用 AltspaceVR 時所發生的事件。 在針對問題進行疑難排解的過程中，系統可能會要求您「上傳您的記錄」，讓我們的小組可以複習它們。 這是 AltspaceVR 的一項功能，可讓您將本機記錄內容傳送給我們的小組，以協助我們針對您的問題進行疑難排解。

### <a name="in-altspacevr"></a>在 AltspaceVR 中

若要在 AltspaceVR 中上傳用戶端記錄檔，請流覽至 [ **設定] 功能表** ，然後選取左側導覽列中的 [ **支援** ]。 這裡有幾個上傳記錄的選項可用，如下列螢幕擷取畫面所示。

![開啟支援面板的設定功能表，並醒目提示 [記錄] 欄位](images/help-altvr-uploadlogs.png)

### <a name="fields"></a>欄位

**「發生錯誤的原因為何？」**
描述發生什麼事-例如，如果您發現 bug，請描述您預期會發生什麼事，而不是實際發生) 。 當您按下 [上傳] 時，此資訊會連同記錄一起傳送。

「 **Upload 記錄**」此按鈕將從目前的會話上傳記錄。 如果您在這個相同的會話中發現問題，請使用此選項 (例如，如果您尚未關閉 AltspaceVR 用戶端) ，而且想要報告它。

「 **Upload 上一個記錄**」此按鈕將會從上一個會話上傳記錄。

「 **Upload 上一個損毀記錄** 檔」此按鈕將會從您所遇到的最新損毀上傳更多記錄內容。

### <a name="in-client-logs"></a>在用戶端記錄中

您也可以從電腦取出記錄檔。 您可以在 [這裡](#app-version-in-client-logs)找到有關如何取得這些記錄檔的指示。


一旦找到這些檔案，請 [開啟支援票證](https://help.altvr.com/hc/en-us/requests/new) ，並上傳您的票證要求記錄，然後再按一下 [提交]。

## <a name="what-do-i-do-if-i-cant-launch-altspacevr"></a>如果無法啟動 AltspaceVR，該怎麼辦？

AltspaceVR 可能不會為您啟動的原因有好幾種。 請嘗試下列步驟，以確保應用程式已正確安裝所需的協力廠商軟體。

### <a name="if-youre-trying-to-launch-altspacevr-for-the-first-time"></a>如果您是第一次嘗試啟動 AltspaceVR：

1. 確認您的裝置受支援，並符合 [指定的最低需求](../getting-started/system-requirements.md)。
2. 請確定您已安裝最新的[Oculus 軟體](https://www.oculus.com/setup)，且設定 > 一般 > 的未知裝置設定為開啟。 如果以2D 模式啟動，您就不需要安裝 Oculus。
3. 請確定您有正常運作的網際網路連線。 如果您嘗試從網路防火牆內啟動 Altspace，請開啟 UDP 埠5055和5056，以及 TCP 埠80和443。 如果您是在公司或教育級防火牆的網路中，您可能需要聯繫網路系統管理員或 IT 部門。
4. 另請參閱：
    * [安裝 AltspaceVR 以進行 Oculus 的尋找](../getting-started/oculus-installation.md)
    * [安裝適用于 Windows Mixed Reality 的 AltspaceVR](../getting-started/wmr-installation.md)

### <a name="if-altspacevr-reports-that-the-current-version-is-out-of-date"></a>如果 AltspaceVR 報告目前版本已過期：

* 您所使用的應用程式版本已不再支援。 如果您是透過店面下載 AltspaceVR，更新可能會在您的商店更新用戶端之前先啟動。
* 如果您想要強制更新，您可以透過各種店面進行：
    * **Microsoft Store：** [Microsoft Store 支援-在 Microsoft Store 中取得應用程式和遊戲的更新](https://support.microsoft.com/account-billing/get-updates-for-apps-and-games-in-microsoft-store-a1fe19c0-532d-ec47-7035-d1c5a1dd464f)
    * **Oculus：** 開啟您的 Oculus 程式庫，並流覽至左側導覽列中的 [更新]。
    * **流出：** [流支援-更新 & 安裝問題](https://support.steampowered.com/kb_article.php?ref=2274-IFLV-5334)

### <a name="if-the-program-was-working-but-ceased-to-launch-after-update"></a>如果程式正常運作，但在更新之後不會啟動：

* 進行軟體的「全新重新安裝」。 這需要您卸載或移除應用程式的現有版本。 從系統完全移除之後，請透過串流、Oculus 或 Microsoft Store 安裝 Altspace。
* 如果您在啟動 AltspaceVR 時發生問題，請透過 [支援票證](https://help.altvr.com/hc/requests/new)讓我們知道。 從您的會話包含 [記錄](altspacevr-app-faq.md#how-do-i-upload-my-client-logs) 檔。

### <a name="if-altspacevr-fails-to-launch-after-customizing-your-home-space"></a>如果 AltspaceVR 在自訂您的主空間之後無法啟動：

* 流覽至您 [的首頁空間網站](https://account.altvr.com/users/sign_in)。
* 確認您的全球範本仍然存在。 如果範本已與您共用，則擁有者可能已刪除該範本，這會導致您的主空間無法載入。
    * 如果範本已刪除，只需從左側的 [全球工具] 面板中 [編輯]，將現有的範本取代為另一個範本，然後使用 [更新] 儲存變更。
* 從左側的 [世界工具] 面板中選取 [物件]，以移除任何可能無法載入的物件。 有問題的物件可能包括：
    * 來自已刪除之套件的物件，或從套件刪除的物件，仍存在於您的世界中。
    * 實驗性 GLTFs。
* 解決上述專案之後，請嘗試重新輸入 AltspaceVR。

如需更多網路系統管理員或 IT 部門的支援（包括 Azure IP 範圍和服務標記），請參閱我們的 [下載詳細資料](https://www.microsoft.com/en-us/download/details.aspx?id=56519)。

## <a name="support"></a>支援

AltspaceVR 團隊的問題或意見反應？ 

> [!div class="nextstepaction"]
> [按一下這裡以傳送支援要求](https://help.altvr.com/hc/requests/new)