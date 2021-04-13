---
title: Unity 上載者說明
description: 隨時掌握最新的 AltspaceVR Unity 上傳程式常見問題和解決方案。
ms.date: 02/10/2021
ms.topic: article
keywords: 說明，常見問題
ms.openlocfilehash: 814ff293cb98490900cd929f33477d15d3d668ae
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212493"
---
# <a name="unity-uploader-help"></a>Unity 上載者說明

**1. 這項工具有多棒？**

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/cheyenne-mountain-gate-room-v1/player]

這就是我的 Stargate Unity 場景，內含可為閘道和 DND 提供的 SDK 應用程式

**2. 我是影片學習模組，我的影片在哪裡？**

[查看我們的影片](https://youtu.be/km9CnVYPzoM)

**3. 我可以在哪裡找到範例？**

[精選的世界](https://account.altvr.com/worlds/featured) 和 [Jimmy 的範例](https://account.altvr.com/worlds/1046572460192825569) 是很好的起點

**4. 這是否適用于套件和新的 SDK？**
是的，如果您想要的話，可以一起使用所有工具。 我們正在嘗試開發它們，以便緊密合作。

**5. 它是否支援粒子效果？**

![雪粒子效果的 GIF](images/uploader-faq-img-01.gif)

**6. 我可以取得 hrtf 音訊嗎？**
目前不是，但您可以放置音訊來源，以在當地語系化的區域中播放。 

**7. 內建光源是否正常運作？**
是，但您的燈光必須設定為 "內建"，而不是「混合」

**8. 全球照明是否正常運作？**
Yes

**9. 您一定要重設世界嗎？**
是。 每次都必須重載 Unity 資產套件組合。 

**10. 我可以使用自己的自訂材質和著色器嗎？**

![自訂材質和著色器的 GIF](images/uploader-faq-img-02.gif)

**11. 我可以只上傳到一個平臺嗎？**
是，使用上載工具。 不過，在 Android 上的人員在您上傳其平臺的場景之前，將不會看到您世界中的任何事物。 

**12. 是否允許腳本？**
否，基於安全性理由，我們不能允許腳本或腳本參考。 如果您的上傳包含腳本或腳本參考，則會被拒絕。 如果您的世界需要撰寫腳本，請參閱新的 SDK。 

**13. 我可以上傳的場景有多大？**
我們建議您從小規模開始，並留意 Altspace 中沒有怪物電腦的人員。 話雖如此，我們已經有遊戲進入其 maps 以進行即時串流 (例如，射擊的「VR」遊戲) 

![AltspaceVR 中的 VR 遊戲螢幕擷取畫面](images/uploader-faq-img-03.png)

**14. 我必須裝載場景檔案嗎？**
否，Altspace 會在您上傳檔案後提供檔案

**15. 允許陰影嗎？**
Yes

**16. 我可以使用上傳者來快速進行反覆運算嗎？**
如果您已在世界中，您可以在上傳程式中按下傳、重設您的世界，並在最少10秒內查看更新的場景。 通常，您會看到30秒到幾分鐘的迴圈，視場景的複雜度而定。 有個飲料，讓您成為世界 Builder！

**17. 哪裡可以取得3D 模型？**
Sketchfab、Sketchup、Minecraft、Unity 資產存放區等等。

**18. 它是否支援動畫？**

![自訂動畫執行的 GIF](images/uploader-faq-img-04.gif)

**19. 如何設定空間音訊？** 匯入所選的 wav 檔案，在場景中建立空白的遊戲物件，並選取此物件。 將您匯入的音效拖放至物件的偵測器，它就會建立音訊來源。 之後，將音量調整為不超過0.5，將空間 blend 變更為3D，然後調整最小和最大距離以建立適當的音效區域。 根據預設，這會顯示為球體，例如 colliders。 若要取得真正的下降，您必須根據自己的喜好來調整下拉曲線。 [ (via @IsThatToasted) ](https://www.youtube.com/watch?v=ktb2vAAwknw&list=PLGmYIROty-5bpzKQNK3mRMi4pmh_LinV4&t=642s&index=29)

**20. 我要如何看到跨眼尖/奇怪？**
有時，上傳程式無法成功覆寫您的轉譯設定。 [移至編輯 > 專案設定 > Player]。 確定已核取 [支援 > 虛擬實境的 XR 設定] 和 [立體轉譯方法] 是 [單一傳遞] 或 [單一傳遞 (預覽) ]，適用于 PC 和 Android (選取機器人圖示) 。 之後再進行組建 + 上傳，並重設您的世界。 