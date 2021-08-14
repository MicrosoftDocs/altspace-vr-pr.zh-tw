---
title: 使用 Web 投影機串流瀏覽器
description: 瞭解如何使用 web 投影機將來自指定瀏覽器的內容串流至 AltspaceVR 體驗。
ms.date: 03/11/2021
ms.topic: article
keywords: web 投影機、串流、瀏覽器
ms.openlocfilehash: 8f25de68ba633e10b9192b85c883de4ba48fd7987ec5d301ebac8443982a1a55
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127297"
---
# <a name="using-the-web-projector-to-stream-a-browser"></a>使用 Web 投影機串流瀏覽器

AltspaceVR Web 投影機是一個強大的媒體共用解決方案，可讓您將指定的瀏覽器索引標籤從桌上型電腦直接串流至 AltspaceVR。 它可用來共用投影片、影片、相片，以及您可以從瀏覽器中開啟的其他任何東西。 * 網頁投影機需要下載瀏覽器延伸模組，而且目前可透過全球編輯器來取得。 以下是完整的功能和使用方式的總覽：

## <a name="requirements"></a>規格需求

1. 您必須使用電腦或 Mac 來串流您的瀏覽器。
2. Edge 瀏覽器目前支援必要的瀏覽器擴充功能。  (我們正在擴充這份清單。 ) 
3. 雖然您可以從 Mac 電腦進行串流，但 AltspaceVR Mac 用戶端還無法使用網頁投影機。
4. 如果您已正確設定所有專案 (使用相同的帳戶登入瀏覽器延伸模組/AltspaceVR，AltspaceVR 中的網頁投影機已連線/廣播) ，而且仍看到綠色畫面，則 WebProjector 需要開啟 TCP 埠443和 UDP 埠範圍20000-20400。

> [!NOTE]
> 這項功能主要是用來串流您所選擇的瀏覽器索引標籤。 如果您嘗試改為串流您的桌面應用程式，Web 投影機將會串流所有電腦音訊 (包括 AltspaceVR) ，而這可能會導致回顯/意見反應。 您必須將 AltspaceVR 靜音，以防止發生此情況。 或者，您也可以在從電腦進行串流時，使用不同的裝置來執行 AltspaceVR。

## <a name="getting-started"></a>開始使用

1. 若要開始，您必須下載並安裝瀏覽器延伸模組，可在 [這裡](https://account.altvr.com/web_projector)找到。
2. 接下來， [在您的 Edge 瀏覽器中側載您的擴充](https://docs.microsoft.com/microsoft-edge/extensions-chromium/getting-started/extension-sideloading)功能。
    * 完成下載後，請移至瀏覽器的 [ **延伸** 模組] 區段。  (在 **設定** 下找到) 
    * 將 .zip 檔案解壓縮。
    * 在 **開發人員模式** 上切換，然後選取 [已 **解壓縮載入**]
    * 選擇您剛剛解壓縮的資料夾。 這是網頁投影機擴充功能。
    * 新增擴充功能之後，您就可以進入 **詳細資料** 來設定您的設定。

## <a name="setting-up-a-shareable-browser"></a>設定可共用的瀏覽器

下載並安裝延伸模組之後，您就可以開始使用！

1. 在您的 Edge 瀏覽器中開啟索引標籤，並流覽至您想要共用的媒體。
2. 設定您的視窗，讓您可以共用。  (注意：整個瀏覽器視窗都會投射在世界中) 
3. 找出新安裝的擴充功能 (在瀏覽器) 中，它會顯示為 URL 列附近的 AltspaceVR 圖示。 選取 [AltspaceVR]。 系統會提示您登入您的帳戶。  ( * 注意：請務必登入您將用來設定網頁投影機的相同帳戶。 ) 
4. 登入後，您應該會看到 [延伸模組] 畫面提供 [ **開始串流** ] 選項。 加以選取。

## <a name="projecting-your-browser-in-world"></a>在世界各地投影您的瀏覽器

1. 一旦您的瀏覽器設定為投射，且您已透過延伸模組開始串流，請開啟 AltspaceVR。
2. 藉由開啟您的世界編輯器 > 基本 > Web 投影機，在您選擇的環境中設定 Web 投影機
3. 一旦放置之後，您就可以使用您的世界編輯器控制項來調整 Web 投影機的大小。  (也會在螢幕上包含指示。 ) 
4. 選取 [**連線**] 按鈕以開始串流處理您的 Edge 瀏覽器。
5. 請記得按一下 [ **廣播** ]，開始與空間中的所有來賓共用。
6. 別忘了 **停止串流。** 您的會話最後會結束，但在那之前，它將會繼續即時投影您的瀏覽器。 當您完成時，最好立即結束您的會話。

![AltspaceVR 世界中的瀏覽器投影](images/web-project-img-01.png)

**影片串流秘訣：** 如果影片口吃、停止串流、將影片品質調整為480p 或360p，然後重新開機您的串流和廣播。 較高的解析度可能會佔用 CPU 並上傳頻寬。

> [!NOTE]
> 目前，網頁投影機頂端的其他控制項按鈕尚未上線。 它們將維持灰色並 unclickable。 這不是錯誤，而是設計 (目前) 。

> [!IMPORTANT]
> 免責聲明：注意：像是 AltspaceVR 中的所有其他功能一樣，Web 投影機的使用方式會受限於我們[的服務條款](../community/terms-of-service.md)和我們的[Community 標準](../community/community-standards.md)。 因此，Web 投影機可能不會用來串流違反任一協定的內容。 這樣做會導致 AltspaceVR 所採取的仲裁動作。 無法保證存取網頁投影機 Open Beta 版，而且只能授與暫時試用版。 Beta 的長度和您參與的長度是 AltspaceVR 小組的判斷。 使用 Web 投影機的搶鮮版（Beta）並不是必要的，而且參與 Beta 版是純粹自願的。 建議參與者提供關於 Web 投影機的意見反應，以協助塑造功能的功能和可用性，因為開發會繼續進行。 Web 投影機的搶鮮版（Beta）可能會有有限的功能，且可能受限於非預期的錯誤。 事先感謝您的參與。
