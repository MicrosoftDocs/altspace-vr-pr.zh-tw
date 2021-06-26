---
title: 全球建築工具組簡介
description: 瞭解如何使用 Unity 場景範本搭配全球建築工具組來設定和上傳您的 AltspaceVR 世界。
ms.date: 03/11/2021
ms.topic: article
keywords: 工具箱
ms.openlocfilehash: 3b41f02aec1077a37b95a6826c105e1cd31974e3
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923075"
---
# <a name="introducing-the-world-building-toolkit"></a>全球建築工具組簡介

> [!NOTE]
> 「世界建築」工具組是由我們很棒的朋友 [Anthony Madden](https://twitter.com/chigamesstudio)所執行的一項社區專案，並提供我們的支援。 如果您有興趣，請加入 [官方 AltspaceVR 但是](https://discordapp.com/invite/altspacevr) ，並造訪 #world 大樓頻道。 目前有 Mac 試用版 Beta 版， [還有更多詳細資料](https://altvr.com/altspacevr-mac)

上載程式可讓您使用 Unity 場景作為您的世界的範本。 您可以從 Minecraft 帶入鬼房子或您最愛的建立。 如果您可以將它匯入 Unity，您可能會以這種方式 Altspace。 以下是一些 [範例領域](https://account.altvr.com/worlds/1046572460192825569)。

![範例世界](images/unity-uploader-img-01.png)

## <a name="setup"></a>安裝程式

1. 加入 [官方的 AltspaceVR 但是](https://discordapp.com/invite/altspacevr) ，並造訪 #world 大樓頻道-朋友不會讓朋友單獨建立世界。
2. 閱讀我們的 [世界大樓開始使用指南](world-building-getting-started.md) 以瞭解基本概念
3. [安裝 Unity Hub](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) 並安裝 **unity 2020.3.9**。 除非您完全符合此版本，否則上載者將無法運作。 如果您沒有帳戶，您將需要免費的 Unity 帳戶，並選擇 [ **個人** ]，因為這樣做可讓您享受更多樂趣！ 在安裝期間，請確定勾選 [ **Android 組建** ] 選項，並停用自動更新。
4. [下載最新的 Unity 上載者](upgrading-content-to-the-latest-unity.md#altspacevr-uploader-v090-upgrade-guide)
5. 在我們的網站上[建立範本](https://account.altvr.com/space_templates/new)。 將它命名 **Hello World 範本**。
6. [建立世界](https://account.altvr.com/worlds/my) 並 **Hello World** 命名。 選取 **Hello World 範本** 作為範本。

![建立的世界畫面](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a>上傳您的場景

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-a-Template/player]

1. 開啟 Unity 中樞，並建立新的 Unity 2020.3.9 專案。
2. 當您的專案開啟時，按兩下您所下載的檔案，以匯入上載程式， (它是 Unity 套件) 。 您現在應該會看到名為 **AltspaceVR** 的新索引標籤。 您必須針對要與 Altspace 搭配使用的每個 Unity 專案匯入套件
3. 開啟 **功能表 > AltspaceVR > 組建設定**
4. 使用您的 Altspace 帳號憑證登入
5. 選取 [**載入範本**]，然後選取 [ **Hello World 範本**]
6. 將 cube 新增至場景並儲存。
7. **要檢查 Windows 的組建嗎？** 然後取消核取 **Android 的組建？**
8. 選取 [上傳]。 大約一分鐘，您應該會看到 **上傳** 完成。
9. 藉由啟動 Altspace 並從 **功能表 > 世界 > 我的世界** 來加入 **Hello World**
10. 從 **功能表 > 設定 > 適中 > 重設空間** 重設世界
11. 您應該會看到 cube。 如果您在上述影片中快速進行，您可以在最少10秒內看到變更。

## <a name="whats-supported"></a>支援的項目

* 是：模型、衝突、動畫、粒子效果、音訊、skyboxes 等等
* 否：腳本。 基於安全性考慮，包含腳本的上傳將會遭到拒絕
* 也許：動態全球照明這類的有趣事物
* 個別或一起針對不同的平臺上傳場景
* 查看 [精選領域](https://account.altvr.com/worlds/featured)，許多都是使用上傳者建立的

## <a name="tips"></a>提示

* 加入 [官方 AltspaceVR 但是](https://discordapp.com/invite/altspacevr)。
* 在左側的範本頁面上，我們會顯示依平臺的最新上傳。 如果成功，您會看到 **1-2 分鐘前**。Screen_Shot_2019-01-11 _at_1.21.04_AM.png

![已反白顯示上傳的範本面板開啟](images/unity-uploader-img-03.png)

* 當您更新時，可以在世界各地。 當上傳者顯示 **上傳完成** 時，您可以重設世界以查看變更。
* 使用簡單的場景來建立電腦的功能，應該不到1分鐘的時間，就能在 Altspace 中看到變更
* 將您的世界設為私用且未列出，以避免分散注意力。
* 將 cube 放置於來源，讓您可以看到人員預設會產生的位置。 上傳時隱藏 cube。

## <a name="troubleshooting"></a>疑難排解

**我正在進行或無法傳送至任何** 您必須將衝突新增至物件，以傳送至這些物件。

**沒有變更**
    * 您是否已將場景儲存在 Unity 中？
    * 您選擇要測試的平臺嗎？
    * 你是在正確的世界嗎？ 您是否在上載者和世界表單中選擇正確的範本？
    * 您是否已檢查範本頁面統計資料？

**上傳失敗或超時**
    * 最常見的上傳錯誤是 Unity 版本錯誤。 它必須完全符合所需的版本。
    * 您的上傳可能太大。 請嘗試保持電腦幕後 < 100 MB。 從小規模開始，然後建立。 Optimize、optimize、optimize。
    * 使用簡單的 cube 來試用全新的專案。
    * 請勿在組建期間強制結束--它可能會損毀您的場景。 嘗試將。

**這是緩慢的流程**
    * 建議您在稍後逐一查看和 Android 時，才建立電腦。
    * 嘗試移除未使用的檔案。 基於任何原因，Unity 有時候會過度。

**我無法使用 Altspace 認證登入**
    * 電子郵件會區分大小寫。
    * 以新的專案嘗試。
    * 請確定您的 Altspace 帳戶良好。

## <a name="see-also"></a>另請參閱

* [Unity 學習](https://unity3d.com/learn)
* [Unity 論壇](https://forum.unity.com)
