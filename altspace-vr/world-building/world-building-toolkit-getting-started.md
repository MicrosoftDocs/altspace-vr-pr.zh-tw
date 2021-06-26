---
title: 全球建築工具組簡介
description: 瞭解如何使用 Unity 場景範本搭配全球建築工具組來設定和上傳您的 AltspaceVR 世界。
ms.date: 03/11/2021
ms.topic: article
keywords: 工具箱
ms.openlocfilehash: 3b41f02aec1077a37b95a6826c105e1cd31974e3
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923075"
---
# <a name="introducing-the-world-building-toolkit"></a><span data-ttu-id="576bd-104">全球建築工具組簡介</span><span class="sxs-lookup"><span data-stu-id="576bd-104">Introducing the World Building Toolkit</span></span>

> [!NOTE]
> <span data-ttu-id="576bd-105">「世界建築」工具組是由我們很棒的朋友 [Anthony Madden](https://twitter.com/chigamesstudio)所執行的一項社區專案，並提供我們的支援。</span><span class="sxs-lookup"><span data-stu-id="576bd-105">The World Building Toolkit is a community project run by our awesome friend, [Anthony Madden](https://twitter.com/chigamesstudio), with support from us.</span></span> <span data-ttu-id="576bd-106">如果您有興趣，請加入 [官方 AltspaceVR 但是](https://discordapp.com/invite/altspacevr) ，並造訪 #world 大樓頻道。</span><span class="sxs-lookup"><span data-stu-id="576bd-106">If you're interested, please join the [Official AltspaceVR Discord](https://discordapp.com/invite/altspacevr) and visit the #world-building channel.</span></span> <span data-ttu-id="576bd-107">目前有 Mac 試用版 Beta 版， [還有更多詳細資料](https://altvr.com/altspacevr-mac)</span><span class="sxs-lookup"><span data-stu-id="576bd-107">We currently have a Mac Trial Beta right now, [more details](https://altvr.com/altspacevr-mac)</span></span>

<span data-ttu-id="576bd-108">上載程式可讓您使用 Unity 場景作為您的世界的範本。</span><span class="sxs-lookup"><span data-stu-id="576bd-108">The Uploader allows you to use a Unity scene as a Template for your Worlds.</span></span> <span data-ttu-id="576bd-109">您可以從 Minecraft 帶入鬼房子或您最愛的建立。</span><span class="sxs-lookup"><span data-stu-id="576bd-109">You can bring in a haunted house for Halloween or your favorite creation from Minecraft.</span></span> <span data-ttu-id="576bd-110">如果您可以將它匯入 Unity，您可能會以這種方式 Altspace。</span><span class="sxs-lookup"><span data-stu-id="576bd-110">If you can import it into Unity, you can probably get it into Altspace this way.</span></span> <span data-ttu-id="576bd-111">以下是一些 [範例領域](https://account.altvr.com/worlds/1046572460192825569)。</span><span class="sxs-lookup"><span data-stu-id="576bd-111">Here are a few [example Worlds](https://account.altvr.com/worlds/1046572460192825569).</span></span>

![範例世界](images/unity-uploader-img-01.png)

## <a name="setup"></a><span data-ttu-id="576bd-113">安裝程式</span><span class="sxs-lookup"><span data-stu-id="576bd-113">Setup</span></span>

1. <span data-ttu-id="576bd-114">加入 [官方的 AltspaceVR 但是](https://discordapp.com/invite/altspacevr) ，並造訪 #world 大樓頻道-朋友不會讓朋友單獨建立世界。</span><span class="sxs-lookup"><span data-stu-id="576bd-114">Join the [Official AltspaceVR Discord](https://discordapp.com/invite/altspacevr) and visit the #world-building channel - Friends don't let friends build Worlds alone.</span></span>
2. <span data-ttu-id="576bd-115">閱讀我們的 [世界大樓開始使用指南](world-building-getting-started.md) 以瞭解基本概念</span><span class="sxs-lookup"><span data-stu-id="576bd-115">Read our [World-Building Getting Started Guide](world-building-getting-started.md) for the basics</span></span>
3. <span data-ttu-id="576bd-116">[安裝 Unity Hub](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) 並安裝 **unity 2020.3.9**。</span><span class="sxs-lookup"><span data-stu-id="576bd-116">[Install Unity Hub](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) and install **Unity 2020.3.9**.</span></span> <span data-ttu-id="576bd-117">除非您完全符合此版本，否則上載者將無法運作。</span><span class="sxs-lookup"><span data-stu-id="576bd-117">The Uploader won't work unless you match this version exactly.</span></span> <span data-ttu-id="576bd-118">如果您沒有帳戶，您將需要免費的 Unity 帳戶，並選擇 [ **個人** ]，因為這樣做可讓您享受更多樂趣！</span><span class="sxs-lookup"><span data-stu-id="576bd-118">You'll need a free Unity account if you don't have one and choose **Personal** since you're doing this for fun!</span></span> <span data-ttu-id="576bd-119">在安裝期間，請確定勾選 [ **Android 組建** ] 選項，並停用自動更新。</span><span class="sxs-lookup"><span data-stu-id="576bd-119">During the install, make sure you check the **Android Builds** option and disable auto-update.</span></span>
4. [<span data-ttu-id="576bd-120">下載最新的 Unity 上載者</span><span class="sxs-lookup"><span data-stu-id="576bd-120">Download the latest Unity Uploader</span></span>](upgrading-content-to-the-latest-unity.md#altspacevr-uploader-v090-upgrade-guide)
5. <span data-ttu-id="576bd-121">在我們的網站上[建立範本](https://account.altvr.com/space_templates/new)。</span><span class="sxs-lookup"><span data-stu-id="576bd-121">[Create a Template](https://account.altvr.com/space_templates/new) on our website.</span></span> <span data-ttu-id="576bd-122">將它命名 **Hello World 範本**。</span><span class="sxs-lookup"><span data-stu-id="576bd-122">Name it **Hello World Template**.</span></span>
6. <span data-ttu-id="576bd-123">[建立世界](https://account.altvr.com/worlds/my) 並 **Hello World** 命名。</span><span class="sxs-lookup"><span data-stu-id="576bd-123">[Create a World](https://account.altvr.com/worlds/my) and name it **Hello World**.</span></span> <span data-ttu-id="576bd-124">選取 **Hello World 範本** 作為範本。</span><span class="sxs-lookup"><span data-stu-id="576bd-124">Select **Hello World Template** as the Template.</span></span>

![建立的世界畫面](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a><span data-ttu-id="576bd-126">上傳您的場景</span><span class="sxs-lookup"><span data-stu-id="576bd-126">Upload your scene</span></span>

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-a-Template/player]

1. <span data-ttu-id="576bd-127">開啟 Unity 中樞，並建立新的 Unity 2020.3.9 專案。</span><span class="sxs-lookup"><span data-stu-id="576bd-127">Open Unity Hub and create a new Unity 2020.3.9 project.</span></span>
2. <span data-ttu-id="576bd-128">當您的專案開啟時，按兩下您所下載的檔案，以匯入上載程式， (它是 Unity 套件) 。</span><span class="sxs-lookup"><span data-stu-id="576bd-128">With your project open, import the Uploader by double-clicking the file you downloaded (it's a Unity package).</span></span> <span data-ttu-id="576bd-129">您現在應該會看到名為 **AltspaceVR** 的新索引標籤。</span><span class="sxs-lookup"><span data-stu-id="576bd-129">You should now see a new tab called **AltspaceVR**.</span></span> <span data-ttu-id="576bd-130">您必須針對要與 Altspace 搭配使用的每個 Unity 專案匯入套件</span><span class="sxs-lookup"><span data-stu-id="576bd-130">You'll need to import the package for every Unity project you want to use with Altspace</span></span>
3. <span data-ttu-id="576bd-131">開啟 **功能表 > AltspaceVR > 組建設定**</span><span class="sxs-lookup"><span data-stu-id="576bd-131">Open **Menu > AltspaceVR > Build Settings**</span></span>
4. <span data-ttu-id="576bd-132">使用您的 Altspace 帳號憑證登入</span><span class="sxs-lookup"><span data-stu-id="576bd-132">Sign in with your Altspace account credentials</span></span>
5. <span data-ttu-id="576bd-133">選取 [**載入範本**]，然後選取 [ **Hello World 範本**]</span><span class="sxs-lookup"><span data-stu-id="576bd-133">Select **Load Templates** and then select **Hello World Template**</span></span>
6. <span data-ttu-id="576bd-134">將 cube 新增至場景並儲存。</span><span class="sxs-lookup"><span data-stu-id="576bd-134">Add a cube to your scene and save.</span></span>
7. <span data-ttu-id="576bd-135">**要檢查 Windows 的組建嗎？** 然後取消核取 **Android 的組建？**</span><span class="sxs-lookup"><span data-stu-id="576bd-135">Check **Build for Windows?** and uncheck **Build for Android?**</span></span>
8. <span data-ttu-id="576bd-136">選取 [上傳]。</span><span class="sxs-lookup"><span data-stu-id="576bd-136">Select **Upload**.</span></span> <span data-ttu-id="576bd-137">大約一分鐘，您應該會看到 **上傳** 完成。</span><span class="sxs-lookup"><span data-stu-id="576bd-137">In about a minute, you should see **Upload** complete.</span></span>
9. <span data-ttu-id="576bd-138">藉由啟動 Altspace 並從 **功能表 > 世界 > 我的世界** 來加入 **Hello World**</span><span class="sxs-lookup"><span data-stu-id="576bd-138">Join **Hello World** by launching Altspace and entering from **Menu > Worlds > My Worlds**</span></span>
10. <span data-ttu-id="576bd-139">從 **功能表 > 設定 > 適中 > 重設空間** 重設世界</span><span class="sxs-lookup"><span data-stu-id="576bd-139">Reset the World from **Menu > Settings > Moderate > Reset Space**</span></span>
11. <span data-ttu-id="576bd-140">您應該會看到 cube。</span><span class="sxs-lookup"><span data-stu-id="576bd-140">You should see the cube.</span></span> <span data-ttu-id="576bd-141">如果您在上述影片中快速進行，您可以在最少10秒內看到變更。</span><span class="sxs-lookup"><span data-stu-id="576bd-141">If you do it fast like in the video above, you can see changes within as little as 10 seconds.</span></span>

## <a name="whats-supported"></a><span data-ttu-id="576bd-142">支援的項目</span><span class="sxs-lookup"><span data-stu-id="576bd-142">What's supported</span></span>

* <span data-ttu-id="576bd-143">是：模型、衝突、動畫、粒子效果、音訊、skyboxes 等等</span><span class="sxs-lookup"><span data-stu-id="576bd-143">Yes: models, collision, animations, particle effects, audio, skyboxes, and so on</span></span>
* <span data-ttu-id="576bd-144">否：腳本。</span><span class="sxs-lookup"><span data-stu-id="576bd-144">No: scripts.</span></span> <span data-ttu-id="576bd-145">基於安全性考慮，包含腳本的上傳將會遭到拒絕</span><span class="sxs-lookup"><span data-stu-id="576bd-145">For security purposes, uploads containing scripts will be rejected</span></span>
* <span data-ttu-id="576bd-146">也許：動態全球照明這類的有趣事物</span><span class="sxs-lookup"><span data-stu-id="576bd-146">Maybe: fancy stuff like dynamic global illumination</span></span>
* <span data-ttu-id="576bd-147">個別或一起針對不同的平臺上傳場景</span><span class="sxs-lookup"><span data-stu-id="576bd-147">Upload scenes for different platforms separately or together</span></span>
* <span data-ttu-id="576bd-148">查看 [精選領域](https://account.altvr.com/worlds/featured)，許多都是使用上傳者建立的</span><span class="sxs-lookup"><span data-stu-id="576bd-148">See [Featured Worlds](https://account.altvr.com/worlds/featured), many were built using the Uploader</span></span>

## <a name="tips"></a><span data-ttu-id="576bd-149">提示</span><span class="sxs-lookup"><span data-stu-id="576bd-149">Tips</span></span>

* <span data-ttu-id="576bd-150">加入 [官方 AltspaceVR 但是](https://discordapp.com/invite/altspacevr)。</span><span class="sxs-lookup"><span data-stu-id="576bd-150">Join the [Official AltspaceVR Discord](https://discordapp.com/invite/altspacevr).</span></span>
* <span data-ttu-id="576bd-151">在左側的範本頁面上，我們會顯示依平臺的最新上傳。</span><span class="sxs-lookup"><span data-stu-id="576bd-151">On the Template page on the left side, we show you the latest uploads by platform.</span></span> <span data-ttu-id="576bd-152">如果成功，您會看到 **1-2 分鐘前**。Screen_Shot_2019-01-11 _at_1.21.04_AM.png</span><span class="sxs-lookup"><span data-stu-id="576bd-152">If it was successful, you'd see **1-2 mins ago**.Screen_Shot_2019-01-11 _at_1.21.04_AM.png</span></span>

![已反白顯示上傳的範本面板開啟](images/unity-uploader-img-03.png)

* <span data-ttu-id="576bd-154">當您更新時，可以在世界各地。</span><span class="sxs-lookup"><span data-stu-id="576bd-154">You can be in-World when you update.</span></span> <span data-ttu-id="576bd-155">當上傳者顯示 **上傳完成** 時，您可以重設世界以查看變更。</span><span class="sxs-lookup"><span data-stu-id="576bd-155">The moment the Uploader says **Upload Complete** you can reset the World to see the changes.</span></span>
* <span data-ttu-id="576bd-156">使用簡單的場景來建立電腦的功能，應該不到1分鐘的時間，就能在 Altspace 中看到變更</span><span class="sxs-lookup"><span data-stu-id="576bd-156">Building for PC-only with a simple scene should take less than 1 minute to see a change in Altspace</span></span>
* <span data-ttu-id="576bd-157">將您的世界設為私用且未列出，以避免分散注意力。</span><span class="sxs-lookup"><span data-stu-id="576bd-157">Set your World to be Private and Unlisted to avoid distractions.</span></span>
* <span data-ttu-id="576bd-158">將 cube 放置於來源，讓您可以看到人員預設會產生的位置。</span><span class="sxs-lookup"><span data-stu-id="576bd-158">Place a cube at the origin so you can see where people will spawn by default.</span></span> <span data-ttu-id="576bd-159">上傳時隱藏 cube。</span><span class="sxs-lookup"><span data-stu-id="576bd-159">Hide the cube when uploading.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="576bd-160">疑難排解</span><span class="sxs-lookup"><span data-stu-id="576bd-160">Troubleshooting</span></span>

<span data-ttu-id="576bd-161">**我正在進行或無法傳送至任何** 您必須將衝突新增至物件，以傳送至這些物件。</span><span class="sxs-lookup"><span data-stu-id="576bd-161">**I'm falling or can't teleport onto anything** You need to add collision to objects to teleport onto them.</span></span>

<span data-ttu-id="576bd-162">**沒有變更**</span><span class="sxs-lookup"><span data-stu-id="576bd-162">**Nothing changed**</span></span>
    * <span data-ttu-id="576bd-163">您是否已將場景儲存在 Unity 中？</span><span class="sxs-lookup"><span data-stu-id="576bd-163">Did you save the scene in Unity?</span></span>
    * <span data-ttu-id="576bd-164">您選擇要測試的平臺嗎？</span><span class="sxs-lookup"><span data-stu-id="576bd-164">Did you choose the platform you're testing on?</span></span>
    * <span data-ttu-id="576bd-165">你是在正確的世界嗎？</span><span class="sxs-lookup"><span data-stu-id="576bd-165">Are you in the right World?</span></span> <span data-ttu-id="576bd-166">您是否在上載者和世界表單中選擇正確的範本？</span><span class="sxs-lookup"><span data-stu-id="576bd-166">Did you choose the right Template in the Uploader AND in the World form?</span></span>
    * <span data-ttu-id="576bd-167">您是否已檢查範本頁面統計資料？</span><span class="sxs-lookup"><span data-stu-id="576bd-167">Did you check the Template page stats?</span></span>

<span data-ttu-id="576bd-168">**上傳失敗或超時**</span><span class="sxs-lookup"><span data-stu-id="576bd-168">**Upload fails or times out**</span></span>
    * <span data-ttu-id="576bd-169">最常見的上傳錯誤是 Unity 版本錯誤。</span><span class="sxs-lookup"><span data-stu-id="576bd-169">Most common upload error is having the wrong Unity version.</span></span> <span data-ttu-id="576bd-170">它必須完全符合所需的版本。</span><span class="sxs-lookup"><span data-stu-id="576bd-170">It must match the required version exactly.</span></span>
    * <span data-ttu-id="576bd-171">您的上傳可能太大。</span><span class="sxs-lookup"><span data-stu-id="576bd-171">Your upload might be too large.</span></span> <span data-ttu-id="576bd-172">請嘗試保持電腦幕後 < 100 MB。</span><span class="sxs-lookup"><span data-stu-id="576bd-172">Try to keep PC scenes < 100 MB.</span></span> <span data-ttu-id="576bd-173">從小規模開始，然後建立。</span><span class="sxs-lookup"><span data-stu-id="576bd-173">Start small and build up.</span></span> <span data-ttu-id="576bd-174">Optimize、optimize、optimize。</span><span class="sxs-lookup"><span data-stu-id="576bd-174">Optimize, optimize, optimize.</span></span>
    * <span data-ttu-id="576bd-175">使用簡單的 cube 來試用全新的專案。</span><span class="sxs-lookup"><span data-stu-id="576bd-175">Try with a fresh project with a simple cube.</span></span>
    * <span data-ttu-id="576bd-176">請勿在組建期間強制結束--它可能會損毀您的場景。</span><span class="sxs-lookup"><span data-stu-id="576bd-176">Don't force quit during a build--it can corrupt your scene.</span></span> <span data-ttu-id="576bd-177">嘗試將。</span><span class="sxs-lookup"><span data-stu-id="576bd-177">Try reuploading.</span></span>

<span data-ttu-id="576bd-178">**這是緩慢的流程**</span><span class="sxs-lookup"><span data-stu-id="576bd-178">**It's a slow process**</span></span>
    * <span data-ttu-id="576bd-179">建議您在稍後逐一查看和 Android 時，才建立電腦。</span><span class="sxs-lookup"><span data-stu-id="576bd-179">We recommend building for PC only while iterating and for Android later.</span></span>
    * <span data-ttu-id="576bd-180">嘗試移除未使用的檔案。</span><span class="sxs-lookup"><span data-stu-id="576bd-180">Try removing unused files.</span></span> <span data-ttu-id="576bd-181">基於任何原因，Unity 有時候會過度。</span><span class="sxs-lookup"><span data-stu-id="576bd-181">For whatever reason Unity gets overzealous sometimes.</span></span>

<span data-ttu-id="576bd-182">**我無法使用 Altspace 認證登入**</span><span class="sxs-lookup"><span data-stu-id="576bd-182">**I can't sign in with my Altspace credentials**</span></span>
    * <span data-ttu-id="576bd-183">電子郵件會區分大小寫。</span><span class="sxs-lookup"><span data-stu-id="576bd-183">Emails are case-sensitive.</span></span>
    * <span data-ttu-id="576bd-184">以新的專案嘗試。</span><span class="sxs-lookup"><span data-stu-id="576bd-184">Try with a new project.</span></span>
    * <span data-ttu-id="576bd-185">請確定您的 Altspace 帳戶良好。</span><span class="sxs-lookup"><span data-stu-id="576bd-185">Make sure your Altspace account is in good standing.</span></span>

## <a name="see-also"></a><span data-ttu-id="576bd-186">另請參閱</span><span class="sxs-lookup"><span data-stu-id="576bd-186">See also</span></span>

* [<span data-ttu-id="576bd-187">Unity 學習</span><span class="sxs-lookup"><span data-stu-id="576bd-187">Unity Learn</span></span>](https://unity3d.com/learn)
* [<span data-ttu-id="576bd-188">Unity 論壇</span><span class="sxs-lookup"><span data-stu-id="576bd-188">Unity Forums</span></span>](https://forum.unity.com)
