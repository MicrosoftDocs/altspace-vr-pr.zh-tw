---
title: Altspace 上載者簡介
description: 瞭解如何使用 Unity 場景範本搭配 Altspace 上傳程式來設定和上傳您的 AltspaceVR 領域。
ms.date: 09/29/2021
ms.author: v-vtieto
ms.topic: article
keywords: 工具組、Altspace、上載者
ms.openlocfilehash: 8d71551fe552159c0078105307802774f44c0d47
ms.sourcegitcommit: 8c58f9f9ad1a3f9534141dee2c78e32792d0db7a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/25/2021
ms.locfileid: "130298787"
---
# <a name="introducing-the-altspace-uploader"></a>Altspace 上載者簡介

> [!NOTE]
> - 如果您有興趣，請加入 [官方 AltspaceVR 但是](https://discordapp.com/invite/altspacevr) ，並造訪 #world 大樓頻道。  
> - 如果您正嘗試恢復舊的空間，請參閱 [升級指南](upgrading-old-unity-projects.md)。 

上載程式可讓您使用 Unity 場景作為您的世界的範本。 您可以從 Minecraft 帶入鬼房子或您最愛的建立。 如果您可以將它匯入 Unity，您可能會以這種方式 Altspace。 以下是一些 [範例領域](https://account.altvr.com/worlds/1046572460192825569)。

![範例世界](images/unity-uploader-img-01.png)

## <a name="setup"></a>安裝程式

1. 加入 [官方 AltspaceVR 但是](https://discordapp.com/invite/altspacevr) ，並造訪 #world 大樓頻道。 朋友不讓朋友單獨建立世界。
2. 閱讀我們的 [世界大樓開始使用指南](world-building-getting-started.md) 以瞭解基本概念
3. [安裝 Unity 中樞](https://unity3d.com/get-unity/download) 和 **unity 2020.3.9**。 除非您完全符合此版本，否則上載者將無法運作。 如果您沒有可用的 Unity 帳戶，您將需要一個帳戶。 在安裝期間，請選擇 [ **個人** 版 (]，因為這樣做很有趣！ ) ，請務必執行下列動作：
    * 包含 **Android 組建支援** 模組。
    * 在 Windows 上，包含 **(Mono) 模組的 Mac 組建支援**。
    * 在 Mac 上，包含 **(Mono) 模組的 Windows 組建支援**。
4. [下載 AltspaceVR 上載者](https://aka.ms/AvrUrpUploader)
5. 在我們的網站上[建立範本](https://account.altvr.com/space_templates/new)。 將它命名 **Hello World 範本**。
6. [建立世界](https://account.altvr.com/worlds/my) 並 **Hello World** 命名。 選取 **Hello World 範本** 作為範本。

![建立的世界畫面](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a>Upload 您的場景

> [!NOTE]
> 您可以在 [這裡](https://buildingthemetaverse.medium.com/how-to-make-your-own-altspace-templates-and-kits-unity-2020-3-9-uploader-2-x-5b40e92bb759)找到更詳細的逐步指南。

1. 開啟 Unity 中樞，並建立新的 Unity 2020.3.9 專案。 針對您的範本，選取 [ **通用轉譯管線**]。

    ![選擇 URP Unity 範本](images/001-unity-templates.png)

1. 流覽至您下載 Altspace 上傳程式的資料夾，然後將它從該資料夾複製或移動到新 Unity 專案的根資料夾。
1. 在 Unity 的功能表列上，選取 [ **Window**  >  **封裝管理員]。**
1. 在封裝管理員的功能表列中，選取加號下拉式清單 ( "+" ) ，然後選取 [**從 tarball 新增套件**]。
1. 流覽至包含 Altspace 上傳程式的資料夾，然後選取 [上傳]，再按一下 [ **開啟**]。  載入封裝之後， **AltspaceVR** 會顯示在功能表列上：

    ![功能表列上的 AltspaceVR](images/002-altspacevr-on-menu-bar.png)

> [!NOTE]
> 您必須將 Altspace 上載套件匯入至您想要搭配 Altspace 使用的每個 Unity 專案。
1. 在功能表列上，選取 [ **AltspaceVR > 範本**]。
1. 在 [ **ALTSPACE VR 範本** ] 對話方塊中，使用您的 Altspace 帳號憑證登入。  (MSA 登入很快就會推出。 如果您只是使用 Microsoft 帳戶登入 Altspace，則必須在網站上使用 [忘記密碼] 選項來建立密碼。 ) 
1. 按一下 [ **選取範本** ] 下拉式清單，然後選取 [ **Hello World 範本**]。
1. 選擇場景：按一下 [**選擇 unity** 檔] 省略號按鈕 (三個點) ，然後流覽至專案中的 [**資產**]  >  **場景** 資料夾，然後選取 [ **SampleScene** ] 並開啟它。
1. 在 [**平臺的組建**] 底下，確認已選取 **Windows** 。 現在，其他兩個選項 [ **Android** ] 和 [ **Mac**] 則 **不** 應選取。 一旦您希望人們造訪，您應該針對所有平臺進行建立和上傳。」
1. 選取 [**組建 &] Upload** 按鈕。 此程式可能需要一或兩分鐘的時間。
1. 啟動 Altspace，然後選取 [ **主功能表**]，然後在功能表列上選取 [ **我的領域**]。
1. 流覽至 **Hello World** 然後開啟它。

    您的場景應該類似于您在 Unity 編輯器中看到的內容。

## <a name="whats-supported"></a>支援的項目

* 是：模型、衝突、動畫、粒子效果、音訊、skyboxes 等等。
* 否：腳本。 基於安全性考慮，包含腳本的上傳將會遭到拒絕。
* 也許：像是動態全球照明的有趣東西。
* 不同平臺的 Upload 場景個別或一起。
* 請參閱 [精選領域](https://account.altvr.com/worlds/featured)。 許多都是使用上傳者所建立。

## <a name="tips"></a>提示

* 加入 [官方 AltspaceVR 但是](https://discordapp.com/invite/altspacevr)。
* 在左側的範本頁面上，我們會顯示依平臺的最新上傳。 如果成功，您會看到 **1-2 分鐘前**。 

![已反白顯示上傳的範本面板開啟](images/template-upload-list.png)

* 當您更新時，可以在世界各地。 當上傳者顯示 **Upload 完成** 時，您可以重設世界以查看變更。
* 使用簡單的場景建立僅限電腦時，應該不到一分鐘的時間，就能在 Altspace 中看到變更。
* 將您的世界設為私用且未列出，以避免分散注意力。
* 將 cube 放置於來源，讓您可以看到人員預設會產生的位置。 上傳時隱藏 cube。

## <a name="troubleshooting"></a>疑難排解

**我正在進行或無法傳送至任何** 您必須將衝突新增至物件，以傳送至這些物件。

**沒有變更**
    * 您是否已將場景儲存在 Unity 中？
    * 您選擇要測試的平臺嗎？
    * 你是在正確的世界嗎？ 您是否在上載者和世界表單中選擇正確的範本？
    * 您是否已檢查範本頁面統計資料？

**Upload 失敗或超時**
    * 最常見的上傳錯誤結果是因為有錯誤的 Unity 版本。 您必須完全符合所需的版本。
    * 您的上傳可能太大。 請嘗試保持電腦幕後 < 100 MB。 從小規模開始，然後建立。 Optimize、optimize、optimize。
    * 請嘗試使用包含簡單 cube 的全新專案。
    * 請勿在組建期間強制結束--它可能會損毀您的場景。 請嘗試重新上傳。

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
