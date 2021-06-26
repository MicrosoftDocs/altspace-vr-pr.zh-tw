---
title: 將內容更新至最新的 Unity 版本
description: 瞭解如何將內容更新至最新版本的 Unity。
ms.date: 06/4/2021
ms.topic: article
keywords: 套件、世界、unity、更新、著色器、上載器、疑難排解
ms.openlocfilehash: f8a805c4b3350f2c97c43d3d48c35733ec7e9710
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/25/2021
ms.locfileid: "112961206"
---
# <a name="updating-content-to-the-latest-unity-version"></a>將內容更新至最新的 Unity 版本

## <a name="moving-to-unity-202039"></a>移至 Unity 2020.3。9

從今天開始，AltspaceVR 已升級至最新版本的 Unity (2020.3.9) 。 除了一些效能改進之外，這項更新未來也會證明我們有很高興納入的功能。 這種變更應該與所有現有的內容相容。 如果不是，請隨意聯絡支援： altvr.com/support

雖然這移至2020.3.9 並不會影響使用者產生的內容，但在幾周內，我們將變更 AltspaceVR 的身歷聲轉譯模式，以 [要求使用者更新其內容]( https://docs.unity3d.com/Manual/SinglePassStereoRendering.html)。 此升級至 [單一傳遞實例](https://docs.unity3d.com/Manual/SinglePassInstancing.html) 將可大幅改善您的世界效能。 請記住，這個新組建將不再支援與2019.4 及更舊版本的內容回溯相容性。 很緊急地，所有建立者所擁有的內容都會儘快更新，以避免中斷的變更。 遵循下列指南來更新您的內容，並確保能夠順利轉換至 Unity 2020.3.9 上的單一傳遞實例。

> [!NOTE]
> 如果您經常使用其他人所擁有且已與您共用的內容，請洽詢全球/套件擁有者，並確定他們計畫更新其內容。

> 如果您是內容建立者，且有問題或需要協助，請洽詢我們的支援小組以取得協助： altvr.com/support

## <a name="testing-your-spi-content"></a>測試您的 SPI 內容

使用下列預覽版本的 AltspaceVR，以在 VR 中測試新更新的內容。 預覽版本僅供測試之用，不應該用於平臺的一般用途。

* [AltspaceVR Windows Mixed Reality 的 SPI 預覽](https://aka.ms/AvrSpiMr)
* [適用于 SteamVR 的 AltspaceVR SPI 預覽](https://aka.ms/AvrSpiSteam)
* [適用于 Oculus Rift 的 AltspaceVR SPI Preview](https://aka.ms/AvrSpiRift)

> 注意：僅提供電腦 VR 預覽。 Android 上無法使用單一傳遞實例轉譯，而在 Mac 等非 VR 平臺上則不需要。 因此，您可以使用一般發行版本來測試這些裝置。


## <a name="storecompatibilitycheck"></a>存放區相容性檢查

升級至 Unity 2020.3.9 也會影響耳機和商店組建相容性。 現在您需要從與耳機相容的存放區下載 AltspaceVR。 例如：針對 WinMR 或 Oculus 耳機，請分別從 Windows Store 或 Oculus Store 下載 AltspaceVR。 Windows Mixed Reality 使用者應從 Windows 市集中下載 AltspaceVR、從流出 SteamVR 使用者，以及從 Oculus 商店 Oculus Rift 使用者。

## <a name="altspacevr-uploader-v090-upgrade-guide"></a>AltspaceVR 上載者 v 0.9.0 升級指南 

上傳程式0.9 的封裝方式與舊版上載程式不同。 隨著此封裝變更，新的上傳程式需要新版本的 Unity。 本指南的目的是要讓所有相關人員都能更順暢且更安全地進行此升級流程。

1. **備份您的專案** -建立整個專案目錄的複本，並將它放在安全的地方。 這項升級是一種破壞性升級，因此在完成後，您將無法建立或上傳 Unity 2019.4 的組合。 如果您在這項升級期間遇到任何問題，您需要一份全新的專案，才能回復。 您也需要它來更新任何即時套件或範本，再 AltspaceVR 正式升級至 Unity 2020.3.9。

2. **移除舊** 的上傳程式-使用 Unity closed，刪除下列檔案/資料夾，並對應的中繼檔案：

    ```console
    * Assets/Altspace

    * Assets/Plugins

    * Assets/Prefabs/test-folder, Readme.txt

    * Assets/Resources/bg.jpeg, bg2.jpeg, logo.png, UserPreferences.asset

    * Assets/DFloor_v004.fbx

    * Library (This is a Unity system folder, not an Uploader folder. Delete it anyway, and let it be rebuilt during the upgrade.)
    ```

3. **下載引擎版本** -開啟 unity 中樞，並安裝 unity 2020.3.9 (或 [按一下這裡](https://unity3d.com/ru/unity/whats-new/2020.3.9) 直接安裝) 。

4. **升級專案** -在 Unity 2020.3.9 中開啟已清除的專案，並允許 Unity 升級您的專案。

5. 僅 (電腦) **下載混合現實功能工具** -請遵循指示下載「 [混合現實」功能工具](/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool)，此工具將用來管理上載程式套件的安裝。

6. **安裝** 上傳程式-使用 MR 功能工具來選取您的 Unity 專案，並在 AltspaceVR 標題) 下新增 AltspaceVR 上傳程式功能 (。 遵循工具中的指示。

在 macOS 上，從登錄中手動下載最新 [版本，然後](https://dev.azure.com/aipmr/MixedReality-Unity-Packages/_packaging?_a=package&feed=Unity-packages&package=com.microsoft.altspacevr_uploader&protocolType=Npm&version=0.9.0&view=versions)從 Unity 編輯器的套件管理員中安裝它， (Windows > 封裝管理員 > + > 從 Tarball) 新增套件。

封裝完成匯入後，[AltspaceVR] 功能表項目中應該會有熟悉的上傳視窗。

## <a name="troubleshooting-tips"></a>疑難排解秘訣

1. 如果您的 WinMR 耳機有控制器或輸入問題，請確定其位於您的頭部，以適當地與目前狀態感應器互動。 這是已知的問題，Microsoft 正積極努力解決此問題。

2. 檢查您的耳機和商店組建相容性。 例如，如果您使用的是 WinMR 耳機，請確定您的 AltspaceVR 組建是透過 Windows Store 取得的。

3. 如果在測試期間發現您的內容只會以 VR 模式出現在一眼中，則您使用的自訂著色器可能不支援 SPI 轉譯。 您必須選擇不同的著色器，或遵循 [Unity 的 SPI 升級指南](https://docs.unity3d.com/Manual/SinglePassInstancing.html) ，手動編輯著色器並新增支援。

4. 在 WinMR 上，請記住，您必須先執行下列動作，才能在 AltspaceVR 中存取 VR 模式： 
    1. 從 Microsoft Store 下載並安裝 Windows Mixed Reality 的 OpenXR。
        1. 開啟混合實境入口應用程式
        2. 在應用程式左下角，選取 [查看更多]
        3. 在出現的功能表中，選取 [設定 OpenXR]。 這樣做會讓 Windows Store 從您可以安裝執行時間的地方啟動。 如果沒有出現這個功能表項目，OpenXR 可能已安裝在您的電腦上。