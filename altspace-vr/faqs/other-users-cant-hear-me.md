---
title: 其他使用者無法聽取我的意見
description: 瞭解如何找出並修正與其他使用者無法在 AltspaceVR 中聽到我的問題。
ms.date: 03/11/2021
ms.topic: article
keywords: 常見問題
ms.openlocfilehash: 189d96790207085a2a2c47e964c0db8a08ed95a76d91d2ced3026ba3455b45e3
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "119128087"
---
# <a name="other-users-cant-hear-me"></a>其他使用者無法聽取我的意見

首先，判斷 AltspaceVR 是否偵測到您麥克風的音訊。 您可以藉由查看您的視圖左下方的麥克風圖示是否在說話時閃爍。 當您說話時，如果圖示閃爍，麥克風就會正常運作。 如果圖示為紅色，表示您已靜音。 選取圖示以將自己靜音或取消靜音。

如果在靜音之後看不到您的麥克風圖示閃爍，您可能需要調整 AltspaceVR 中的麥克風設定，移至 [功能表]/[設定/音訊/音訊輸入選擇]。 然後使用箭號按鈕來選取您想要使用的 Mic。
 
## <a name="oculus-quest"></a>Oculus Quest 

當您安裝 AltspaceVR 時，請務必授與使用 Mic 音訊的許可權。 您可以執行的另一項檢查如下：功能表/設定/音訊/音訊輸入選取範圍，並將其設定為 [Android 音訊輸入] (這是 [執行/Quest2's] 預設 mic) 。
 
## <a name="windows-mixed-reality-oculus-rift-htc-vive-or-2d-mode"></a>Windows Mixed Reality、Oculus Rift、HTC Vive 或2d 模式

請確定您在 AltspaceVR：功能表/設定/音訊/音訊輸入選取專案中有正確的麥克風設定。 然後使用箭號按鈕來選取您想要使用的 Mic。

開始 AltspaceVR 之前，請確定已將適當的麥克風設定為 Windows 中的預設錄製裝置。 Oculus Rift 和 HTC Vive 都有內建的麥克風，如果您有另一個麥克風插入 AltspaceVR 可能會嘗試使用該裝置。
 
若要在 Windows 中變更您的預設錄製裝置：
* 在 Windows 中，以滑鼠右鍵按一下您的喇叭圖示，然後選取 [**播放裝置**]。
* 流覽至 [ **錄製** ] 索引標籤
* 尋找您想要使用的麥克風。 HTC Vive 麥克風會標示為 [ **麥克風-USB 音訊裝置** ]，而 Oculus Rift 麥克風則會標示為 [ **麥克風-Rift 音訊**]。
* 以滑鼠右鍵按一下該麥克風，然後選取 [**設為預設裝置**]
* 重新開機 AltspaceVR 之後，您的麥克風現在會被挑選
 
在遵循這些步驟之後，您仍會遇到一些其他問題，這些問題可能會影響您：
* 如果您 Alt-Tab 超過30秒的時間，AltspaceVR 會 automute 您，您可以使用鍵盤快速鍵停用此功能：空格鍵以關閉/開啟靜音。
* AltspaceVR 音訊系統的磁片區閾值如下所示。 將 mic 層級設定為 [最大值]、將 mic 設定為靠近您的嘴，然後以一般磁片區說話。
* 結束 VR，嘗試將您的 USB 纜線從耳機插入替代 USB 3.0 埠。 在我們的經驗中，某些 USB 3.0 埠會造成問題。

AltspaceVR 可能無法辨識在遊戲中進行的音效設定變更，因此您可能需要重新開機 AltspaceVR 以上的麥克風變更才會生效。  當您重新輸入遊戲時，請查看麥克風圖示，看看它是否閃爍。 如果圖示閃爍，表示您的麥克風正在運作。