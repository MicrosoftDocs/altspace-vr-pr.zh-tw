---
title: 我無法啟動 AltspaceVR
description: 瞭解如何識別、報告和修正任何與啟動 AltspaceVR 環境相關的問題。
ms.date: 02/10/2021
ms.topic: article
keywords: 常見問題
ms.openlocfilehash: 50edddef669aca14640fd6e910c12c15864cf46a099e54bceed40494e9817de4
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127924"
---
# <a name="i-cant-launch-altspacevr"></a>我無法啟動 AltspaceVR

AltspaceVR 可能不會為您啟動的原因有好幾種。 請嘗試下列步驟，以確保應用程式已正確安裝所需的協力廠商軟體。

## <a name="if-youre-trying-to-launch-altspacevr-for-the-first-time"></a>如果您是第一次嘗試啟動 AltspaceVR：

1. 確認您的裝置受支援，並符合 [指定的最低需求](../getting-started/system-requirements.md)。
2. 請確定您已安裝最新的[Oculus 軟體](https://www.oculus.com/setup)，且設定 > 一般 > 的未知裝置設定為開啟。 如果以2D 模式啟動，您就不需要安裝 Oculus。
3. 請確定您有正常運作的網際網路連線。 如果您嘗試從網路防火牆內啟動 Altspace，請開啟 UDP 埠5055和5056，以及 TCP 埠80和443。 如果您是在公司或教育級防火牆的網路中，您可能需要聯繫網路系統管理員或 IT 部門。
4. 另請參閱：
    * [安裝 AltspaceVR 以進行 Oculus 的尋找](../getting-started/oculus-installation.md)
    * [安裝適用于 Windows Mixed Reality 的 AltspaceVR](../getting-started/wmr-installation.md)

## <a name="if-altspacevr-reports-that-the-current-version-is-out-of-date"></a>如果 AltspaceVR 報告目前版本已過期：

* 您所使用的應用程式版本已不再支援。 如果您是透過店面下載 AltspaceVR，更新可能會在您的商店更新用戶端之前先啟動。
* 如果您想要強制更新，您可以透過各種店面進行：
    * **Microsoft Store：** [Microsoft Store 支援-在 Microsoft Store 中取得應用程式和遊戲的更新](https://support.microsoft.com/account-billing/get-updates-for-apps-and-games-in-microsoft-store-a1fe19c0-532d-ec47-7035-d1c5a1dd464f)
    * **Oculus：** 開啟您的 Oculus 程式庫，並流覽至左側導覽列中的 [更新]。
    * **流出：** [流支援-更新 & 安裝問題](https://support.steampowered.com/kb_article.php?ref=2274-IFLV-5334)

## <a name="if-the-program-was-working-but-ceased-to-launch-after-update"></a>如果程式正常運作，但在更新之後不會啟動：

* 進行軟體的「全新重新安裝」。 這需要您卸載或移除應用程式的現有版本。 從系統完全移除之後，請透過串流、Oculus 或 Microsoft Store 安裝 Altspace。
* 如果您在啟動 AltspaceVR 時發生問題，請透過 [支援票證](https://help.altvr.com/hc/requests/new)讓我們知道。 從您的會話包含 [記錄](uploading-client-logs.md) 檔。

## <a name="if-altspacevr-fails-to-launch-after-customizing-your-home-space"></a>如果 AltspaceVR 在自訂您的主空間之後無法啟動：

* 流覽至您 [的首頁空間網站](https://account.altvr.com/users/sign_in)。
* 確認您的全球範本仍然存在。 如果範本已與您共用，則擁有者可能已刪除該範本，這會導致您的主空間無法載入。
    * 如果範本已刪除，只需從左側的 [全球工具] 面板中 [編輯]，將現有的範本取代為另一個範本，然後使用 [更新] 儲存變更。
* 從左側的 [世界工具] 面板中選取 [物件]，以移除任何可能無法載入的物件。 有問題的物件可能包括：
    * 來自已刪除之套件的物件，或從套件刪除的物件，仍存在於您的世界中。
    * 實驗性 GLTFs。
* 解決上述專案之後，請嘗試重新輸入 AltspaceVR。

如需更多網路系統管理員或 IT 部門的支援（包括 Azure IP 範圍和服務標記），請參閱我們的 [下載詳細資料](https://www.microsoft.com/en-us/download/details.aspx?id=56519)。