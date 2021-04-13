---
title: 上傳自訂 Skyboxes
description: 取得在 AltspaceVR 體驗中上傳自訂 skyboxes 並進行疑難排解的逐步指示。
ms.date: 03/11/2021
ms.topic: article
keywords: skyboxes，疑難排解
ms.openlocfilehash: 02d5bc762dc36d4195100e8155d6250789e833f7
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212436"
---
# <a name="uploading-custom-skyboxes"></a>上傳自訂 Skyboxes

Skybox 可讓您建立世界的 **背景** ，讓體驗更具沉浸。 Skyboxes 有不同的類型，但我們目前支援 **equirectangular**。 以下是使用360攝影機所採用的範例 (更多[範例) ：](http://moments.mankindforward.com/) 

![360 equirectangular 觀賞客廳](images/custom-skyboxes-img-01.jpeg)

您也可以使用 [Unity 上載](world-building-toolkit-getting-started.md) 程式，但這種方法比較簡單。

1. 流覽至 [ [世界] > Skyboxes](https://account.altvr.com/skyboxes) ，然後按右邊的 [ **建立** ] 按鈕

![在 [skyboxes] 面板中開啟的 [世界網站] 頁面](images/custom-skyboxes-img-02.png)

2. 填入名稱並指定您的360影像。 這並不是相片，有些程式可以讓您自行繪製，也可以在線上搜尋。 當您準備好時，選取 [建立]。 

![Skybox 建立表單](images/custom-skyboxes-img-03.png)

3. 您可以選擇上傳 **預覽** 影像，以便輕鬆地識別此 skybox。 您也可以上傳 WAV 格式的環境音訊。 

> [!IMPORTANT]
> 建議您在上傳360影像之後，分別上傳預覽影像和環境音訊。 如果您將它們上傳，檔案大小可能夠大而無法停止處理常式。 [Jetsons World](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) 是如何搭配使用 Skybox 與環境音效的絕佳範例。 請注意，全球 Builder 如何保持音效，而您聽到的音效是偶爾出現的，讓人們不會感到苦惱。 

4. 輸入您的世界，然後開啟 [World 編輯器]。 在 [Skyboxes] 底下，選取新的 Skybox。 幾秒鐘後，天空就會變動。 您世界上的其他人也會看到天空變更。 若要切換回，請選擇相同清單中的 **預設** skybox。 

## <a name="troubleshooting"></a>疑難排解

**天空中有接合線或線：- (。** 這是我們即將修正的 bug

**上傳失敗**
    * 嘗試自行上傳360映射
    * 嘗試使用另一個較小的檔案作為測試

**我找不到360相片**
    * Flickr 是很好的來源 (變更篩選以尋找創意的 commons) 
    * 拿自己！ Ricoh 的攝影機都成功。 
**天空看起來有顆粒狀或 blocky** 您可能需要找到較高解析度的影像。 通常大約 2-5 MB 和 ~ 5000 px x 2000 px

**它會影響我的世界幀率！**
影像可能太大。 某些產生的 skyboxes 可以是8k。 它們通常會隨附適用于 mobile 的2k 版本，請使用該版本。

**使用環境音訊協助我**
    * 使用 >audacity 之類的免費軟體來降低磁片區，或建立您自己的迴圈。 請記住，音訊將會在人們的系統中重複執行並播放，讓它保持低且不討厭
    * [自由音效](https://freesound.org/) 是絕佳的免權利物來源
