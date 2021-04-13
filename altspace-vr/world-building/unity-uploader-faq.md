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
# <a name="unity-uploader-help"></a><span data-ttu-id="6b52b-104">Unity 上載者說明</span><span class="sxs-lookup"><span data-stu-id="6b52b-104">Unity Uploader help</span></span>

<span data-ttu-id="6b52b-105">**1. 這項工具有多棒？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-105">**1. How awesome is this tool?**</span></span>

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/cheyenne-mountain-gate-room-v1/player]

<span data-ttu-id="6b52b-106">這就是我的 Stargate Unity 場景，內含可為閘道和 DND 提供的 SDK 應用程式</span><span class="sxs-lookup"><span data-stu-id="6b52b-106">That's my Stargate Unity scene with an SDK app powering the Gate and DND</span></span>

<span data-ttu-id="6b52b-107">**2. 我是影片學習模組，我的影片在哪裡？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-107">**2. I'm a video learner, where's my videos?**</span></span>

[<span data-ttu-id="6b52b-108">查看我們的影片</span><span class="sxs-lookup"><span data-stu-id="6b52b-108">Check out our videos</span></span>](https://youtu.be/km9CnVYPzoM)

<span data-ttu-id="6b52b-109">**3. 我可以在哪裡找到範例？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-109">**3. Where can I find examples?**</span></span>

<span data-ttu-id="6b52b-110">[精選的世界](https://account.altvr.com/worlds/featured) 和 [Jimmy 的範例](https://account.altvr.com/worlds/1046572460192825569) 是很好的起點</span><span class="sxs-lookup"><span data-stu-id="6b52b-110">[Featured Worlds](https://account.altvr.com/worlds/featured) and [Jimmy's Examples](https://account.altvr.com/worlds/1046572460192825569) are good places to start</span></span>

<span data-ttu-id="6b52b-111">**4. 這是否適用于套件和新的 SDK？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-111">**4. Will this work with Kits and the new SDK?**</span></span>
<span data-ttu-id="6b52b-112">是的，如果您想要的話，可以一起使用所有工具。</span><span class="sxs-lookup"><span data-stu-id="6b52b-112">Yes, you can use all the tools together if you'd like.</span></span> <span data-ttu-id="6b52b-113">我們正在嘗試開發它們，以便緊密合作。</span><span class="sxs-lookup"><span data-stu-id="6b52b-113">We're trying to develop them to work seamlessly together.</span></span>

<span data-ttu-id="6b52b-114">**5. 它是否支援粒子效果？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-114">**5. Does it support particle effects?**</span></span>

![雪粒子效果的 GIF](images/uploader-faq-img-01.gif)

<span data-ttu-id="6b52b-116">**6. 我可以取得 hrtf 音訊嗎？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-116">**6. Can I get spatialized audio?**</span></span>
<span data-ttu-id="6b52b-117">目前不是，但您可以放置音訊來源，以在當地語系化的區域中播放。</span><span class="sxs-lookup"><span data-stu-id="6b52b-117">Not right now but you can place audio sources to play in localized areas.</span></span> 

<span data-ttu-id="6b52b-118">**7. 內建光源是否正常運作？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-118">**7. Does baked lighting work?**</span></span>
<span data-ttu-id="6b52b-119">是，但您的燈光必須設定為 "內建"，而不是「混合」</span><span class="sxs-lookup"><span data-stu-id="6b52b-119">Yes, but your lights have to be set to "baked" and not "mixed"</span></span>

<span data-ttu-id="6b52b-120">**8. 全球照明是否正常運作？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-120">**8. Does global illumination work?**</span></span>
<span data-ttu-id="6b52b-121">Yes</span><span class="sxs-lookup"><span data-stu-id="6b52b-121">Yes</span></span>

<span data-ttu-id="6b52b-122">**9. 您一定要重設世界嗎？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-122">**9. Do you always have to reset the World?**</span></span>
<span data-ttu-id="6b52b-123">是。</span><span class="sxs-lookup"><span data-stu-id="6b52b-123">Yes.</span></span> <span data-ttu-id="6b52b-124">每次都必須重載 Unity 資產套件組合。</span><span class="sxs-lookup"><span data-stu-id="6b52b-124">We have to reload the Unity Asset Bundles every time.</span></span> 

<span data-ttu-id="6b52b-125">**10. 我可以使用自己的自訂材質和著色器嗎？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-125">**10. Can I use my own custom materials and shaders?**</span></span>

![自訂材質和著色器的 GIF](images/uploader-faq-img-02.gif)

<span data-ttu-id="6b52b-127">**11. 我可以只上傳到一個平臺嗎？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-127">**11. Can I upload to one platform only?**</span></span>
<span data-ttu-id="6b52b-128">是，使用上載工具。</span><span class="sxs-lookup"><span data-stu-id="6b52b-128">Yes, using the Uploader tool.</span></span> <span data-ttu-id="6b52b-129">不過，在 Android 上的人員在您上傳其平臺的場景之前，將不會看到您世界中的任何事物。</span><span class="sxs-lookup"><span data-stu-id="6b52b-129">However, people who are on Android won't see anything in your World until you upload the scene for their platform.</span></span> 

<span data-ttu-id="6b52b-130">**12. 是否允許腳本？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-130">**12. Are scripts allowed?**</span></span>
<span data-ttu-id="6b52b-131">否，基於安全性理由，我們不能允許腳本或腳本參考。</span><span class="sxs-lookup"><span data-stu-id="6b52b-131">No, for security reasons we can't allow scripts or script references.</span></span> <span data-ttu-id="6b52b-132">如果您的上傳包含腳本或腳本參考，則會被拒絕。</span><span class="sxs-lookup"><span data-stu-id="6b52b-132">If your upload contains scripts or script references, it will be rejected.</span></span> <span data-ttu-id="6b52b-133">如果您的世界需要撰寫腳本，請參閱新的 SDK。</span><span class="sxs-lookup"><span data-stu-id="6b52b-133">Take a look at the new SDK if you World needs scripting.</span></span> 

<span data-ttu-id="6b52b-134">**13. 我可以上傳的場景有多大？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-134">**13. How big of a scene can I upload?**</span></span>
<span data-ttu-id="6b52b-135">我們建議您從小規模開始，並留意 Altspace 中沒有怪物電腦的人員。</span><span class="sxs-lookup"><span data-stu-id="6b52b-135">We suggest you start small and be mindful of people in Altspace who don't have monster PCs.</span></span> <span data-ttu-id="6b52b-136">話雖如此，我們已經有遊戲進入其 maps 以進行即時串流 (例如，射擊的「VR」遊戲) </span><span class="sxs-lookup"><span data-stu-id="6b52b-136">That said, we've had games bring in their maps for live streams (for example, Onward, a VR shooter game)</span></span>

![AltspaceVR 中的 VR 遊戲螢幕擷取畫面](images/uploader-faq-img-03.png)

<span data-ttu-id="6b52b-138">**14. 我必須裝載場景檔案嗎？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-138">**14. Do I have to host the scene files?**</span></span>
<span data-ttu-id="6b52b-139">否，Altspace 會在您上傳檔案後提供檔案</span><span class="sxs-lookup"><span data-stu-id="6b52b-139">No, Altspace is serving up the files once you upload them</span></span>

<span data-ttu-id="6b52b-140">**15. 允許陰影嗎？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-140">**15. Are shadows allowed?**</span></span>
<span data-ttu-id="6b52b-141">Yes</span><span class="sxs-lookup"><span data-stu-id="6b52b-141">Yes</span></span>

<span data-ttu-id="6b52b-142">**16. 我可以使用上傳者來快速進行反覆運算嗎？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-142">**16. How quickly can I iterate using the Uploader?**</span></span>
<span data-ttu-id="6b52b-143">如果您已在世界中，您可以在上傳程式中按下傳、重設您的世界，並在最少10秒內查看更新的場景。</span><span class="sxs-lookup"><span data-stu-id="6b52b-143">If you're already in your World, you can press Upload in the Uploader, reset your World, and see the updated scene in as little as 10 seconds.</span></span> <span data-ttu-id="6b52b-144">通常，您會看到30秒到幾分鐘的迴圈，視場景的複雜度而定。</span><span class="sxs-lookup"><span data-stu-id="6b52b-144">Typically, you'll see loops of 30 seconds to a few minutes depending on the complexity of your scene.</span></span> <span data-ttu-id="6b52b-145">有個飲料，讓您成為世界 Builder！</span><span class="sxs-lookup"><span data-stu-id="6b52b-145">Have a drink, you deserve it for being a World-Builder!</span></span>

<span data-ttu-id="6b52b-146">**17. 哪裡可以取得3D 模型？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-146">**17. Where do I get 3D models?**</span></span>
<span data-ttu-id="6b52b-147">Sketchfab、Sketchup、Minecraft、Unity 資產存放區等等。</span><span class="sxs-lookup"><span data-stu-id="6b52b-147">Sketchfab, Sketchup, Minecraft, Unity Asset Store, and so on.</span></span>

<span data-ttu-id="6b52b-148">**18. 它是否支援動畫？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-148">**18. Does it support animations?**</span></span>

![自訂動畫執行的 GIF](images/uploader-faq-img-04.gif)

<span data-ttu-id="6b52b-150">**19. 如何設定空間音訊？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-150">**19. How can I set up spatial audio?**</span></span> <span data-ttu-id="6b52b-151">匯入所選的 wav 檔案，在場景中建立空白的遊戲物件，並選取此物件。</span><span class="sxs-lookup"><span data-stu-id="6b52b-151">Import the wav file of choice, create an empty game object in the scene and select this object.</span></span> <span data-ttu-id="6b52b-152">將您匯入的音效拖放至物件的偵測器，它就會建立音訊來源。</span><span class="sxs-lookup"><span data-stu-id="6b52b-152">Drag and drop your imported sound to the inspector of the object and it will create an audio source.</span></span> <span data-ttu-id="6b52b-153">之後，將音量調整為不超過0.5，將空間 blend 變更為3D，然後調整最小和最大距離以建立適當的音效區域。</span><span class="sxs-lookup"><span data-stu-id="6b52b-153">Afterwards adjust the volume to no more than 0.5, change the spatial blend to 3D, and adjust the min and Max distance to create a proper area of sound.</span></span> <span data-ttu-id="6b52b-154">根據預設，這會顯示為球體，例如 colliders。</span><span class="sxs-lookup"><span data-stu-id="6b52b-154">This is displayed as sphere like colliders by default.</span></span> <span data-ttu-id="6b52b-155">若要取得真正的下降，您必須根據自己的喜好來調整下拉曲線。</span><span class="sxs-lookup"><span data-stu-id="6b52b-155">To get a true drop off, you'll need to adjust the drop off curve to your liking.</span></span> [<span data-ttu-id="6b52b-156"> (via @IsThatToasted) </span><span class="sxs-lookup"><span data-stu-id="6b52b-156">(via @IsThatToasted)</span></span>](https://www.youtube.com/watch?v=ktb2vAAwknw&list=PLGmYIROty-5bpzKQNK3mRMi4pmh_LinV4&t=642s&index=29)

<span data-ttu-id="6b52b-157">**20. 我要如何看到跨眼尖/奇怪？**</span><span class="sxs-lookup"><span data-stu-id="6b52b-157">**20. How come I'm seeing cross-eyed / weirdness?**</span></span>
<span data-ttu-id="6b52b-158">有時，上傳程式無法成功覆寫您的轉譯設定。</span><span class="sxs-lookup"><span data-stu-id="6b52b-158">Sometimes the Uploader doesn't successfully override your rendering settings.</span></span> <span data-ttu-id="6b52b-159">[移至編輯 > 專案設定 > Player]。</span><span class="sxs-lookup"><span data-stu-id="6b52b-159">"Go to Edit > Project Settings > Player".</span></span> <span data-ttu-id="6b52b-160">確定已核取 [支援 > 虛擬實境的 XR 設定] 和 [立體轉譯方法] 是 [單一傳遞] 或 [單一傳遞 (預覽) ]，適用于 PC 和 Android (選取機器人圖示) 。</span><span class="sxs-lookup"><span data-stu-id="6b52b-160">Make sure "XR Settings > Virtual Reality Supported" is checked and "Stereo Rendering Method" is "Single Pass" or "Single Pass (Preview)" for both PC and Android (select the robot icon).</span></span> <span data-ttu-id="6b52b-161">之後再進行組建 + 上傳，並重設您的世界。</span><span class="sxs-lookup"><span data-stu-id="6b52b-161">Afterwards build + upload again and reset your World.</span></span> 