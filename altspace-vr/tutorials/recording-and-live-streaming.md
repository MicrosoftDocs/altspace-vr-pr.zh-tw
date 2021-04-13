---
title: 錄製和即時串流
description: 瞭解如何錄製和即時串流您的 AltspaceVR 事件，以便與您的使用者進行升級和分享。
ms.date: 02/10/2021
ms.topic: article
keywords: 串流、錄製
ms.openlocfilehash: 80d54407915af1a0d4b7783858446f54205e6a2a
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212552"
---
# <a name="recording-and-live-streaming"></a>錄製和即時串流

錄製和即時串流您的 AltspaceVR 體驗，以顯示世界各地的其他人，是在一般情況下宣傳您的活動、AltspaceVR 和 VR 的絕佳方法！ 請看下面的內容，瞭解如何開始使用：

在本文中，您將學會如何：

* [如何在電腦上以2D 模式錄製 AltspaceVR](#recording-altspacevr-in-2d-mode-on-pc)
* [如何在電腦上以2D 模式即時串流至 YouTube AltspaceVR](#live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc)

## <a name="recording-altspacevr-in-2d-mode-on-pc"></a>在電腦上以2D 模式錄製 AltspaceVR

### <a name="the-short-version"></a>簡短版本

已安裝 AltspaceVR 和 OBS。 以2D 模式啟動 AltspaceVR、啟動 OBS、將 OBS 設定為記錄 AltspaceVR 並記錄離開！

### <a name="the-slightly-longer-version"></a>稍長的版本

1. 訪問 [https://obsproject.com/](https://obsproject.com/)
2. 選取 [ **Windows** ] 以下載 OBS。 這篇文章使用 **OBS v 22.0.2**
3. 安裝 OBS

### <a name="have-altspacevr-running-in-2d-mode-before-you-run-obs"></a>執行 OBS 之前，請先以2D 模式執行 AltspaceVR

1. 從我們的網站下載並安裝 AltspaceVR： [altvr.com/get](https://altvr.com/getaltspacevr)
2. 請務必從您的電腦撥出 HMD 的 USB 纜線，或如果您有 Rift： Ctrl + Alt + Del、Services、Oculus VR Runtime 服務、按一下滑鼠右鍵、停止，以2D 模式啟動 AltspaceVR。 
    * 這將會停用 Oculus 並以2D 模式啟動 AltspaceVR，請重複這些步驟，並使用 Start 來取回 VR 模式。

現在，Alt-Tab 到 OBS：

1. 在 [來源] 底下，選取 [ **+ > 遊戲捕獲] > 建立新** 的
2. 編輯文字至「AltspaceVR Capture」、勾選 [ **讓來源可見**]，然後選取 [確定]
3. 按兩下 [來源] 底下的 [ **AltspaceVR Capture** ]
4. 變更 **模式** 以 **抓取特定視窗**
5. 視窗： [AltspaceVR.exe]： AltspaceVR
6. 視窗符合優先順序：符合標題，否則尋找相同可執行檔的視窗
7. 向下滾動以捕捉資料指標： untick 確定

這應該會讓 AltspaceVR 顯示在 OBS 中。 現在，若要在 OBS 中設定下列屬性，請移至 [檔案 **> 設定**：

| 索引標籤 | 設定 |
|---|---|
| 一般 | 保留預設值 |
| 串流 | 保留預設值 |
| 輸出模式：切換至 Advanced | [資料流程] 索引標籤 <br> 音訊曲目1 <br> 編碼器： x264 <br> 強制串流服務編碼器設定：滴答 <br> 重新調整輸出：未核取 <br> 速率控制： CBR <br> 位元速率： 6000 (6000，適用于 60 fps) 30 fps 或9000 <br> 主要畫面格間隔 = 2 <br> CPU 使用量預設值 = veryfast |
| 記錄 | 類型：標準 <br> 錄製路徑： D：/Video (流覽至您想要儲存影片檔案的位置)  <br> 錄製格式：有可能會在錄製時出現某些損毀的 (。如果您損毀影片仍可搭配使用 flv，請在這裡嘗試使用 flv)  <br> 音訊曲目1 <br> 編碼器：使用串流編碼器 |
| 音訊 | 音訊位元速率：所有曲目的 160 ()  |
| 重新執行緩衝區 | 保留預設值 |
| 音訊 | 取樣率：48khz <br> 頻道：身歷聲 <br> 桌面音訊裝置：預設 <br> 桌面音訊裝置2：停用 <br> Mic/Aux 音訊裝置：預設 |
| 影片 | 基底 (畫布) 解析度：1920x1080 <br> 輸出 (調整) 解析度：1920x1080 <br> 縮小濾波器：雙立方 (Sharpened 調整，16個樣本)  <br> 一般 FPS 值：30 |
| 熱鍵 | 保留預設值 |
| 進階 | 進程優先順序：一般 |

好的， **現在請務必選取**[套用]，然後按一下 **[確定]** 儲存所有的 OBS 設定。 

1. Alt-Tab 移至 AltspaceVR，進入正確的空間/世界/事件，並將您的相機對齊 (也就是您的圖片) 我們即將錄製影片！
2. Alt-Tab 至 OBS，並在您準備好時，按一下 [ **開始錄製**]。

您將會在 OBS 的右下方看到該 REC：將開始計算，這表示您正在錄製！

從下列內容進行測試記錄： 
1. 在 AltspaceVR 中開啟/關閉/變換功能表以讓 UI 音效
2. 說「Sibilance，Sibilance」，讓另一位使用者在一般磁片區與您對話，或觀看2D 顯示器上的影片。
3. 查看桌面音訊和 Mic/Aux 層級，因為這樣做可查看其運作是否正常。

錄製時，通常會將 Mic/Aux 靜音。 請繼續並選取 Mic/Aux 的喇叭圖示，它會使用 X 來轉換紅色。

* 與您的音訊和其他使用者的音訊相符很難，因此 Mic 的音效最好是靜音。
* 音訊的另一個問題是 OBS 的設定方式。 它會從您的電腦中捕捉所有音訊，因此，如果您要觀賞 YouTube，則會記錄該音訊或可寬比的郵件或通知音效。
* 若只要從 AltspaceVR 錄製音訊，請移至音量混音器 (以滑鼠右鍵按一下 Windows) 右下方的喇叭圖示，並將 [系統音效]、[瀏覽器] 等靜音，但不要將 OBS 或 AltspaceVR 靜音。

> [!IMPORTANT]
> 請記得在錄製之後，將這些音量混音器設定重新開啟。

現在，流覽回 OBS，然後選取 [從檔案 **停止錄製** **>顯示錄製**]。 這會開啟包含您 OBS 影片檔案的資料夾，然後按兩下測試影片。

有時候錄製很多，因此請降低桌面音訊的滑杆，並進行另一項錄製以進行測試。

<!-- Missing image -->

## <a name="live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc"></a>在電腦上以 AltspaceVR 2D 模式即時串流至 YouTube

### <a name="the-short-version"></a>簡短版本

已安裝 AltspaceVR 和 OBS。 以2D 模式啟動 AltspaceVR、啟動 OBS、即時串流或在 YouTube 上建立「新的實況活動」、使用 YouTube 串流金鑰設定 OBS、以 YouTube 串流金鑰開始串流、在 YouTube 上開始串流處理、開始在 YouTube 上進行串流處理！

### <a name="the-slightly-longer-version"></a>稍長的版本

1. 訪問 [https://obsproject.com/](https://obsproject.com/)
2. 按一下 [ **Windows** ] 以下載 OBS (這篇文章使用 OBS v 22.0.2) 
3. 安裝 OBS

執行 OBS 之前，請先以2D 模式執行 AltspaceVR
1. 從我們的網站下載 AltspaceVR： [https://account.altvr.com/downloads](https://account.altvr.com/downloads)
2. 若要確定您以2D 模式啟動 AltspaceVR，請從電腦拔下 HMD 的 USB 纜線，或如果您有 Rift： Ctrl + Alt + Del、Services、Oculus VR Runtime 服務、按一下滑鼠右鍵、停止。 這將會停用 Oculus Home 並以2D 模式啟動 AltspaceVR、重複這些步驟，並開始重新取得 VR 模式。

Alt-Tab 到 OBS

1. 在 [來源] 底下，選取 [ **+** 遊戲捕捉]、[建立新的]、[編輯文字] 至 [AltspaceVR Capture]、勾選 [讓來源可見、正常]
2. 按兩下 AltspaceVR Capture
3. 模式：捕獲特定視窗
4. 視窗： [AltspaceVR.exe]： AltspaceVR
5. 視窗符合優先順序：符合標題，否則尋找相同可執行檔的視窗
6. 向下滾動以捕捉資料指標： untick 確定

這應該會讓 AltspaceVR 顯示在 OBS 中。 太好了！

現在在 OBS 中會前往檔案>設定

| 索引標籤 | 設定 |
|---|---|
| 一般 | 當串流 (這會將影片檔案記錄至您的電腦，以及即時串流) 時，會自動進行滴答記錄 |
| 串流 | 資料流程類型：串流服務 <br> 服務： YouTube/YouTube 遊戲 (也可以串流至 Twitch、混音器、Facebook Live 等 ) <br>伺服器：主要 YouTube 內嵌伺服器 <br>串流金鑰：從 YouTube * * _ 貼上您的串流金鑰 (請參閱「即時設定 <br>在 YouTube 上串流處理)  |
| 輸出 | 輸出模式：切換至 Advanced |
| 串流 | 音訊曲目1 <br>編碼器： x264 <br>tick 強制串流服務編碼器設定 <br>重新調整輸出：未核取 <br>速率控制： CBR <br>位元速率： 6000 (6000，適用于 60 fps) 30 fps 或9000 <br>主要畫面格間隔 = 2 <br>CPU 使用量預設值 = veryfast |
| 記錄 | 類型：標準 <br>錄製路徑： D：/Video (流覽至您想要儲存影片檔案的位置，如果您已選取 [串流處理時自動記錄])  <br>錄製格式：有可能會在錄製時出現某些損毀的 (。如果您損毀影片仍可搭配使用 flv，請在這裡嘗試使用 flv)  <br>音訊曲目1 <br>編碼器：使用串流編碼器 |
| 音訊 | 音訊位元速率：適用于所有曲目的 160 () 取樣率：48khz <br>頻道：身歷聲 <br>桌面音訊裝置：預設 <br>桌面音訊裝置2：停用 <br>Mic/Aux 音訊裝置：預設 |
| 重新執行緩衝區 | 保留預設值 |
| 影片 | 基底 (畫布) 解析度：1920x1080 <br>輸出 (調整) 解析度：1920x1080 <br>縮小濾波器：雙立方 (Sharpened 調整，16個樣本)  <br>一般 FPS 值：30 |
| 熱鍵 | 保留預設值 |
| 進階 | 進程優先順序：一般 |

好的，現在請務必按一下 [套用]，再按一下 [確定]，然後關閉並重新開啟 OBS。 這會儲存您所有的 OBS 設定。 美觀： ) 

請參閱上面的「如何錄製電腦2D 模式的 AltspaceVR」一節中的指示，以瞭解如何使用本機錄製（而不是即時串流）來測試錄製，以及如何在錄製之前先取得攝影機照片設定。

音訊的另一個問題是 OBS 的設定方式。 它會從您的電腦中捕捉所有音訊，因此，如果您要觀賞 YouTube，則會記錄該音訊、小組訊息或通知聲音。

若只要從 AltspaceVR 錄製音訊，請移至音量混音器 (以滑鼠右鍵按一下 Windows) 右下方的喇叭圖示，並將 [系統音效]、[瀏覽器] 等靜音，但不要將 OBS 或 AltspaceVR 靜音。

請不要忘了在錄製後再重新開啟，) 

### <a name="setting-up-live-streaming-on-youtube"></a>在 YouTube 上設定即時串流

您可以實際快速取得即時串流 (即時串流) 或設定未來的即時串流活動， (新的實況活動) 。 我可能會建議您將它設定為「新的實況活動」。

1. 開啟您的瀏覽器並登入 [https://www.youtube.com/](https://www.youtube.com/)
2. 選取您的帳戶圖示，右上方，從下拉式清單中選取 Creator Studio
3. 頁面左側的即時串流。

「立即串流」方法會變更縮圖，如果您需要變更基本資訊編碼器安裝程式將伺服器 URL 保持為預設值 _ * * 資料流程名稱/金鑰，請按一下 [顯示]，並複製此金鑰開啟 OBS 設定資料流程將此值貼到 [資料流程金鑰套用]，然後按一下 [開始串流切換至 YouTube]，您就會看到現在已上線 YouTube！
若要查看您實際的 YouTube live stream 影片頁面，您需要向下移動並查看共用連結的右下角。
將它複製並貼到新的瀏覽器索引標籤，然後按一下 [影片]。您會在清單中看到您的影片，它會立即顯示，按一下該畫面，您就會看到您的 YouTube 即時串流頁面。
此 URL 是您的即時串流連結，可與您的所有社交頻道共用： ) 若要停止即時串流，請按一下 [OBS] 上的 [停止串流]，這會結束 YouTube 上的即時串流。

「事件」方法： https://www.youtube.com/my_live_events 按一下 [新增實況活動] 新增標題、日期、開始時間、描述和標記-別忘了標記 AltspaceVR： ) 從下拉式功能表類型選擇 [公用]：如果您想要新增自訂縮圖，請按一下 [流覽]，然後上傳您的影像。  (1280x720 最適合) 選取：單次使用串流金鑰選取您的編碼器：其他編碼器複製資料流程名稱 (串流金鑰) 

現在以滑鼠右鍵按一下 [監看式監看式頁面] 和 [在新索引標籤中開啟連結]

這是您的 YouTube live stream 活動連結，可在您的實際活動前以社交方式共用！

現在開啟 OBS 檔>設定資料流程將您剛複製的資料流程金鑰貼到 [資料流程金鑰] 欄位，然後按一下 [儲存變更]，以滑鼠右鍵按一下 [Live Control 會議室] 和 [在新索引標籤中開啟連結]，然後再按一下 [開始串流處理]，再按一下 [開始串流處理]。您會看到 [預覽] 按鈕現在是藍色，請按一下 [預覽按鈕] 對話方塊，詢問您是否要預覽實況活動、[確定]，然後您會看到 [開始串流處理] 按鈕按一下 [開始串流處理] 對話方塊，詢問您是否要串流處理實況活動，確定

您現在已經上線了！

移至您的瀏覽器索引標籤，並開啟 [觀賞 Watch 頁面] 連結，以確定影片看起來不錯。 請記住，您不會聽到音訊，因為當您在 Windows 音量混音器中將音訊靜音時，就會關閉瀏覽器的音訊。 檢查手機上的音訊，或要求朋友為您檢查音訊。

查看良好！

Alt-Tab 回到 AltspaceVR，將您的攝影機移 (也就是您的活動周圍) 。

當您完成實況串流之後，請回到 YouTube 的 [Live Control 會議室] 頁面

按一下 [停止串流]

對話方塊隨即開啟，詢問您是否要停止串流處理實況活動，確定

移至 OBS，然後按一下 [停止串流]。

恭喜您現在是 AltspaceVR 的流處理器！


Recording_AltspaceVR_.png


針對額外的點數，與全世界的社交媒體共用您的影片，並確定標記 @AltspaceVR ： ) 