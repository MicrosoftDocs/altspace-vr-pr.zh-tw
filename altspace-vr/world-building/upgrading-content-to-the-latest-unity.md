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
# <a name="updating-content-to-the-latest-unity-version"></a><span data-ttu-id="30b13-104">將內容更新至最新的 Unity 版本</span><span class="sxs-lookup"><span data-stu-id="30b13-104">Updating Content to the Latest Unity Version</span></span>

## <a name="moving-to-unity-202039"></a><span data-ttu-id="30b13-105">移至 Unity 2020.3。9</span><span class="sxs-lookup"><span data-stu-id="30b13-105">Moving to Unity 2020.3.9</span></span>

<span data-ttu-id="30b13-106">從今天開始，AltspaceVR 已升級至最新版本的 Unity (2020.3.9) 。</span><span class="sxs-lookup"><span data-stu-id="30b13-106">Starting today, AltspaceVR has upgraded to a recent version of Unity (2020.3.9).</span></span> <span data-ttu-id="30b13-107">除了一些效能改進之外，這項更新未來也會證明我們有很高興納入的功能。</span><span class="sxs-lookup"><span data-stu-id="30b13-107">In addition to some performance improvements, this update future-proofs us for forthcoming features that we're excited to incorporate.</span></span> <span data-ttu-id="30b13-108">這種變更應該與所有現有的內容相容。</span><span class="sxs-lookup"><span data-stu-id="30b13-108">This change should be compatible with all existing content.</span></span> <span data-ttu-id="30b13-109">如果不是，請隨意聯絡支援： altvr.com/support</span><span class="sxs-lookup"><span data-stu-id="30b13-109">If it isn't, feel free to contact support: altvr.com/support</span></span>

