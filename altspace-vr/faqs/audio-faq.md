---
title: AltspaceVR 音訊的常見問題
description: 疑難排解和支援音訊相關問題。
ms.date: 8/23/2021
author: qianw211
ms.author: v-qianwen
ms.topic: article
keywords: vr、音訊、疑難排解、支援
ms.openlocfilehash: 05c8a477b9e50b5067e62b934fe2ff8bd656f06c
ms.sourcegitcommit: 5c452a9092297c0bfbc8efabebf395e7ee31853f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/30/2021
ms.locfileid: "129311851"
---
# <a name="frequently-asked-questions-about-audio"></a>關於音訊的常見問題

## <a name="does-my-vr-headset-have-a-built-in-mic"></a>我的 VR 耳機是否有內建的 mic？

### <a name="oculus-riftrift-s-oculus-questquest-2-windows-mixed-reality-and-htc-vive"></a>Oculus Rift/Rift S、Oculus 的、Windows Mixed Reality 和 HTC Vive

是的，這些 VR 耳機有內建的麥克風。

### <a name="windows"></a>Windows

針對與 Windows 搭配使用的耳機，您應該能夠在您有耳機電源時，找到 **錄製裝置** 下所列的麥克風。

### <a name="further-troubleshooting"></a>進一步的疑難排解

* [AltspaceVR 支援-其他使用者無法聽取我的意見](#what-do-i-do-if-other-users-cant-hear-me)
* [AltspaceVR 支援-管理 Oculus 的許可權](../getting-started/oculus-controls.md#managing-permissions)

## <a name="is-there-a-push-to-talk-button"></a>是否有 [點擊對話] 按鈕？

沒有 [點擊對話] 按鈕。  如果您看一下視野的左下方，有一個麥克風圖示可用來切換語音。 或者，您也可以使用鍵盤快速鍵（空格鍵）來將麥克風靜音/取消靜音。

當您說話時，如果圖示閃爍，您的麥克風可以正常運作！
 
## <a name="what-do-i-do-if-my-audio-is-choppy"></a>如果音訊不穩定，該怎麼辦？

有些使用者注意到，當其他人為說話時，音訊會以斷斷續續或一般的方式出現。 其他使用者可能會在其他情況下通知您自己的音訊是透過斷斷續續或機器人。

首先要嘗試的是重新進入您所處的空間，如果失敗，甚至重新開機 AltspaceVR。 音訊問題並不常見，但在發生這種情況時，通常很容易就能解決問題。 

如果這項作業失敗，則您可以調查：

#### <a name="cpu-performance-for-desktop-users"></a>桌面使用者的 CPU 效能

請參閱我們建議用來執行 AltspaceVR 的硬體 [系統規格](../getting-started/system-requirements.md) 。 我們發現 i3 或較低的 Cpu 會造成問題，而不只是影片的畫面播放速率，也可以促成音訊問題，例如，捨棄和品質不良。

#### <a name="internet-bandwidth-and-network-connection"></a>網際網路頻寬和網路連接

低速網際網路連線 (小於 5mbps) 或 WiFi 的使用者可能會有音訊問題，例如下拉式。 我們建議您將乙太網路纜線連接到您的電腦，並以比5mbps 更快的速度 hardline 連接。 您可能會想要結束任何可能在背景中使用網際網路連線的程式。

## <a name="what-do-i-do-if-other-users-cant-hear-me"></a>如果其他使用者無法聽到我，該怎麼辦？

首先，判斷 AltspaceVR 是否偵測到您麥克風的音訊。 您可以藉由查看您的視圖左下方的麥克風圖示是否在說話時閃爍。 當您說話時，如果圖示閃爍，麥克風就會正常運作。 如果圖示為紅色，表示您已靜音。 選取圖示以將自己靜音或取消靜音。

如果在靜音之後看不到您的麥克風圖示閃爍，您可能需要調整 AltspaceVR 中的麥克風設定，移至 [功能表]/[設定/音訊/音訊輸入選擇]。 然後使用箭號按鈕來選取您想要使用的 Mic。
 
### <a name="oculus-questquest-2"></a>Oculus 的追求/進行中2

當您安裝 AltspaceVR 時，請務必授與使用 Mic 音訊的許可權。 您可以執行的另一項檢查如下：功能表/設定/音訊/音訊輸入選取範圍，並將其設定為 Android 音訊輸入，也就是 Quest2's 預設 mic。
 
### <a name="windows-mixed-reality-oculus-riftrift-s-htc-vive-or-2d-mode"></a>Windows Mixed Reality、Oculus Rift/Rift S、HTC Vive 或2d 模式

請確定您在 AltspaceVR：功能表/設定/音訊/音訊輸入選取專案中有正確的麥克風設定。 然後使用箭號按鈕來選取您想要使用的 Mic。

開始 AltspaceVR 之前，請確定已將適當的麥克風設定為 Windows 中的預設錄製裝置。 Oculus Rift/Rift S 和 HTC Vive 都有內建的麥克風，如果您已在 AltspaceVR 中插入另一個麥克風，則可能會嘗試使用該裝置。
 
若要在 Windows 中變更您的預設錄製裝置：

* 在 Windows 中，以滑鼠右鍵按一下您的喇叭圖示，然後選取 [**開啟音效設定**]。
* 流覽至 [ **輸入]/[選擇您的輸入裝置** ] 下拉式清單。
* 從下拉式功能表中選擇您想要使用的麥克風： 
    * HTC Vive 麥克風會標示為 [ **麥克風-USB 音訊裝置**]。
    * Oculus Rift 麥克風將標示為 **耳機麥克風 (Oculus 虛擬音訊裝置)**。
* 重新開機 AltspaceVR 之後，您的麥克風現在會被挑選
 
如果您在遵循這些步驟之後仍遇到問題，可能會對您造成影響的事項如下：

* 如果您 Alt-Tab 離開超過30秒，AltspaceVR 會自動將您靜音。 您可以在 **AltspaceVR 閒置時，于功能表 > 設定 > 音訊 > 靜音** 中停用此功能。
* AltspaceVR 音訊系統的磁片區閾值如下所示。 將 mic 層級設定為 [最大值]、將 mic 設定為靠近您的嘴，然後以一般磁片區說話。
* 結束 VR，嘗試將您的 USB 纜線從耳機插入替代 USB 3.0 埠。 在我們的經驗中，某些 USB 3.0 埠會造成問題。

AltspaceVR 可能無法辨識在遊戲中進行的音效設定變更，因此您可能需要重新開機 AltspaceVR，才能讓上述麥克風的變更生效。  當您重新輸入遊戲時，請查看麥克風圖示，看看是否在說話時閃爍。 如果圖示閃爍，表示您的麥克風正在運作。

## <a name="support"></a>支援

AltspaceVR 團隊的問題或意見反應？ 

> [!div class="nextstepaction"]
> [按一下這裡以傳送支援要求](https://help.altvr.com/hc/requests/new)