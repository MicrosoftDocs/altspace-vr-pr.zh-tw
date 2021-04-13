---
title: 上傳自訂套件
description: 瞭解如何在 AltspaceVR 中設定、產生及上傳您自己的自訂套件，以及疑難排解說明。
ms.date: 03/11/2021
ms.topic: article
keywords: 套件、上傳、疑難排解
ms.openlocfilehash: e5a1b9c2ef5339db0cb821cb6f7d21a930416451
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212553"
---
# <a name="uploading-custom-kits"></a>上傳自訂套件

「世界編輯器」包含可在您的世界中產生的成品套件。 例如， [Campfire 套件](https://account.altvr.com/kits/993516233267609824) 有許多類型的樹狀結構，每種類型的樹狀結構都是成品。 若要建立您自己的套件，您必須建立 Unity AssetBundles 並上傳包含每個成品 Unity 預製專案的 .zip 檔案，並在我們的網站上註冊每個成品。 幸運的是，社區驅動的 Unity 上傳程式會將大部分的工作流程自動化。 上傳之後，您可以從您自己的套件產生物件，讓其他使用者可以自動看見它們。 稍後，您可以與您的朋友分享您的套件，也可以透過精選來與整個社區分享。

## <a name="prerequisites"></a>必要條件

1. [安裝 Unity 中樞和 Unity](world-building-toolkit-getting-started.md)
2. 下載最新版本的[Unity 上載](https://altvr.com/download-latest-unity-uploader/)程式

## <a name="setup"></a>設定 

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-1-Setup/player]

1. 在我們的全球網站上建立套件 [> 套件](https://account.altvr.com/kits)
2. 從瀏覽器的網址列將套件識別碼複製到剪貼簿 (此步驟會在上傳版 0.9 + 中更簡單) 
3. 建立新的 Unity 專案
4. 按兩下套件以匯入 Unity 上載程式

![匯入 unity 上載套件](images/custom-kits-img-01.png)

5. 使用您的 Altspace 電子郵件和密碼登入上載程式

![Unity 中的 AltspaceVR 登入介面](images/custom-kits-img-02.png)

## <a name="generate-and-upload-your-kit"></a>產生並上傳您的套件

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-2/player]

1. 以套件識別碼填入套件 **資料夾名稱** 作為前置詞和主題 (例如 **1137484494681408069_Pirates**) ，並以套件識別碼填入 **套件資產名稱** 作為前置詞。 所有資產都必須有這個前置詞。

![Unity 中具有套件資料夾名稱的 AltspaceVR 介面](images/custom-kits-img-03.png)

2. 針對每個成品或一組構件：
* 將您的來源預製專案 (s) 拖曳至 [階層] 索引標籤
* 選取您要包含在集合中的專案，例如五種類型的桶
* 使用 **圓柱** 更新 **套件資產名稱**
* Select **將 GameObject (s) 轉換為套件預製專案**
* 確認已在資產/Prefabs 資料夾中建立新的 Prefabs 和螢幕擷取畫面

![已選取成品的 Unity 中的 AltspaceVR 介面](images/custom-kits-img-04.png)

> [!NOTE]
> 如果您想要對產生的預製專案進行任何修改，請將其拖曳回階層中，進行變更， **然後按一下 [** 檢查] 索引標籤中的 [套用] 來更新預製專案。 

3. 當您準備好時，請向下 [上傳] 索引標籤，讓我們準備產生具有資產套件組合的 zip 檔案
4. 若要更快速地進行反復專案，請取消核取 **Android 的組建套件？**。 請記得在您完成反覆運算或想要與套件共用/功能時，建立並上傳 Android 版。 
5. 選取 **載入套件預製專案目錄**
6. 選擇符合套件資料夾名稱的 [ **組建** ]。 通常會從相同的 Unity 專案產生多個套件。 這可能需要一些時間，視您的套件大小而定。 完成時，包含 zip 檔案的資料夾將會自動開啟。 
7. 移至網站，編輯您稍早建立的套件，然後上傳您所產生的 zip 檔案。 視檔案大小而定，此上傳可能需要一段時間。
    * 如果成功，您會在左側的「上傳」檔案大小、電腦和 Android，以及上次更新時間
    * 如果不成功，請確定您沒有任何腳本，我們不支援腳本，我們會檢查這些腳本是否有安全性，然後再試一次。

恭喜！ 您已經準備好使用自己的套件建立世界！

## <a name="troubleshooting"></a>疑難排解 

**有任何限制嗎？**
但不會有任何硬性限制，但請記住，即使只有一個成品，使用者仍需要針對整個套件下載其平臺的 AssetBundle。 請嘗試將每個平臺的下載保持在 5 MB 以下。 其中一種方法是將專案分割成較小的套件。 例如，200 .props 應該以半個分割。 

**看到「分割眼睛」？**
重新匯入最新的上載者以取得正確的轉譯設定

**更新/變更未反映？**
    * 查看套件頁面上的更新時間
    * 重新進入世界將無法運作--重新開機用戶端。 甚至可能需要幾分鐘的時間才會更新
    * 請確定您的資料夾名稱或預製專案名稱中沒有空格 **，例如「party_favors」與**「合作物件喜好」

**它會持續說我有腳本，但是我不** 會AssetBundle 瀏覽器有時會自動包含檔案。 請嘗試隔離您所攜帶的模型。 例如，不要將它拖曳到另一個預製專案的一部分。

**物件和動畫的意義為何？**
在這些情況下，會在 1x1x1 Cube 下放置，並停用網格轉譯和碰撞。 物件應已啟用迴圈，並應將 **縮放比例** 設定 **為階層，以便** 我們可以在 Altspace 中適當地進行調整。 在產生所有動畫的 prefabs 之後，請針對每個動畫停用 **衝突** 物件的衝突。

**構件很暗** 您是否將模型的材質著色器設定為 **僅限行動/頂點的方向燈**？

成品 **未面對正確的方式** 旋轉 **模型** 和 **碰撞**，並更新預製專案。 旋轉父系不會進行任何動作，而是會忽略該動作。 您可以使用 [ **旋轉覆寫** ] 欄位來輕鬆執行此動作。

**這些成品可以搭配 SDK 的 **CreateFromLibrary** 函式使用嗎？**
是