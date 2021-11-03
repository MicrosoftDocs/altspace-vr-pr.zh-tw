---
title: 錄製和即時串流
description: 瞭解如何錄製和即時串流您的 AltspaceVR 事件，以便與您的使用者進行升級和分享。
author: qianw211
ms.author: v-qianwen
ms.date: 11/1/2021
ms.topic: article
keywords: 串流、錄製、影片、音訊、youtube、obs、即時
ms.openlocfilehash: e82960097103df25c50f0b03b76d21e10b1cbbd6
ms.sourcegitcommit: 20605c50a93852f93a3464c5c339f6a7da67a047
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/03/2021
ms.locfileid: "131278974"
---
# <a name="recording-and-live-streaming"></a>錄製和即時串流

錄製和即時串流您的 AltspaceVR 體驗，以顯示世界各地的其他人，是在一般情況下宣傳您的活動、AltspaceVR 和 VR 的絕佳方法！ 請參閱下列各節，以瞭解如何開始使用。

在本文中，您將學會如何：

* [在電腦上以2D 模式錄製 AltspaceVR](#recording-altspacevr-in-2d-mode-on-pc)
* [在電腦上以2D 模式 AltspaceVR 至 YouTube 的即時串流](#live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc)

## <a name="recording-altspacevr-in-2d-mode-on-pc"></a>在電腦上以2D 模式錄製 AltspaceVR

### <a name="the-short-version"></a>簡短版本

1. AltspaceVR 和 OBS (開啟的廣播者軟體) 安裝。 以2D 模式啟動 AltspaceVR、啟動 OBS、將 OBS 設定為記錄 AltspaceVR 並記錄離開！

### <a name="the-slightly-longer-version"></a>稍長的版本

1. 訪問 [https://obsproject.com/](https://obsproject.com/)
2. 選取 **Windows** 下載 OBS。 這篇文章使用 **OBS v 26.1.1 版**
3. 安裝 OBS

### <a name="have-altspacevr-running-before-you-run-obs"></a>執行 OBS 之前，請先執行 AltspaceVR

1. 從我們的網站下載並安裝 AltspaceVR： [altvr.com/get](https://altvr.com/getaltspacevr)
2. 如果您想要讓您的 VR 影片穩定，並消除不穩定的標頭移動，請務必使用2D 用戶端，或從您的電腦撥接耳機的 USB 纜線，以2D 模式啟動 AltspaceVR。 如果您有 Rift，請按 Ctrl + Alt + Del、選取 [ **服務**]、[ **Oculus VR Runtime 服務**]、按一下滑鼠右鍵，然後選取 [ **停止**]。 這將會停用 Oculus 並以2D 模式啟動 AltspaceVR。 重複這些步驟，並使用 Start 來取回 VR 模式。
3. 您也可以使用遊戲捕捉搭配 OBS，以 VR 模式記錄您的體驗

現在，Alt-Tab 到 OBS：

1. 在 [ **場景**] 下，選取 **+** 並命名您的新場景
2. 接下來，在 [**來源**] 底下，選取： **+ > 遊戲捕捉 > 建立新** 的
2. 編輯文字至「AltspaceVR Capture」、勾選 [ **讓來源可見**]，然後選取 **[確定]**
3. 按兩下 [**來源**] 底下的 [ **AltspaceVR Capture** ]
4. 變更 **模式** 以 **抓取特定視窗**
5. 視窗： [AltspaceVR.exe]： AltspaceVR
6. 視窗符合優先順序：符合標題，否則尋找相同可執行檔的視窗
7. 向下滾動以 **捕捉資料指標**： untick
8. 選取 [確定]
9. 這應該會讓 AltspaceVR 顯示在 OBS 中。

現在，若要在 OBS 中設定下列屬性，請移至 [檔案 **>] 設定**：

|索引標籤|設定|
|---|---|
| **一般** | 保留預設值 |
| **串流** | 保留預設值 |
| **輸出** | 切換至 Advanced |
| **-資料流程索引標籤** | 音訊曲目1 <br> 編碼器： x264 <br> 重新調整輸出：未核取 <br> 速率控制： CBR <br> 位元速率： 6000 (6000，適用于 60 fps) 30 fps 或9000 <br> 主要畫面格間隔 = 2 <br> CPU 使用量預設值 = veryfast |
| **-記錄索引標籤** | 類型：標準 <br> 錄製路徑： D：/Video (流覽至您想要儲存的影片檔案)  <br> 記錄格式：有可能會在錄製時出現某些損毀的 (。如果您當機，則會在這裡嘗試使用 flv，而不是使用，如果您當機，則影片仍可使用 flv)  <br> 音訊曲目1 <br> 編碼器：使用串流編碼器 |
| **-音訊索引標籤** | 音訊位元速率：所有曲目的 160 ()  |
| **-重新執行緩衝區索引標籤** | 保留預設值 |
| **音訊** | 取樣率： 44.1 khz <br> 頻道：身歷聲 <br> 桌面音訊：預設 <br> 桌面音訊2：停用 <br> Mic/Aux 音訊：預設 |
| **影片** | 基底 (畫布) 解析度：1920x1080 <br> 輸出 (調整) 解析度：1920x1080 <br> 縮小濾波器：雙立方 (Sharpened 調整，16個樣本)  <br> 一般 FPS 值： 30 (或 60)  |
| **熱鍵** | 保留預設值 |
| **進階** | 進程優先順序：一般 | <br>

<br>好的， **現在請務必選取**[套用]，然後按一下 **[確定]** 儲存所有的 OBS 設定。 

1. Alt-Tab 移至 AltspaceVR，進入正確的空間/世界/事件，並將您的相機對齊 (也就是您的圖片) 我們即將錄製影片！
2. Alt-Tab 至 OBS，並在您準備好時，按一下 [ **開始錄製**]。

您將會在 OBS 的右下方看到 **REC：** 即將開始計算，而點是紅色，表示您正在錄製！

從下列內容進行測試記錄： 
1. 在 AltspaceVR 中開啟/關閉/變換功能表以讓 UI 音效
2. 請確定您已 unmuted，例如「Sibilance，Sibilance」，或讓另一位使用者在一般磁片區與您交談。
3. 當您這樣做時，請查看 **桌面音訊** 和 **Mic/Aux** 層級，以查看是否已正確地挑選音訊。

錄製時，通常會將 Mic/Aux 靜音。 請繼續並選取 Mic/Aux 的喇叭圖示，它會使用 X 來轉換紅色。

* 您很難將 mic 音訊等級與其他使用者的音訊進行比對，因此當您錄製活動時，Mic 最適合靜音。
* 音訊的另一個問題是 OBS 的設定方式。 它會從您的電腦中捕捉所有音訊，因此，如果您要觀賞 YouTube 或在電腦上取得通知音效，則會錄製該音訊。
* 若只要錄製 AltspaceVR 中的音訊，請移至 [**開啟磁片區混音** 器] (以滑鼠右鍵按一下 Windows) 的喇叭圖示，然後將 [系統音效]、[瀏覽器] 和 [靜音] 設為靜音，但不要將 OBS 或 AltspaceVR 靜音。

> 須知錄製之後，別忘了將這些磁片區混音器設定取消靜音。

現在，請流覽回到 OBS，然後選取 [ **停止錄製**]。 若要尋找您剛剛錄製的影片，請移至 [檔案 **>顯示錄製**]。 這會開啟包含您 OBS 影片檔案的資料夾，然後按兩下測試影片。

有時候錄製很多，因此請減少 OBS 中桌面音訊的滑杆，並進行另一項錄製以進行測試。

Pro 提示：使用 Ctrl + Alt + P 在攝影模式上切換，將會從您的視圖中移除 UI，以取得很好的乾淨快照。

恭喜您是 AltspaceVR 的影片錄製器！

## <a name="live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc"></a>在電腦上以 AltspaceVR 2D 模式即時串流至 YouTube

### <a name="the-short-version"></a>簡短版本

已安裝 AltspaceVR 和 OBS。 啟動 AltspaceVR 和 OBS。 您可以使用即時串流「立即」或「之後的日期」。 在 YouTube 上，使用您的 YouTube 串流金鑰設定 OBS。 開始在 OBS 和 YouTube 上進行串流處理，您也不會遇到競爭情形！

### <a name="the-slightly-longer-version"></a>稍長的版本

See the [Recording AltspaceVR in 2D mode on PC](#recording-altspacevr-in-2d-mode-on-pc) section at the top of this page for instructions on how to test recording using a local recording instead of the live stream, and how to get your camera shot set up.

## <a name="setting-up-live-streaming-on-youtube"></a>在 YouTube 上設定即時串流

您可以取得「立即」的即時串流，或使用「之後的日期」來設定未來的即時串流。

1. 開啟您的瀏覽器並登入 [https://www.youtube.com/](https://www.youtube.com/) ，然後前往 [https://studio.youtube.com/](https://studio.youtube.com/)
2. 查看右上方，然後選取 [ **建立** ] **，然後上線**

「**立即** 的」方法：

1. 選取 **立即的/開始**
1. 選取 **串流軟體/GO**
1. 選擇 **編輯**、右上角以編輯您的影片詳細資料和自訂
1. 在 [ **Stream 設定** 下，保留預設值
1. **在 [串流金鑰] 旁邊 (貼上編碼器)** 中，**複製** 金鑰，以便將它貼到 OBS
1. 開啟 OBS/**設定**  /  **資料流程**
1. 在 [ **服務** ] 下拉式功能表中，選取 [ **YouTube-RTMPS**
1. 將串流金鑰從 YouTube 貼到 OBS 中的 [ **串流金鑰** ] 欄位
1. 按一下[套用]，然後按一下 **[確定]**
1. 選取 [在 OBS 中 **啟動串流** ]
1. 切換至 YouTube，您將會看到您現在已上線至 YouTube！
1. 若要查看您實際的 YouTube live stream 影片頁面，您必須選取右上方的共用圖示
1. 按一下 [影片連結]，您就會看到並聆聽您的 YouTube live stream 
1. 此 URL 是您的即時串流連結，可與您的所有社交頻道共用： ) 
1. 若要停止即時串流，請選取 YouTube 上的 [結束串流]，然後在 OBS 上停止串流

「**之後的日期**」方法：
1. 選擇左上方的 [ **管理** ] 圖示
1. 選取 **排程資料流程**，右上方
1. 新增標題、描述、分類 (1280x720) 的縮圖，然後按 **[下一步]**
1. Live chat 選項 **，接著**
1. 私用、未列出或公用 (選擇公用) 
1. 排程您要上線的日期和時間，然後 **進行**

 **當您準備好在未來開始實況串流時：**
1. 在 [Stream 設定下，保留預設值
1. **在 [串流金鑰] 旁邊 (貼上編碼器)** 中，**複製** 金鑰，以便將它貼到 OBS
1. 開啟 OBS/**設定**  /  **資料流程**
* 在 [ **服務** ] 下拉式功能表中，選取 [ **YouTube-RTMPS**
1. 將串流金鑰從 YouTube 貼到 OBS 中的 [ **串流金鑰** ] 欄位
1. 按一下[套用]，然後按一下 **[確定]**
1. 選取 [在 OBS 中 **啟動串流** ]
1. 切換至 YouTube，您將會看到您現在已上線至 YouTube！
1. 若要查看您實際的 YouTube live stream 影片頁面，您必須選取右上方的共用圖示
1. 按一下 [影片連結]，您就會看到並聆聽您的 YouTube live stream 
1. 此 URL 是您的即時串流連結，可與您的所有社交頻道共用： ) 
1. 若要停止即時串流，請選取 YouTube 上的 [**結束串流**]，然後在 OBS 上 **停止串流**

針對額外得分，請分享您的社交影片，並務必標記我們 @AltspaceVR ： ) 