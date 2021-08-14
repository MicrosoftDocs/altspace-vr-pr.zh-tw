---
title: 匯入 glTF 模型
description: 瞭解如何正確地將 3D glTF 模型匯入您的 AltspaceVR 體驗，並針對任何問題進行疑難排解。
ms.date: 03/11/2021
ms.topic: article
keywords: 模型、glTF、匯入、sketchfab、疑難排解
ms.openlocfilehash: 527c38fc49028258fa432445fe14a355710a18be65ee74252a8c39bc1bfe5190
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127033"
---
# <a name="importing-gltf-models"></a>匯入 glTF 模型

> [!NOTE]
> 這項功能目前可用於早期存取程式中的選取使用者。

將3D 模型和場景帶入 Altspace 的其中一種方式是使用 [glTF 標準](https://en.wikipedia.org/wiki/GlTF)。 您可以 (封裝的 glTF) 上傳 glb 檔案，以建立您稍後可以在世界編輯器中產生的模型。 這是 [上傳您自己的套件](uploading-custom-kits.md)的替代方案。 建議您建立快速示範的模型，因為您不需要使用 Unity 和套件來充分發揮效能和重複使用性。 

1. 尋找一些 glTF 3D 資產。 要搜尋的其中一個位置是 Sketchfab (嘗試篩選) [這](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models)類 **可下載** 的模型。 找到之後，請選取 [ **下載3D 模型**：

![Sketchfab 的3D 狗模型](images/importing-models-img-01.png)

2. 將連結複製到模型，並閱讀授權需求。 
3. 下載 **Autoconverted 格式 (glTF)** 版本

![已反白顯示自動轉換格式的 Sketchfab 下載選項](images/importing-models-img-02.png)

4. 開啟 [GLB Packer](https://glb-packer.glitch.me)網站，並核取 [**將 PNG 轉換成 JPEG (Beta 版**] 核取方塊) 
5. 將您下載的 glTF 檔案解壓縮，並將它們一次全部拖曳至 [GLB Packer 瀏覽器] 索引標籤

![顯示模型解壓縮的視窗](images/importing-models-img-03.png)

6. 視檔案的數目和大小而定，可能需要一段時間才能處理。 處理完成時，將會下載 **glb** 檔案。 將該檔案重新命名為有資訊的內容--這會是世界中物件的名稱 (例如 **低 Poly Wolf. glb**) 
7. 流覽至 [altvr.com > 更 > 的模型](https://account.altvr.com/users/sign_in)，然後選取 [**建立**]
8. 請指定 glb 檔案的位置，並確定您將 Sketchfab 連結複製到屬性的描述中。 您可以視需要指定預覽影像，然後選取 [ **建立模型**：

![AltspaceVR 中的模型預覽](images/importing-models-img-04.png)

9. 選取 [**複製到剪貼** 簿]
10. 開啟 **全球編輯器 > Altspace > 基本 > GLTF**
11. 貼上您的 url，然後選取 [**確認**]

恭喜！ 您只是產生第一個模型。

## <a name="troubleshooting"></a>疑難排解

**當我按一下 [ **確認** ] 時沒有任何事**
    * 我們目前有10萬個多邊形的限制。 如果失敗，請刪除物件，以避免使用者加入您的世界時可能發生的問題
    * 資產可能有其他問題。 請盡可能使用最少多邊形的資產。
    * 您所帶入的模型可能很小或很大。 請嘗試增加/減少比例，或四處移動您的頭像，您可能會在模型內

**載入速度很慢** 世界上的其他使用者可以快載入的速度，取決於其連線速度。 它也不會像套件資產一樣快取。 如果您將其中一個放在家裡，每次加入時，最後會 redownloading 相同的模型，這並不重要。

沒有 **衝突** 依預設，不會發生這種情況下的物件衝突

**當我產生它時，我在六個 DOF 或我的控制項中失去了控制項，因此難以操作** 是的，我們知道這些問題，希望儘快解決這些問題。  