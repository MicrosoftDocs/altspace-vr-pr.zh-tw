---
title: 使用多媒體主控台
description: 瞭解如何在 AltspaceVR 體驗中開始設定、發佈和控制多媒體主控台。
ms.date: 03/11/2021
ms.topic: article
keywords: 主控台，多媒體
ms.openlocfilehash: 601328eb6f266dbcfc9d81fc4f1c2d09ac62b318
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212237"
---
# <a name="using-the-multimedia-console"></a><span data-ttu-id="1be14-104">使用多媒體主控台</span><span class="sxs-lookup"><span data-stu-id="1be14-104">Using the multimedia console</span></span>

<span data-ttu-id="1be14-105">多媒體主控台是一種工具，可讓您在事件和世界中共用媒體。</span><span class="sxs-lookup"><span data-stu-id="1be14-105">The Multimedia Console is a tool that enables media sharing in events and worlds.</span></span> <span data-ttu-id="1be14-106">您可以使用它來共用影像、簡報、投影片、livestreams、影片、播放清單等專案。</span><span class="sxs-lookup"><span data-stu-id="1be14-106">You can use it to share things like images, presentation slides, livestreams, videos, playlists, and more.</span></span> <span data-ttu-id="1be14-107">以下逐步指示說明如何使用多媒體主控台 **v 0.5.0 +**。</span><span class="sxs-lookup"><span data-stu-id="1be14-107">Below is a step-by-step instruction on how to use the Multimedia Console **v0.5.0+**.</span></span> 

## <a name="getting-started"></a><span data-ttu-id="1be14-108">開始使用</span><span class="sxs-lookup"><span data-stu-id="1be14-108">Getting started</span></span>

<span data-ttu-id="1be14-109">開始使用多媒體主控台的程式分為兩個部分。</span><span class="sxs-lookup"><span data-stu-id="1be14-109">Getting started with the Multimedia Console is a two part process.</span></span>  <span data-ttu-id="1be14-110">首先，您將使用入口網站來產生和發佈您在環境中放置之多媒體主控台會話的設定。</span><span class="sxs-lookup"><span data-stu-id="1be14-110">First there's the web portal that you'll use to generate and publish a configuration for the Multimedia Console session you place in your environment.</span></span>  <span data-ttu-id="1be14-111">第二個是在您的環境中放置實際的多媒體主控台應用程式，並設定應該使用的設定程式碼。</span><span class="sxs-lookup"><span data-stu-id="1be14-111">Second is the placement of the actual Multimedia Console app in your environment and setting the configuration code it should use.</span></span>

### <a name="configuring-the-multimedia-console-with-the-web-portal"></a><span data-ttu-id="1be14-112">使用入口網站設定多媒體主控台</span><span class="sxs-lookup"><span data-stu-id="1be14-112">Configuring the Multimedia console with the web portal</span></span>