<span data-ttu-id="30b13-110">雖然這移至2020.3.9 並不會影響使用者產生的內容，但在幾周內，我們將變更 AltspaceVR 的身歷聲轉譯模式，以 [要求使用者更新其內容]( https://docs.unity3d.com/Manual/SinglePassStereoRendering.html)。</span><span class="sxs-lookup"><span data-stu-id="30b13-110">Though this move to 2020.3.9 hasn't affected user-generated content, in a few weeks we're making a change to AltspaceVR's [stereo rendering mode that will require users to update their content]( https://docs.unity3d.com/Manual/SinglePassStereoRendering.html).</span></span> <span data-ttu-id="30b13-111">此升級至 [單一傳遞實例](https://docs.unity3d.com/Manual/SinglePassInstancing.html) 將可大幅改善您的世界效能。</span><span class="sxs-lookup"><span data-stu-id="30b13-111">This upgrade to [Single Pass Instancing](https://docs.unity3d.com/Manual/SinglePassInstancing.html) will allow for significant performance improvements in your worlds.</span></span> <span data-ttu-id="30b13-112">請記住，這個新組建將不再支援與2019.4 及更舊版本的內容回溯相容性。</span><span class="sxs-lookup"><span data-stu-id="30b13-112">Keep in mind that this new build will no longer support backwards-compatibility with content from 2019.4 and older.</span></span> <span data-ttu-id="30b13-113">很緊急地，所有建立者所擁有的內容都會儘快更新，以避免中斷的變更。</span><span class="sxs-lookup"><span data-stu-id="30b13-113">It's urgent that all creator-owned content is updated as soon as possible to avoid breaking changes.</span></span> <span data-ttu-id="30b13-114">遵循下列指南來更新您的內容，並確保能夠順利轉換至 Unity 2020.3.9 上的單一傳遞實例。</span><span class="sxs-lookup"><span data-stu-id="30b13-114">Follow the guide below to update your content and ensure a smooth transition to Single Pass Instancing on Unity 2020.3.9.</span></span>

> [!NOTE]
> <span data-ttu-id="30b13-115">如果您經常使用其他人所擁有且已與您共用的內容，請洽詢全球/套件擁有者，並確定他們計畫更新其內容。</span><span class="sxs-lookup"><span data-stu-id="30b13-115">If you are regularly using content that is owned by someone else and has been shared with you, contact the world/kit owner and make sure they are planning to update their content.</span></span>

> <span data-ttu-id="30b13-116">如果您是內容建立者，且有問題或需要協助，請洽詢我們的支援小組以取得協助： altvr.com/support</span><span class="sxs-lookup"><span data-stu-id="30b13-116">If you are a content creator and you have questions or require assistance, please contact our support team for help: altvr.com/support</span></span>

## <a name="testing-your-spi-content"></a><span data-ttu-id="30b13-117">測試您的 SPI 內容</span><span class="sxs-lookup"><span data-stu-id="30b13-117">Testing your SPI content</span></span>

<span data-ttu-id="30b13-118">使用下列預覽版本的 AltspaceVR，以在 VR 中測試新更新的內容。</span><span class="sxs-lookup"><span data-stu-id="30b13-118">Use the following preview versions of AltspaceVR to test your newly updated content in VR.</span></span> <span data-ttu-id="30b13-119">預覽版本僅供測試之用，不應該用於平臺的一般用途。</span><span class="sxs-lookup"><span data-stu-id="30b13-119">The preview versions are for testing purposes only, and shouldn't be used for a general use of the platform.</span></span>

* [<span data-ttu-id="30b13-120">AltspaceVR Windows Mixed Reality 的 SPI 預覽</span><span class="sxs-lookup"><span data-stu-id="30b13-120">AltspaceVR SPI Preview for Windows Mixed Reality</span></span>](https://aka.ms/AvrSpiMr)
* [<span data-ttu-id="30b13-121">適用于 SteamVR 的 AltspaceVR SPI 預覽</span><span class="sxs-lookup"><span data-stu-id="30b13-121">AltspaceVR SPI Preview for SteamVR</span></span>](https://aka.ms/AvrSpiSteam)
* [<span data-ttu-id="30b13-122">適用于 Oculus Rift 的 AltspaceVR SPI Preview</span><span class="sxs-lookup"><span data-stu-id="30b13-122">AltspaceVR SPI Preview for Oculus Rift</span></span>](https://aka.ms/AvrSpiRift)

> <span data-ttu-id="30b13-123">注意：僅提供電腦 VR 預覽。</span><span class="sxs-lookup"><span data-stu-id="30b13-123">Note: Only PC VR previews have been provided.</span></span> <span data-ttu-id="30b13-124">Android 上無法使用單一傳遞實例轉譯，而在 Mac 等非 VR 平臺上則不需要。</span><span class="sxs-lookup"><span data-stu-id="30b13-124">Single pass instanced rendering is not available on Android, and is not needed on non-VR platforms like Mac.</span></span> <span data-ttu-id="30b13-125">因此，您可以使用一般發行版本來測試這些裝置。</span><span class="sxs-lookup"><span data-stu-id="30b13-125">Thus, you can use the general release version to test these devices.</span></span>


## <a name="storecompatibilitycheck"></a><span data-ttu-id="30b13-126">存放區相容性檢查</span><span class="sxs-lookup"><span data-stu-id="30b13-126">Store Compatibility Check</span></span>

<span data-ttu-id="30b13-127">升級至 Unity 2020.3.9 也會影響耳機和商店組建相容性。</span><span class="sxs-lookup"><span data-stu-id="30b13-127">The upgrade to Unity 2020.3.9 will also affect headset and store-build compatibility.</span></span> <span data-ttu-id="30b13-128">現在您需要從與耳機相容的存放區下載 AltspaceVR。</span><span class="sxs-lookup"><span data-stu-id="30b13-128">It's now a requirement that you download AltspaceVR from the store that is compatible with your headset.</span></span> <span data-ttu-id="30b13-129">例如：針對 WinMR 或 Oculus 耳機，請分別從 Windows Store 或 Oculus Store 下載 AltspaceVR。</span><span class="sxs-lookup"><span data-stu-id="30b13-129">As an example: For a WinMR or Oculus headset, download AltspaceVR from the Windows Store or Oculus Store, respectively.</span></span> <span data-ttu-id="30b13-130">Windows Mixed Reality 使用者應從 Windows 市集中下載 AltspaceVR、從流出 SteamVR 使用者，以及從 Oculus 商店 Oculus Rift 使用者。</span><span class="sxs-lookup"><span data-stu-id="30b13-130">Windows Mixed Reality users should download AltspaceVR from the Windows Store, SteamVR users from Steam, and Oculus Rift users from the Oculus Store.</span></span>

## <a name="altspacevr-uploader-v090-upgrade-guide"></a><span data-ttu-id="30b13-131">AltspaceVR 上載者 v 0.9.0 升級指南</span><span class="sxs-lookup"><span data-stu-id="30b13-131">AltspaceVR Uploader v0.9.0 Upgrade Guide</span></span> 

<span data-ttu-id="30b13-132">上傳程式0.9 的封裝方式與舊版上載程式不同。</span><span class="sxs-lookup"><span data-stu-id="30b13-132">Uploader 0.9 is packaged differently than previous versions of the Uploader.</span></span> <span data-ttu-id="30b13-133">隨著此封裝變更，新的上傳程式需要新版本的 Unity。</span><span class="sxs-lookup"><span data-stu-id="30b13-133">Simultaneous with this packaging change, the new Uploader requires a new version of Unity.</span></span> <span data-ttu-id="30b13-134">本指南的目的是要讓所有相關人員都能更順暢且更安全地進行此升級流程。</span><span class="sxs-lookup"><span data-stu-id="30b13-134">This guide is intended to make this upgrade process smoother and safer for all who are involved.</span></span>

1. <span data-ttu-id="30b13-135">**備份您的專案** -建立整個專案目錄的複本，並將它放在安全的地方。</span><span class="sxs-lookup"><span data-stu-id="30b13-135">**BACK UP YOUR PROJECT** - Create a copy of your entire project directory, and put it somewhere safe.</span></span> <span data-ttu-id="30b13-136">這項升級是一種破壞性升級，因此在完成後，您將無法建立或上傳 Unity 2019.4 的組合。</span><span class="sxs-lookup"><span data-stu-id="30b13-136">This upgrade is a destructive upgrade, so you won't be able to create or upload bundles for Unity 2019.4 after you complete it.</span></span> <span data-ttu-id="30b13-137">如果您在這項升級期間遇到任何問題，您需要一份全新的專案，才能回復。</span><span class="sxs-lookup"><span data-stu-id="30b13-137">If you come across any problems during this upgrade, you'll NEED a clean copy of your project to fall back on.</span></span> <span data-ttu-id="30b13-138">您也需要它來更新任何即時套件或範本，再 AltspaceVR 正式升級至 Unity 2020.3.9。</span><span class="sxs-lookup"><span data-stu-id="30b13-138">You'll also need it to update any live kits or templates before AltspaceVR officially upgrades to Unity 2020.3.9.</span></span>

2. <span data-ttu-id="30b13-139">**移除舊** 的上傳程式-使用 Unity closed，刪除下列檔案/資料夾，並對應的中繼檔案：</span><span class="sxs-lookup"><span data-stu-id="30b13-139">**REMOVE OLD UPLOADER** - With Unity closed, delete the following files/folders, and it's corresponding .meta files:</span></span>

    ```console
    * Assets/Altspace

    * Assets/Plugins

    * Assets/Prefabs/test-folder, Readme.txt

    * Assets/Resources/bg.jpeg, bg2.jpeg, logo.png, UserPreferences.asset

    * Assets/DFloor_v004.fbx

    * Library (This is a Unity system folder, not an Uploader folder. Delete it anyway, and let it be rebuilt during the upgrade.)
    ```

3. <span data-ttu-id="30b13-140">**下載引擎版本** -開啟 unity 中樞，並安裝 unity 2020.3.9 (或 [按一下這裡](https://unity3d.com/ru/unity/whats-new/2020.3.9) 直接安裝) 。</span><span class="sxs-lookup"><span data-stu-id="30b13-140">**DOWNLOAD ENGINE VERSION** - Open the Unity Hub, and install Unity 2020.3.9 (or [click here](https://unity3d.com/ru/unity/whats-new/2020.3.9) to install directly).</span></span>

4. <span data-ttu-id="30b13-141">**升級專案** -在 Unity 2020.3.9 中開啟已清除的專案，並允許 Unity 升級您的專案。</span><span class="sxs-lookup"><span data-stu-id="30b13-141">**UPGRADE PROJECT** - Open your cleaned project in Unity 2020.3.9, and allow Unity to upgrade your project.</span></span>

5. <span data-ttu-id="30b13-142">僅 (電腦) **下載混合現實功能工具** -請遵循指示下載「 [混合現實」功能工具](/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool)，此工具將用來管理上載程式套件的安裝。</span><span class="sxs-lookup"><span data-stu-id="30b13-142">(PC Only) **DOWNLOAD MIXED REALITY FEATURE TOOL** - Follow the instructions to download the [Mixed Reality Feature Tool](/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool), which you'll use to manage the installation of the Uploader package.</span></span>

6. <span data-ttu-id="30b13-143">**安裝** 上傳程式-使用 MR 功能工具來選取您的 Unity 專案，並在 AltspaceVR 標題) 下新增 AltspaceVR 上傳程式功能 (。</span><span class="sxs-lookup"><span data-stu-id="30b13-143">**INSTALL THE UPLOADER** - Use the MR Feature Tool to select your Unity project, and add the AltspaceVR Uploader feature (under the AltspaceVR heading).</span></span> <span data-ttu-id="30b13-144">遵循工具中的指示。</span><span class="sxs-lookup"><span data-stu-id="30b13-144">Follow the instructions in the tool.</span></span>

<span data-ttu-id="30b13-145">在 macOS 上，從登錄中手動下載最新 [版本，然後](https://dev.azure.com/aipmr/MixedReality-Unity-Packages/_packaging?_a=package&feed=Unity-packages&package=com.microsoft.altspacevr_uploader&protocolType=Npm&version=0.9.0&view=versions)從 Unity 編輯器的套件管理員中安裝它， (Windows > 封裝管理員 > + > 從 Tarball) 新增套件。</span><span class="sxs-lookup"><span data-stu-id="30b13-145">On macOS, manually download the latest version from the [registry](https://dev.azure.com/aipmr/MixedReality-Unity-Packages/_packaging?_a=package&feed=Unity-packages&package=com.microsoft.altspacevr_uploader&protocolType=Npm&version=0.9.0&view=versions), and install it from within the Unity Editor's package manager (Windows > Package Manager > + > Add package from tarball).</span></span>

<span data-ttu-id="30b13-146">封裝完成匯入後，[AltspaceVR] 功能表項目中應該會有熟悉的上傳視窗。</span><span class="sxs-lookup"><span data-stu-id="30b13-146">Once the package finishes importing, the familiar Uploader window should be available in the AltspaceVR menu item.</span></span>

## <a name="troubleshooting-tips"></a><span data-ttu-id="30b13-147">疑難排解秘訣</span><span class="sxs-lookup"><span data-stu-id="30b13-147">Troubleshooting Tips</span></span>

1. <span data-ttu-id="30b13-148">如果您的 WinMR 耳機有控制器或輸入問題，請確定其位於您的頭部，以適當地與目前狀態感應器互動。</span><span class="sxs-lookup"><span data-stu-id="30b13-148">If you're having controller or input issues on your WinMR headset, ensure it's positioned on your head to properly engage the presence sensor.</span></span> <span data-ttu-id="30b13-149">這是已知的問題，Microsoft 正積極努力解決此問題。</span><span class="sxs-lookup"><span data-stu-id="30b13-149">This is a known issue and Microsoft is actively working to resolve it.</span></span>

2. <span data-ttu-id="30b13-150">檢查您的耳機和商店組建相容性。</span><span class="sxs-lookup"><span data-stu-id="30b13-150">Check your headset and store-build compatibility.</span></span> <span data-ttu-id="30b13-151">例如，如果您使用的是 WinMR 耳機，請確定您的 AltspaceVR 組建是透過 Windows Store 取得的。</span><span class="sxs-lookup"><span data-stu-id="30b13-151">If you're using a WinMR headset, for example, make sure that your AltspaceVR build was acquired through the Windows Store.</span></span>

3. <span data-ttu-id="30b13-152">如果在測試期間發現您的內容只會以 VR 模式出現在一眼中，則您使用的自訂著色器可能不支援 SPI 轉譯。</span><span class="sxs-lookup"><span data-stu-id="30b13-152">If during testing you discover that your content only appears in one eye in VR mode, it is likely that the custom shaders you use do not support SPI rendering.</span></span> <span data-ttu-id="30b13-153">您必須選擇不同的著色器，或遵循 [Unity 的 SPI 升級指南](https://docs.unity3d.com/Manual/SinglePassInstancing.html) ，手動編輯著色器並新增支援。</span><span class="sxs-lookup"><span data-stu-id="30b13-153">You’ll need to choose a different shader, or follow [Unity’s SPI upgrade guide](https://docs.unity3d.com/Manual/SinglePassInstancing.html) to manually edit the shader and add support.</span></span>

4. <span data-ttu-id="30b13-154">在 WinMR 上，請記住，您必須先執行下列動作，才能在 AltspaceVR 中存取 VR 模式：</span><span class="sxs-lookup"><span data-stu-id="30b13-154">For those on WinMR, please remember that before you can access VR mode in AltspaceVR, you must:</span></span> 
    1. <span data-ttu-id="30b13-155">從 Microsoft Store 下載並安裝 Windows Mixed Reality 的 OpenXR。</span><span class="sxs-lookup"><span data-stu-id="30b13-155">Download and install OpenXR for Windows Mixed Reality from the Microsoft Store.</span></span>
        1. <span data-ttu-id="30b13-156">開啟混合實境入口應用程式</span><span class="sxs-lookup"><span data-stu-id="30b13-156">Open the Mixed Reality Portal app</span></span>
        2. <span data-ttu-id="30b13-157">在應用程式左下角，選取 [查看更多]</span><span class="sxs-lookup"><span data-stu-id="30b13-157">On the lower-left corner of the app select "See More"</span></span>
        3. <span data-ttu-id="30b13-158">在出現的功能表中，選取 [設定 OpenXR]。</span><span class="sxs-lookup"><span data-stu-id="30b13-158">In the menu that appears select Set Up OpenXR.</span></span> <span data-ttu-id="30b13-159">這樣做會讓 Windows Store 從您可以安裝執行時間的地方啟動。</span><span class="sxs-lookup"><span data-stu-id="30b13-159">Doing this will cause the Windows Store to launch from where you can install the runtime.</span></span> <span data-ttu-id="30b13-160">如果沒有出現這個功能表項目，OpenXR 可能已安裝在您的電腦上。</span><span class="sxs-lookup"><span data-stu-id="30b13-160">If this menu item does not appear, OpenXR may already be installed on your PC.</span></span>