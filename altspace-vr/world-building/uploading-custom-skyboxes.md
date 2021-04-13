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
# <a name="uploading-custom-skyboxes"></a><span data-ttu-id="8e3c9-104">上傳自訂 Skyboxes</span><span class="sxs-lookup"><span data-stu-id="8e3c9-104">Uploading custom Skyboxes</span></span>

<span data-ttu-id="8e3c9-105">Skybox 可讓您建立世界的 **背景** ，讓體驗更具沉浸。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-105">A Skybox is a way to create a **background** for your World that makes the experience more immersive.</span></span> <span data-ttu-id="8e3c9-106">Skyboxes 有不同的類型，但我們目前支援 **equirectangular**。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-106">There are different kinds of Skyboxes but we currently support **equirectangular**.</span></span> <span data-ttu-id="8e3c9-107">以下是使用360攝影機所採用的範例 (更多[範例) ：](http://moments.mankindforward.com/)</span><span class="sxs-lookup"><span data-stu-id="8e3c9-107">Here's an example taken with a 360 camera (more example [here](http://moments.mankindforward.com/)):</span></span> 

![360 equirectangular 觀賞客廳](images/custom-skyboxes-img-01.jpeg)

<span data-ttu-id="8e3c9-109">您也可以使用 [Unity 上載](world-building-toolkit-getting-started.md) 程式，但這種方法比較簡單。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-109">You can also use the [Unity Uploader](world-building-toolkit-getting-started.md) but this approach is simpler.</span></span>

1. <span data-ttu-id="8e3c9-110">流覽至 [ [世界] > Skyboxes](https://account.altvr.com/skyboxes) ，然後按右邊的 [ **建立** ] 按鈕</span><span class="sxs-lookup"><span data-stu-id="8e3c9-110">Navigate to [Worlds > Skyboxes](https://account.altvr.com/skyboxes) and press the **Create** button on the right</span></span>

![在 [skyboxes] 面板中開啟的 [世界網站] 頁面](images/custom-skyboxes-img-02.png)

2. <span data-ttu-id="8e3c9-112">填入名稱並指定您的360影像。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-112">Fill in a name and specify your 360 image.</span></span> <span data-ttu-id="8e3c9-113">這並不是相片，有些程式可以讓您自行繪製，也可以在線上搜尋。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-113">It doesn't have to be a photo, there are programs that let you draw your own or you can search for some online.</span></span> <span data-ttu-id="8e3c9-114">當您準備好時，選取 [建立]。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-114">When you're ready, select **Create**.</span></span> 

![Skybox 建立表單](images/custom-skyboxes-img-03.png)

3. <span data-ttu-id="8e3c9-116">您可以選擇上傳 **預覽** 影像，以便輕鬆地識別此 skybox。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-116">You can optionally upload a **preview** image so you can easily identify this skybox.</span></span> <span data-ttu-id="8e3c9-117">您也可以上傳 WAV 格式的環境音訊。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-117">You can also upload ambient audio in WAV format.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="8e3c9-118">建議您在上傳360影像之後，分別上傳預覽影像和環境音訊。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-118">We recommend you upload preview images and ambient audio separately, after you upload the 360 image.</span></span> <span data-ttu-id="8e3c9-119">如果您將它們上傳，檔案大小可能夠大而無法停止處理常式。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-119">If you upload them together the file sizes can be large enough to stall the process.</span></span> <span data-ttu-id="8e3c9-120">[Jetsons World](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) 是如何搭配使用 Skybox 與環境音效的絕佳範例。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-120">[Jetsons World](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) is a great example of how to use a Skybox with ambient audio.</span></span> <span data-ttu-id="8e3c9-121">請注意，全球 Builder 如何保持音效，而您聽到的音效是偶爾出現的，讓人們不會感到苦惱。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-121">Notice how the World-Builder kept the audio volume low and sounds you hear are sporadic so people don't get annoyed.</span></span> 

4. <span data-ttu-id="8e3c9-122">輸入您的世界，然後開啟 [World 編輯器]。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-122">Enter your World and open the World Editor.</span></span> <span data-ttu-id="8e3c9-123">在 [Skyboxes] 底下，選取新的 Skybox。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-123">Under Skyboxes, select your new Skybox.</span></span> <span data-ttu-id="8e3c9-124">幾秒鐘後，天空就會變動。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-124">In a few seconds, the sky will literally change.</span></span> <span data-ttu-id="8e3c9-125">您世界上的其他人也會看到天空變更。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-125">Others in your World will also see the sky change.</span></span> <span data-ttu-id="8e3c9-126">若要切換回，請選擇相同清單中的 **預設** skybox。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-126">To switch back, choose the **default** skybox in that same list.</span></span> 

## <a name="troubleshooting"></a><span data-ttu-id="8e3c9-127">疑難排解</span><span class="sxs-lookup"><span data-stu-id="8e3c9-127">Troubleshooting</span></span>

<span data-ttu-id="8e3c9-128">**天空中有接合線或線：- (。**</span><span class="sxs-lookup"><span data-stu-id="8e3c9-128">**There's a seam or line in the sky :-(.**</span></span> <span data-ttu-id="8e3c9-129">這是我們即將修正的 bug</span><span class="sxs-lookup"><span data-stu-id="8e3c9-129">It's a bug that we'll fix soon</span></span>

<span data-ttu-id="8e3c9-130">**上傳失敗**</span><span class="sxs-lookup"><span data-stu-id="8e3c9-130">**Upload failed**</span></span>
    * <span data-ttu-id="8e3c9-131">嘗試自行上傳360映射</span><span class="sxs-lookup"><span data-stu-id="8e3c9-131">try uploading just the 360 image on its own</span></span>
    * <span data-ttu-id="8e3c9-132">嘗試使用另一個較小的檔案作為測試</span><span class="sxs-lookup"><span data-stu-id="8e3c9-132">try with another, smaller file as a test</span></span>

<span data-ttu-id="8e3c9-133">**我找不到360相片**</span><span class="sxs-lookup"><span data-stu-id="8e3c9-133">**I can't find a 360 photo**</span></span>
    * <span data-ttu-id="8e3c9-134">Flickr 是很好的來源 (變更篩選以尋找創意的 commons) </span><span class="sxs-lookup"><span data-stu-id="8e3c9-134">Flickr is a good source (change the filters to find creative commons ones)</span></span>
    * <span data-ttu-id="8e3c9-135">拿自己！</span><span class="sxs-lookup"><span data-stu-id="8e3c9-135">Take your own!</span></span> <span data-ttu-id="8e3c9-136">Ricoh 的攝影機都成功。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-136">We've had success with Ricoh's cameras.</span></span> 
<span data-ttu-id="8e3c9-137">**天空看起來有顆粒狀或 blocky** 您可能需要找到較高解析度的影像。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-137">**The sky looks grainy or blocky** You may need to find a higher-resolution image.</span></span> <span data-ttu-id="8e3c9-138">通常大約 2-5 MB 和 ~ 5000 px x 2000 px</span><span class="sxs-lookup"><span data-stu-id="8e3c9-138">Typically around 2-5 MB and ~5000 px x 2000 px</span></span>

<span data-ttu-id="8e3c9-139">**它會影響我的世界幀率！**</span><span class="sxs-lookup"><span data-stu-id="8e3c9-139">**It hurts my World's framerate!**</span></span>
<span data-ttu-id="8e3c9-140">影像可能太大。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-140">The image is probably too large.</span></span> <span data-ttu-id="8e3c9-141">某些產生的 skyboxes 可以是8k。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-141">Some generated skyboxes can be 8k.</span></span> <span data-ttu-id="8e3c9-142">它們通常會隨附適用于 mobile 的2k 版本，請使用該版本。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-142">They usually come with mobile-friendly 2k versions--use that.</span></span>

<span data-ttu-id="8e3c9-143">**使用環境音訊協助我**</span><span class="sxs-lookup"><span data-stu-id="8e3c9-143">**Help me with the ambient audio**</span></span>
    * <span data-ttu-id="8e3c9-144">使用 >audacity 之類的免費軟體來降低磁片區，或建立您自己的迴圈。</span><span class="sxs-lookup"><span data-stu-id="8e3c9-144">Use free software like Audacity to lower the volume or create your own loops.</span></span> <span data-ttu-id="8e3c9-145">請記住，音訊將會在人們的系統中重複執行並播放，讓它保持低且不討厭</span><span class="sxs-lookup"><span data-stu-id="8e3c9-145">Remember that the audio will be repeated and playing in people's ears so keep it low and not annoying</span></span>
    * <span data-ttu-id="8e3c9-146">[自由音效](https://freesound.org/) 是絕佳的免權利物來源</span><span class="sxs-lookup"><span data-stu-id="8e3c9-146">[Free Sound](https://freesound.org/) is a good source of royalty-free sounds</span></span>