1. <span data-ttu-id="1be14-113">首先，您必須確定您的內容會在線上裝載，因為您將需要 URL。</span><span class="sxs-lookup"><span data-stu-id="1be14-113">First, you'll need to make sure your content is hosted online because you'll need a URL.</span></span> <span data-ttu-id="1be14-114"> (您可以將相片上傳至 altvr.com、線上裝載影片，或使用 Twitch 即時串流連結： https://www.twitch.tv/ninja)</span><span class="sxs-lookup"><span data-stu-id="1be14-114">(You can upload photos to altvr.com, host a video .mp4 file online or use Twitch live stream link: https://www.twitch.tv/ninja)</span></span> 
2. <span data-ttu-id="1be14-115">流覽至多媒體主控台的入口網站，網址為： [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)</span><span class="sxs-lookup"><span data-stu-id="1be14-115">Navigate to the web portal for the Multimedia Console at [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)</span></span>
3. <span data-ttu-id="1be14-116">您可以從入口網站產生和發佈多媒體主控台的設定。</span><span class="sxs-lookup"><span data-stu-id="1be14-116">From the web portal, you can generate and publish a configuration for the Multimedia Console.</span></span>  <span data-ttu-id="1be14-117"> (請參閱下文，以取得各種屬性) 的詳細資料。</span><span class="sxs-lookup"><span data-stu-id="1be14-117">(See below for details about the various properties).</span></span>
4. <span data-ttu-id="1be14-118">當您將媒體輸入媒體清單並設定 [一般] 設定之後，請選取應用程式右上方的 [發佈] 按鈕。</span><span class="sxs-lookup"><span data-stu-id="1be14-118">Once you've entered the media into the media list and have configured the general settings, select the publish button in the top-right part of the app.</span></span>
5. <span data-ttu-id="1be14-119">發佈完成後，對話方塊會顯示兩個文字，讓您進入您所放置的多媒體主控台。</span><span class="sxs-lookup"><span data-stu-id="1be14-119">Once the publish has completed, a dialog will pop up with a two word code for you to enter in to the Multimedia Console you placed.</span></span>
  
### <a name="placing-the-multimedia-console-in-your-environment"></a><span data-ttu-id="1be14-120">將多媒體主控台放在您的環境中</span><span class="sxs-lookup"><span data-stu-id="1be14-120">Placing the Multimedia console in your environment</span></span>

1. <span data-ttu-id="1be14-121">在 [ **世界編輯器] > 編輯器面板上，> SDK 應用程式 > 多媒體主控台**。</span><span class="sxs-lookup"><span data-stu-id="1be14-121">Select on **World Editor > Editor Panel > SDK Apps > Multimedia Console**.</span></span> <span data-ttu-id="1be14-122"> (不會移至 **> 基本 > SDK 應用程式的世界編輯器**，這適用于未註冊的應用程式。 ) </span><span class="sxs-lookup"><span data-stu-id="1be14-122">(Don't go to **World Editor > Basics > SDK App**--that's for unregistered apps.)</span></span>  
2. <span data-ttu-id="1be14-123">將多媒體主控台定位到最適合您的空間和物件。</span><span class="sxs-lookup"><span data-stu-id="1be14-123">Position the Multimedia Console to best suite your space and audience.</span></span>
3. <span data-ttu-id="1be14-124">按一下 [橙色編輯模式] 按鈕，即可退出編輯模式。</span><span class="sxs-lookup"><span data-stu-id="1be14-124">Get out of Edit Mode by clicking the orange Edit Mode button.</span></span>
4. <span data-ttu-id="1be14-125">系統會提示您提供 **媒體播放機擁有者嗎？**</span><span class="sxs-lookup"><span data-stu-id="1be14-125">You'll be prompted **Are you the media player owner?**</span></span> <span data-ttu-id="1be14-126">如果您是此多媒體主控台會話的官方擁有者，請確認並繼續。</span><span class="sxs-lookup"><span data-stu-id="1be14-126">If you're the person who should be the official owner of this Multimedia Console session, confirm and continue.</span></span> <span data-ttu-id="1be14-127"> (其他許可角色也可供使用。</span><span class="sxs-lookup"><span data-stu-id="1be14-127">(Other permissioned roles are available as well.</span></span> <span data-ttu-id="1be14-128">如需詳細清單，請參閱下方。 ) </span><span class="sxs-lookup"><span data-stu-id="1be14-128">See below for a detailed list.)</span></span>
5. <span data-ttu-id="1be14-129">選取 [是] 以確認您是主要主機。</span><span class="sxs-lookup"><span data-stu-id="1be14-129">Select Yes to confirm that you are the primary host.</span></span>  
6. <span data-ttu-id="1be14-130">對話方塊應該會出現，要求您從 web 入口網站輸入程式碼或有效的 JSON。</span><span class="sxs-lookup"><span data-stu-id="1be14-130">A dialog should pop up that asks you to enter a code from the web portal or valid JSON.</span></span>  <span data-ttu-id="1be14-131">輸入入口網站中的兩個單字代碼，包括虛線，然後按 [確定]。</span><span class="sxs-lookup"><span data-stu-id="1be14-131">Enter the two word code from the web portal including the dash and hit OK.</span></span> <span data-ttu-id="1be14-132"> (JSON 是如下所述的 advanced 設定) </span><span class="sxs-lookup"><span data-stu-id="1be14-132">(JSON is an advanced configuration described below)</span></span>
7. <span data-ttu-id="1be14-133">使用您在入口網站中建立的設定，會在幾秒後載入多媒體主控台。</span><span class="sxs-lookup"><span data-stu-id="1be14-133">The Multimedia Console should load after a few seconds with the configuration you built in the web portal.</span></span>

### <a name="controlling-the-multimedia-console"></a><span data-ttu-id="1be14-134">控制多媒體主控台</span><span class="sxs-lookup"><span data-stu-id="1be14-134">Controlling the Multimedia console</span></span>

1. <span data-ttu-id="1be14-135">輸入您的程式碼並完成設定程式之後，您會看到控制項按鈕顯示在媒體顯示下方。</span><span class="sxs-lookup"><span data-stu-id="1be14-135">After you input your code and complete the configuration process, you'll see control buttons appear below a media display.</span></span> 
    * <span data-ttu-id="1be14-136">[**播放**] 會啟動媒體檢視器 (或在目前的專案重新開機（如果先前已停止）) </span><span class="sxs-lookup"><span data-stu-id="1be14-136">**Play** starts the media viewer (or restarts at current entry, if previously stopped)</span></span> 
    * <span data-ttu-id="1be14-137">**停止** 停止 media viewer，並隱藏目前的媒體。</span><span class="sxs-lookup"><span data-stu-id="1be14-137">**Stop** stops the media viewer, and hides current media.</span></span>  
    * <span data-ttu-id="1be14-138">**下一個/** 上一個，跳到下一個或上一個媒體</span><span class="sxs-lookup"><span data-stu-id="1be14-138">**Next/Prev** skips to next or previous media</span></span> 
    * <span data-ttu-id="1be14-139">**x/x**  在 [媒體] 清單中顯示目前的索引，並可讓您跳到清單中的任何點</span><span class="sxs-lookup"><span data-stu-id="1be14-139">**x/x** shows the current index into the media list, and allows you to jump to any point in the list</span></span>
    * <span data-ttu-id="1be14-140">**Config** 允許從 web 入口網站重新進入新的程式碼，以在主控台中設定新的設定。</span><span class="sxs-lookup"><span data-stu-id="1be14-140">**Config** allows reentering a new code from the web portal to set a new configuration in the console.</span></span> 

<span data-ttu-id="1be14-141">現在您已經設定為透過多媒體主控台開始共用！</span><span class="sxs-lookup"><span data-stu-id="1be14-141">Now you're set to begin sharing via the Multimedia Console!</span></span>  
 
## <a name="working-with-the-web-portal"></a><span data-ttu-id="1be14-142">使用入口網站</span><span class="sxs-lookup"><span data-stu-id="1be14-142">Working with the web portal</span></span>

<span data-ttu-id="1be14-143">入口網站是一種 web 應用程式，可讓您設定多媒體主控台的各種功能。</span><span class="sxs-lookup"><span data-stu-id="1be14-143">The web portal is a web app that enables configuring the various features of the Multimedia Console.</span></span>  <span data-ttu-id="1be14-144">這些功能分為兩類：一般媒體主控台設定和媒體播放清單。</span><span class="sxs-lookup"><span data-stu-id="1be14-144">These features fall in to two categories; general media console settings, and the media play list.</span></span>

### <a name="multimedia-console-general-settings"></a><span data-ttu-id="1be14-145">多媒體主控台的一般設定</span><span class="sxs-lookup"><span data-stu-id="1be14-145">Multimedia console general settings</span></span>

<span data-ttu-id="1be14-146">**播放設定**</span><span class="sxs-lookup"><span data-stu-id="1be14-146">**Playback Settings**</span></span>

<span data-ttu-id="1be14-147">媒體清單的一般播放設定</span><span class="sxs-lookup"><span data-stu-id="1be14-147">General playback settings for the media list</span></span>

* <span data-ttu-id="1be14-148">**迴圈媒體清單**-決定當您到達清單結尾時，媒體清單是否應迴圈。</span><span class="sxs-lookup"><span data-stu-id="1be14-148">**Loop Media List**- Determines whether the media list should loop around once you reach the end of the list.</span></span>
* <span data-ttu-id="1be14-149">**啟動方法** -選取多媒體主控台應該啟動的方法。</span><span class="sxs-lookup"><span data-stu-id="1be14-149">**Start Method** - Selects the method by which the multimedia console should start.</span></span>
    * <span data-ttu-id="1be14-150">手動-等候在啟動媒體之前按下 [播放] 按鈕</span><span class="sxs-lookup"><span data-stu-id="1be14-150">Manual - Waits for the play button to be pressed before starting the media</span></span>
    * <span data-ttu-id="1be14-151">自動從開頭開始-自動從清單開頭開始進行媒體清單</span><span class="sxs-lookup"><span data-stu-id="1be14-151">Auto Start from Beginning - Auto start the media list from the beginning of the list</span></span>
    * <span data-ttu-id="1be14-152">自動啟動隨機-自動啟動清單中的隨機起始點的媒體</span><span class="sxs-lookup"><span data-stu-id="1be14-152">Auto Start Random - Auto starts the media from a random starting point in the list</span></span>

<span data-ttu-id="1be14-153">**角色**</span><span class="sxs-lookup"><span data-stu-id="1be14-153">**Roles**</span></span>

<span data-ttu-id="1be14-154">用來控制及設定多媒體主控台的角色指派。</span><span class="sxs-lookup"><span data-stu-id="1be14-154">Role assignments for controlling and configuring the Multimedia Console.</span></span>    <span data-ttu-id="1be14-155">這些角色會細分為下列集合：</span><span class="sxs-lookup"><span data-stu-id="1be14-155">These roles are broken down in to the following set:</span></span>

* <span data-ttu-id="1be14-156">**僅擁有** 者-是多媒體主控台會話擁有者的使用者</span><span class="sxs-lookup"><span data-stu-id="1be14-156">**Owner Only** - The user that is the owner of the Multimedia Console Session</span></span>
* <span data-ttu-id="1be14-157">提高 **許可權的使用者**-在原始媒體主控台設定的空間中，擁有仲裁者、主機或展示者角色的使用者</span><span class="sxs-lookup"><span data-stu-id="1be14-157">**Elevated Users** - Users that have moderator, host, or presenter roles in the space that the Multimedia Console is configured in originally</span></span>
* <span data-ttu-id="1be14-158">**所有使用者** -所有使用者</span><span class="sxs-lookup"><span data-stu-id="1be14-158">**All Users** - All users</span></span>

<span data-ttu-id="1be14-159">這些角色的堆疊方式，是在這份清單中選擇的所有角色，也會獲得使用該功能的許可權。</span><span class="sxs-lookup"><span data-stu-id="1be14-159">These roles stack in the sense that all roles above the one chosen in this list will also be granted permission to use that feature.</span></span>  <span data-ttu-id="1be14-160">範例：提高 **許可權的使用者** 在 AltspaceVR 中包含 **擁有** 者，即使他們不是仲裁者、主機或展示者。</span><span class="sxs-lookup"><span data-stu-id="1be14-160">Example: **Elevated Users** includes the **Owner** even if they aren't a moderator, host, or presenter\*\* in AltspaceVR.</span></span> <span data-ttu-id="1be14-161">角色指派所控制的功能如下所示</span><span class="sxs-lookup"><span data-stu-id="1be14-161">Features that are controlled by role assignments are as follows</span></span>

* <span data-ttu-id="1be14-162">**可以控制媒體播放機** -決定哪些角色可以控制多媒體主控台的 media 播放按鈕</span><span class="sxs-lookup"><span data-stu-id="1be14-162">**Can control media player** - Determines what roles can control the media playback buttons for the Multimedia Console</span></span>
* <span data-ttu-id="1be14-163">**可以設定 media player** -藉由授與存取權給 [設定 **] 按鈕，** 判斷哪些角色可以設定多媒體主控台</span><span class="sxs-lookup"><span data-stu-id="1be14-163">**Can configure the media player** - Determines what roles can configure the Multimedia Console by being granted access to the **Config** button</span></span>

### <a name="adding-photos-and-videos-to-the-media-list"></a><span data-ttu-id="1be14-164">將相片和影片新增至媒體清單</span><span class="sxs-lookup"><span data-stu-id="1be14-164">Adding photos and videos to the media list</span></span>

<span data-ttu-id="1be14-165">媒體是多媒體主控台的核心。</span><span class="sxs-lookup"><span data-stu-id="1be14-165">Media is the heart of the Multimedia Console.</span></span>  <span data-ttu-id="1be14-166">影像和影片連結在多媒體主控台內可作為媒體類型來支援。</span><span class="sxs-lookup"><span data-stu-id="1be14-166">Images and video links are supported as media types within the Multimedia Console.</span></span>  <span data-ttu-id="1be14-167">若要新增媒體，請選取 [ **新增影像** ] 或 [ **新增影片** ] 圖示，讓對話方塊快顯以進入媒體資訊和設定。</span><span class="sxs-lookup"><span data-stu-id="1be14-167">To add new media, select either the **Add Image** or **Add Video** icons to have a dialog pop up to enter the media information and settings.</span></span>  <span data-ttu-id="1be14-168">以下是媒體類型和相關設定的細目</span><span class="sxs-lookup"><span data-stu-id="1be14-168">Below is the breakdown of the media types and associated settings</span></span>

<span data-ttu-id="1be14-169">**影像**</span><span class="sxs-lookup"><span data-stu-id="1be14-169">**Image**</span></span>

<span data-ttu-id="1be14-170">影像應該是標準影像類型，例如 jpeg、png 和兒子。</span><span class="sxs-lookup"><span data-stu-id="1be14-170">Images should be a standard image type such as jpeg, png, and son on.</span></span> <span data-ttu-id="1be14-171">它們必須裝載在具有公用連結的某個位置。</span><span class="sxs-lookup"><span data-stu-id="1be14-171">They need to be hosted somewhere with a public link.</span></span>

* <span data-ttu-id="1be14-172">**名稱** - (需要您想要用來識別映射的) 名稱。</span><span class="sxs-lookup"><span data-stu-id="1be14-172">**Name** - (Required) Name that you wish to identify the image with.</span></span>
* <span data-ttu-id="1be14-173">**影像 url** - (影像的公用 Url) 必要項</span><span class="sxs-lookup"><span data-stu-id="1be14-173">**Image URL** - (Required) The public url of the image</span></span>
* <span data-ttu-id="1be14-174">**跳過之後** -應略過影像的秒數</span><span class="sxs-lookup"><span data-stu-id="1be14-174">**Skip After** - The number of seconds that the image should be skipped after</span></span>

<span data-ttu-id="1be14-175">**影片**</span><span class="sxs-lookup"><span data-stu-id="1be14-175">**Video**</span></span>

<span data-ttu-id="1be14-176">影片可透過 Twitch 和 DLive 託管影片或即時資料流。</span><span class="sxs-lookup"><span data-stu-id="1be14-176">Videos can be hosted videos or live streams through Twitch and DLive.</span></span>  <span data-ttu-id="1be14-177"> (其他支援可以與額外的工作一起運作，以取得適當的串流 url，但在多媒體主控台中並未完全支援) </span><span class="sxs-lookup"><span data-stu-id="1be14-177">(Other support may function with extra work to get the proper stream url, but aren't fully supported within the Multimedia Console)</span></span>

* <span data-ttu-id="1be14-178">**名稱** - (需要您想要用來識別影片的) 名稱。</span><span class="sxs-lookup"><span data-stu-id="1be14-178">**Name** - (Required) Name that you wish to identify the video with.</span></span>
* <span data-ttu-id="1be14-179">**影片 URL** - (需要) 影片裝載所在的公用 URL，或提供即時資料流。</span><span class="sxs-lookup"><span data-stu-id="1be14-179">**Video URL** - (Required) The public url that the video is hosted at or the live stream is served from.</span></span>
* <span data-ttu-id="1be14-180">**跳過之後** -應略過影片的秒數</span><span class="sxs-lookup"><span data-stu-id="1be14-180">**Skip After** - The number of seconds that the video should be skipped after</span></span>
* <span data-ttu-id="1be14-181">**磁片** 區-從 0 (min) -1 (最大) 值的影片數量。</span><span class="sxs-lookup"><span data-stu-id="1be14-181">**Volume** - The volume of the video from 0 (min) - 1 (max) values.</span></span>
* <span data-ttu-id="1be14-182">**開始時間** -從影片開頭開始的秒數。</span><span class="sxs-lookup"><span data-stu-id="1be14-182">**Start Time** - The number of seconds from the beginning of the video start from.</span></span>
* <span data-ttu-id="1be14-183">從 **開始距離開始**：當您從多媒體主控台移出時，磁片區開始落在世界中的距離（單位為量）</span><span class="sxs-lookup"><span data-stu-id="1be14-183">**Roll Off Start Distance** - The distance in meters in world that the volume begins to fall off at as you move away from the Multimedia Console</span></span>
* <span data-ttu-id="1be14-184">**影片結束動作** -到達影片結尾時要採取的動作。</span><span class="sxs-lookup"><span data-stu-id="1be14-184">**End of Video Action** - The action to take once the end of the video is reached.</span></span>
    * <span data-ttu-id="1be14-185">停止-媒體清單在影片結束後停止</span><span class="sxs-lookup"><span data-stu-id="1be14-185">Stop - The media list stops after the video has ended</span></span>
    * <span data-ttu-id="1be14-186">迴圈-影片將會迴圈直到手動略過</span><span class="sxs-lookup"><span data-stu-id="1be14-186">Loop - The video will loop until manually skipped</span></span>
    * <span data-ttu-id="1be14-187">下一步-媒體清單中的下一個媒體會在目前的影片結束之後啟動。</span><span class="sxs-lookup"><span data-stu-id="1be14-187">Play Next - The next media in the media list will be started after the current video ends.</span></span>

## <a name="working-with-json-directly-advancedoptional"></a><span data-ttu-id="1be14-188">直接使用 JSON (advanced/optional) </span><span class="sxs-lookup"><span data-stu-id="1be14-188">Working with JSON directly (advanced/optional)</span></span>

<span data-ttu-id="1be14-189">多媒體主控台支援在 AltspaceVR 中直接將 JSON 輸入主控台的提示。</span><span class="sxs-lookup"><span data-stu-id="1be14-189">The Multimedia Console supports entering JSON directly in to the prompt of the console in AltspaceVR.</span></span>  <span data-ttu-id="1be14-190">JSON 是啟用媒體播放機設定的內部機制。</span><span class="sxs-lookup"><span data-stu-id="1be14-190">JSON is the internal mechanism with which we enable media player configurations.</span></span> <span data-ttu-id="1be14-191">公開直接設定 JSON 的功能，可讓更高階的使用者建立自己的工作流程，以將其需求和熟悉的 JSON 組成套件。</span><span class="sxs-lookup"><span data-stu-id="1be14-191">Exposing the ability to set JSON directly is something that allows for more advanced users to build their own workflows that suites their needs and familiarity with JSON.</span></span>  <span data-ttu-id="1be14-192">以下是 JSON 結構的簡短描述，以及 JSON 驗證的架構。</span><span class="sxs-lookup"><span data-stu-id="1be14-192">The following is a brief description of the JSON structure and the schema by which the JSON is validated.</span></span> <span data-ttu-id="1be14-193">如需下列屬性的詳細說明，請參閱上述有關設定多媒體主控台的章節。</span><span class="sxs-lookup"><span data-stu-id="1be14-193">For more detailed descriptions of the properties below, see the above sections that talk about configuring the Multimedia Console.</span></span>  <span data-ttu-id="1be14-194">本節主要著重于 JSON 資料的架構範例和結構。</span><span class="sxs-lookup"><span data-stu-id="1be14-194">This section is focused primarily on the schema examples and structuring for the JSON data.</span></span>

### <a name="global-media-settings"></a><span data-ttu-id="1be14-195">全域媒體設定</span><span class="sxs-lookup"><span data-stu-id="1be14-195">Global media settings</span></span>

```json
{
  "loopMediaList": true | false
  "startMethod": "manual" | "autostart-beginning" | "autostart-random"
  "controlMediaPlayer": "everyone" | "elevated" | "owner"
  "configureMediaPlayer": "elevated" | "owner"
  ...
}
```

### <a name="media-list"></a><span data-ttu-id="1be14-196">媒體清單</span><span class="sxs-lookup"><span data-stu-id="1be14-196">Media list</span></span>

<span data-ttu-id="1be14-197">媒體清單是在 JSON 結構的根目錄設定的屬性，例如角色和播放設定。</span><span class="sxs-lookup"><span data-stu-id="1be14-197">The media list is a property set at the root of the JSON structure like the Roles and Playback Settings.</span></span>  <span data-ttu-id="1be14-198">它是一個簡單的陣列，可包含下列其中一種媒體配置結構。</span><span class="sxs-lookup"><span data-stu-id="1be14-198">It's a simple array that can contain one of the following media configuration structures.</span></span> <span data-ttu-id="1be14-199"> (請參閱上述屬性描述，以取得各項功能的詳細資料。 ) </span><span class="sxs-lookup"><span data-stu-id="1be14-199">(See property descriptions above for details on what each does.)</span></span>

<span data-ttu-id="1be14-200">**影像範例**</span><span class="sxs-lookup"><span data-stu-id="1be14-200">**Image example**</span></span>

<span data-ttu-id="1be14-201">*必要欄位： "name" 和 "imageUrl"*</span><span class="sxs-lookup"><span data-stu-id="1be14-201">*Required fields: "name" and "imageUrl"*</span></span>

```json
{
    "name": "Altspace Screenshot",
    "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
    "skipAfter": 10
}
```

<span data-ttu-id="1be14-202">**影片範例**</span><span class="sxs-lookup"><span data-stu-id="1be14-202">**Video example**</span></span>

<span data-ttu-id="1be14-203">*必要欄位： "name" 和 "videoUrl"*</span><span class="sxs-lookup"><span data-stu-id="1be14-203">*Required fields: "name" and "videoUrl"*</span></span>

```json
{
    "name": "Ninja Twitch Live Stream",
    "videoUrl":"https://www.twitch.tv/ninja",
    "volume":0.2,
    "startTime":0,
    "endOfVideoAction":"play-next"
}
```

### <a name="example-json"></a><span data-ttu-id="1be14-204">範例 JSON</span><span class="sxs-lookup"><span data-stu-id="1be14-204">Example JSON</span></span>

```json
{
  "loopMediaList": false,
  "startMethod": "autostart-beginning",
  "controlMediaPlayer": "everyone",
  "configureMediaPlayer": "elevated",
  "mediaList": [
    {
      "videoUrl": "https://www.twitch.tv/ninja",
      "volume": 0.2,
      "startTime": 0,
      "endOfVideoAction": "play-next"
    },
    {
      "imageUrl": "http://www.hypergridbusiness.com/wp-content/uploads/2016/09/AltspaceVR-highrise.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://d1qb2nb5cznatu.cloudfront.net/startups/i/333629-6ffd7199b9bcf34d8957e8e09d974a38-medium_jpg.jpg?buster=1423092095",
      "skipAfter": 5
    },
    {
      "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://altvr-wpengine.netdna-ssl.com/wp-content/uploads/2019/05/Educators-in-VR-Social-VR-AltspaceVR.png",
      "skipAfter": 10
    },
    {
      "videoUrl": "https://www.twitch.tv/shroud",
      "volume": 1,
      "startTime": 0,
      "endOfVideoAction": "stop"
    }
  ]
}
```

### <a name="schema"></a><span data-ttu-id="1be14-205">結構描述</span><span class="sxs-lookup"><span data-stu-id="1be14-205">Schema</span></span>

```json
{
  "$schema": "https://json-schema.org/draft-04/schema#",
  "type": "object",
  "required": [
    "mediaList"
  ],
  "properties": {
    "loopMediaList": {
      "type": "boolean",
      "description": "Whether to loop through the media list when reaching the beginning or end of the list."
    },
    "controlMediaPlayer": {
      "type": "string",
      "enum": [
        "everyone",
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are able to control the media player. (Owner can always control player)"
    },
    "configureMediaPlayer": {
      "type": "string",
      "enum": [
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are allowed to configure the media play list.  Note: This role needs to be able to control the media player in order to configure it. (Owner can always configure media)"
    },
    "startMethod": {
      "type": "string",
      "enum": [
        "manual",
        "autostart-beginning",
        "autostart-random"
      ],
      "default": "manual",
      "description": "The method by which the media player should start"
    },
    "mediaList": {
      "description": "A list of images or videos to configure the media player to operate on.",
      "type": "array",
      "items": {
        "oneOf": [
          {
            "title": "Image",
            "type": "object",
            "description": "Configuration for an image media.",
            "properties": {
              "imageUrl": {
                "type": "string",
                "description": "The url for the image to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              }
            },
            "required": [
              "imageUrl"
            ]
          },
          {
            "title": "Video",
            "type": "object",
            "description": "Configuration for a video media.",
            "properties": {
              "videoUrl": {
                "type": "string",
                "description": "The url of the video to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              },
              "volume": {
                "type": "number",
                "minimum": 0,
                "maximum": 1,
                "default": null,
                "description": "The volume to play the video at. (Minimum 0, maximum 1)"
              },
              "startTime": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The time in seconds from the start of the video to begin playing the video at. (Minimum of 0)"
              },
              "rolloffStartDistance": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The distance in meters away from the media player that the volume will begin to fall off. (Minimum 0)"
              },
              "endOfVideoAction": {
                "type": "string",
                "enum": [
                  "stop",
                  "loop",
                  "play-next"
                ],
                "default": null,
                "description": "The type of action to take at the end of the video."
              }
            },
            "required": [
              "videoUrl"
            ]
          }
        ]
      }
    }
  }
}
```

> [!NOTE]
> <span data-ttu-id="1be14-206">最新的多媒體主控台 v 0.5。0</span><span class="sxs-lookup"><span data-stu-id="1be14-206">Up to date with Multimedia Console v0.5.0</span></span>