---
title: 匯入 glTF 模型
description: 瞭解如何正確地將 3D glTF 模型匯入您的 AltspaceVR 體驗，並針對任何問題進行疑難排解。
ms.date: 03/11/2021
ms.topic: article
keywords: 模型、glTF、匯入、sketchfab、疑難排解
ms.openlocfilehash: 4489f90832bd1cf85ff161caed11684257cce6ab
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212433"
---
# <a name="importing-gltf-models"></a><span data-ttu-id="5d838-104">匯入 glTF 模型</span><span class="sxs-lookup"><span data-stu-id="5d838-104">Importing glTF models</span></span>

> [!NOTE]
> <span data-ttu-id="5d838-105">這項功能目前可用於早期存取程式中的選取使用者。</span><span class="sxs-lookup"><span data-stu-id="5d838-105">This feature is available for select users in the Early Access program at this time.</span></span>

<span data-ttu-id="5d838-106">將3D 模型和場景帶入 Altspace 的其中一種方式是使用 [glTF 標準](https://en.wikipedia.org/wiki/GlTF)。</span><span class="sxs-lookup"><span data-stu-id="5d838-106">One way to bring 3D models and scenes into Altspace is using the [glTF standard](https://en.wikipedia.org/wiki/GlTF).</span></span> <span data-ttu-id="5d838-107">您可以 (封裝的 glTF) 上傳 glb 檔案，以建立您稍後可以在世界編輯器中產生的模型。</span><span class="sxs-lookup"><span data-stu-id="5d838-107">You can upload a .glb file (packed glTF) to create a Model that you can later spawn in the World Editor.</span></span> <span data-ttu-id="5d838-108">這是 [上傳您自己的套件](uploading-custom-kits.md)的替代方案。</span><span class="sxs-lookup"><span data-stu-id="5d838-108">It's an alternative to [uploading your own Kits](uploading-custom-kits.md).</span></span> <span data-ttu-id="5d838-109">建議您建立快速示範的模型，因為您不需要使用 Unity 和套件來充分發揮效能和重複使用性。</span><span class="sxs-lookup"><span data-stu-id="5d838-109">We recommend creating Models for quick demonstrations because you won't need to use Unity, and Kits when you want to maximize performance and reusability.</span></span> 

1. <span data-ttu-id="5d838-110">尋找一些 glTF 3D 資產。</span><span class="sxs-lookup"><span data-stu-id="5d838-110">Find some glTF 3D assets.</span></span> <span data-ttu-id="5d838-111">要搜尋的其中一個位置是 Sketchfab (嘗試篩選) [這](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models)類 **可下載** 的模型。</span><span class="sxs-lookup"><span data-stu-id="5d838-111">One place to search is Sketchfab (try filtering for **Downloadable** models like [this](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models)).</span></span> <span data-ttu-id="5d838-112">找到之後，請選取 [ **下載3D 模型**：</span><span class="sxs-lookup"><span data-stu-id="5d838-112">Once you find it, select **Download 3D Model**:</span></span>

![Sketchfab 的3D 狗模型](images/importing-models-img-01.png)

2. <span data-ttu-id="5d838-114">將連結複製到模型，並閱讀授權需求。</span><span class="sxs-lookup"><span data-stu-id="5d838-114">Copy the link to the model and read the licensing requirements.</span></span> 
3. <span data-ttu-id="5d838-115">下載 **Autoconverted 格式 (glTF)** 版本</span><span class="sxs-lookup"><span data-stu-id="5d838-115">Download the **Autoconverted Format (glTF)** version</span></span>

![已反白顯示自動轉換格式的 Sketchfab 下載選項](images/importing-models-img-02.png)

4. <span data-ttu-id="5d838-117">開啟 [GLB Packer](https://glb-packer.glitch.me)網站，並核取 [**將 PNG 轉換成 JPEG (Beta 版**] 核取方塊) </span><span class="sxs-lookup"><span data-stu-id="5d838-117">Open the [GLB Packer](https://glb-packer.glitch.me) site and check the box **Convert PNG to JPEG (beta)**</span></span>
5. <span data-ttu-id="5d838-118">將您下載的 glTF 檔案解壓縮，並將它們一次全部拖曳至 [GLB Packer 瀏覽器] 索引標籤</span><span class="sxs-lookup"><span data-stu-id="5d838-118">Uncompress the glTF files you downloaded and drag them all at once into the GLB Packer browser tab</span></span>

![顯示模型解壓縮的視窗](images/importing-models-img-03.png)

6. <span data-ttu-id="5d838-120">視檔案的數目和大小而定，可能需要一段時間才能處理。</span><span class="sxs-lookup"><span data-stu-id="5d838-120">Depending on the number and size of the files, it may take a while to process.</span></span> <span data-ttu-id="5d838-121">處理完成時，將會下載 **glb** 檔案。</span><span class="sxs-lookup"><span data-stu-id="5d838-121">When processing is done, an **out.glb** file will be downloaded.</span></span> <span data-ttu-id="5d838-122">將該檔案重新命名為有資訊的內容--這會是世界中物件的名稱 (例如 **低 Poly Wolf. glb**) </span><span class="sxs-lookup"><span data-stu-id="5d838-122">Rename that file to something informative--this will be the name of the object in the world (e.g **Low Poly Wolf.glb**)</span></span>
7. <span data-ttu-id="5d838-123">流覽至 [altvr.com > 更 > 的模型](https://account.altvr.com/users/sign_in)，然後選取 [**建立**]</span><span class="sxs-lookup"><span data-stu-id="5d838-123">Navigate to [altvr.com > More > Models](https://account.altvr.com/users/sign_in) and select **Create**</span></span>
8. <span data-ttu-id="5d838-124">請指定 glb 檔案的位置，並確定您將 Sketchfab 連結複製到屬性的描述中。</span><span class="sxs-lookup"><span data-stu-id="5d838-124">Specify the location of the .glb file and make sure you copy the Sketchfab link into the description for attribution.</span></span> <span data-ttu-id="5d838-125">您可以視需要指定預覽影像，然後選取 [ **建立模型**：</span><span class="sxs-lookup"><span data-stu-id="5d838-125">You can specify a preview image if you want, then select **Create Model**:</span></span>

![AltspaceVR 中的模型預覽](images/importing-models-img-04.png)

9. <span data-ttu-id="5d838-127">選取 [**複製到剪貼** 簿]</span><span class="sxs-lookup"><span data-stu-id="5d838-127">Select **Copy to Clipboard**</span></span>
10. <span data-ttu-id="5d838-128">開啟 **全球編輯器 > Altspace > 基本 > GLTF**</span><span class="sxs-lookup"><span data-stu-id="5d838-128">Open the **World Editor > Altspace > Basics > GLTF**</span></span>
11. <span data-ttu-id="5d838-129">貼上您的 url，然後選取 [**確認**]</span><span class="sxs-lookup"><span data-stu-id="5d838-129">Paste in your url and select **Confirm**</span></span>

<span data-ttu-id="5d838-130">恭喜！</span><span class="sxs-lookup"><span data-stu-id="5d838-130">Congrats!</span></span> <span data-ttu-id="5d838-131">您只是產生第一個模型。</span><span class="sxs-lookup"><span data-stu-id="5d838-131">You just spawned your first Model.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="5d838-132">疑難排解</span><span class="sxs-lookup"><span data-stu-id="5d838-132">Troubleshooting</span></span>

<span data-ttu-id="5d838-133">**當我按一下 [ **確認** ] 時沒有任何事**</span><span class="sxs-lookup"><span data-stu-id="5d838-133">**When I clicked **Confirm** nothing happened**</span></span>
    * <span data-ttu-id="5d838-134">我們目前有10萬個多邊形的限制。</span><span class="sxs-lookup"><span data-stu-id="5d838-134">We currently have a 100k polygon limit.</span></span> <span data-ttu-id="5d838-135">如果失敗，請刪除物件，以避免使用者加入您的世界時可能發生的問題</span><span class="sxs-lookup"><span data-stu-id="5d838-135">If it fails, delete the Object to avoid potential problems with users joining your World</span></span>
    * <span data-ttu-id="5d838-136">資產可能有其他問題。</span><span class="sxs-lookup"><span data-stu-id="5d838-136">There may be other problems with the asset.</span></span> <span data-ttu-id="5d838-137">請盡可能使用最少多邊形的資產。</span><span class="sxs-lookup"><span data-stu-id="5d838-137">Try to use assets with as few polygons as possible.</span></span>
    * <span data-ttu-id="5d838-138">您所帶入的模型可能很小或很大。</span><span class="sxs-lookup"><span data-stu-id="5d838-138">The model you're bringing in may be small or large.</span></span> <span data-ttu-id="5d838-139">請嘗試增加/減少比例，或四處移動您的頭像，您可能會在模型內</span><span class="sxs-lookup"><span data-stu-id="5d838-139">Try increasing/decreasing the Scale or move your avatar around, you might be standing inside the model!</span></span>

<span data-ttu-id="5d838-140">**載入速度很慢** 世界上的其他使用者可以快載入的速度，取決於其連線速度。</span><span class="sxs-lookup"><span data-stu-id="5d838-140">**It's slow to load** How quickly other users in the World load it will depend on their connection speeds.</span></span> <span data-ttu-id="5d838-141">它也不會像套件資產一樣快取。</span><span class="sxs-lookup"><span data-stu-id="5d838-141">It's also not cached like Kit assets.</span></span> <span data-ttu-id="5d838-142">如果您將其中一個放在家裡，每次加入時，最後會 redownloading 相同的模型，這並不重要。</span><span class="sxs-lookup"><span data-stu-id="5d838-142">If you place one in your Home, you'll end up redownloading the same Model every time you join, which isn't great.</span></span>

<span data-ttu-id="5d838-143">沒有 **衝突** 依預設，不會發生這種情況下的物件衝突</span><span class="sxs-lookup"><span data-stu-id="5d838-143">**There's no collision** By default there's no collision on the objects that are brought in this way</span></span>

<span data-ttu-id="5d838-144">**當我產生它時，我在六個 DOF 或我的控制項中失去了控制項，因此難以操作** 是的，我們知道這些問題，希望儘快解決這些問題。</span><span class="sxs-lookup"><span data-stu-id="5d838-144">**When I spawn it, I lose my controls on six DOF or I'm inside so it's hard to manipulate it** Yes, we're aware of these issues and hope to address them soon.</span></span>  