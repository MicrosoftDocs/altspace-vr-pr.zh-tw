---
title: 新增自訂產生點
description: 瞭解如何建立、新增和疑難排解自訂產生點至 AltspaceVR。
ms.date: 03/11/2021
ms.topic: article
keywords: spawnpoint，疑難排解
ms.openlocfilehash: 0f53bdc229eb21e50edef34981c592556236fc55
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212222"
---
# <a name="adding-custom-spawn-points"></a><span data-ttu-id="56889-104">新增自訂產生點</span><span class="sxs-lookup"><span data-stu-id="56889-104">Adding custom spawn points</span></span>

<span data-ttu-id="56889-105">進入您世界的人員會在進入您的世界時， **產生或顯示** 在原始位置， (0，0，0) 。</span><span class="sxs-lookup"><span data-stu-id="56889-105">People entering your World will **spawn** or appear at the origin, position (0,0,0), when they enter your World.</span></span> <span data-ttu-id="56889-106">但是，如果您想要的話，您可以新增一或多個產生點，比方說，您可以讓使用者開始進入 castle。</span><span class="sxs-lookup"><span data-stu-id="56889-106">However, you can add one or more Spawn Points if you want to, say, have people start at the entrance to your castle.</span></span> <span data-ttu-id="56889-107">如果您指定多個產生點，就會在每次有人進入時隨機播放一個，而不會包含該來源。</span><span class="sxs-lookup"><span data-stu-id="56889-107">If you specify multiple Spawn Points, one will be randomly chosen whenever someone enters and the origin won't be included.</span></span> <span data-ttu-id="56889-108">您可以將產生點管理到啟用全球編輯器的任何世界或事件。</span><span class="sxs-lookup"><span data-stu-id="56889-108">You can manage Spawn Points to any World or Event where your World Editor is enabled.</span></span> <span data-ttu-id="56889-109">您可以控制人員產生 (位置) 的位置，以及 (旋轉) 所面向的方向。</span><span class="sxs-lookup"><span data-stu-id="56889-109">You control where people spawn (position) and what direction they'll be facing (rotation).</span></span> <span data-ttu-id="56889-110">只有在編輯模式中才會顯示產生點。</span><span class="sxs-lookup"><span data-stu-id="56889-110">Spawn Points will only be visible in Edit Mode.</span></span> 

1. <span data-ttu-id="56889-111">移至您想要讓人員產生的位置附近。</span><span class="sxs-lookup"><span data-stu-id="56889-111">Go near the spot where you want people to spawn.</span></span> <span data-ttu-id="56889-112">> 基本] 開啟 [ **世界編輯器** ]，並確定已核取 [ **鎖定旋轉** ]。</span><span class="sxs-lookup"><span data-stu-id="56889-112">Open **World Editor > Basics** and make sure **Lock Rotation** is checked.</span></span> <span data-ttu-id="56889-113">選取 [產生 **點** ] 以建立一個。</span><span class="sxs-lookup"><span data-stu-id="56889-113">Select **Spawn Point** to create one.</span></span> <span data-ttu-id="56889-114">將它移到您想要的確切位置：</span><span class="sxs-lookup"><span data-stu-id="56889-114">Move it to the exact position you want:</span></span>

![全球編輯器基本概念視窗開啟](images/spawn-points-img-01.png)

2. <span data-ttu-id="56889-116">選取產生點的設定圖示，並確定 **旋轉 > X** 和 **旋轉 > Z** 都是 **0**。</span><span class="sxs-lookup"><span data-stu-id="56889-116">Select on the settings icon for the Spawn Point and make sure **Rotation > X** and **Rotation > Z** are both **0**.</span></span> <span data-ttu-id="56889-117">如果它們是很小的數位，例如 **8.537777745 e-07**，也沒關係。</span><span class="sxs-lookup"><span data-stu-id="56889-117">If they are small numbers like **8.537777745E-07**, that's fine too.</span></span> <span data-ttu-id="56889-118">這是如何處理浮點數的怪癖：</span><span class="sxs-lookup"><span data-stu-id="56889-118">That's a quirk of how floating point numbers are handled:</span></span>

![在全球編輯器設定中更新產生點](images/spawn-points-img-02.png)

3. <span data-ttu-id="56889-120">透過功能表 > 設定重新輸入您的世界 **> 一般 > 重新輸入空間 >**</span><span class="sxs-lookup"><span data-stu-id="56889-120">Reenter your World via **Menu > Settings > General > Reenter Space > Re-Enter**</span></span>
4. <span data-ttu-id="56889-121">您應該會產生新的衍生點！</span><span class="sxs-lookup"><span data-stu-id="56889-121">You should spawn at your new Spawn Point!</span></span>
5. <span data-ttu-id="56889-122">如果您想要讓人們面對不同的方向，請選取產生點的設定，並只將 **旋轉 > Y** 。</span><span class="sxs-lookup"><span data-stu-id="56889-122">If you want people to face a different direction, select the settings for the Spawn Point and set **Rotation > Y** only.</span></span> <span data-ttu-id="56889-123">嘗試將 Y 設定為180，且 X 和 Z 為 0 (警告： X 和 Z 是 advanced，可能會讓人病假) 。</span><span class="sxs-lookup"><span data-stu-id="56889-123">Try setting Y to 180 and both X and Z to 0 (Warning: X and Z are advanced may make people sick).</span></span> <span data-ttu-id="56889-124">然後選取 [ **確認** ]，然後重新輸入世界。</span><span class="sxs-lookup"><span data-stu-id="56889-124">Then select **Confirm** and reenter the World.</span></span> <span data-ttu-id="56889-125">這應該會產生相反方向的。</span><span class="sxs-lookup"><span data-stu-id="56889-125">That should spawn you facing the opposite direction.</span></span> 

## <a name="troubleshooting"></a><span data-ttu-id="56889-126">疑難排解</span><span class="sxs-lookup"><span data-stu-id="56889-126">Troubleshooting</span></span>

<span data-ttu-id="56889-127">**人們仍在原點產生？**</span><span class="sxs-lookup"><span data-stu-id="56889-127">**People still spawning at the origin?**</span></span>
    * <span data-ttu-id="56889-128">確定您的產生點會稍微在地面或表面上。</span><span class="sxs-lookup"><span data-stu-id="56889-128">Make sure your Spawn Points are slightly above the ground or surface.</span></span> <span data-ttu-id="56889-129">如果產生點與其他物件重迭，則人員會在預設位置（來源）產生。</span><span class="sxs-lookup"><span data-stu-id="56889-129">If the Spawn Point is overlapping other objects, people spawn at the default location, the origin.</span></span> <span data-ttu-id="56889-130">如果物件內的產生點和 person 的高度不同，就會發生這種情況。</span><span class="sxs-lookup"><span data-stu-id="56889-130">This can happen if the Spawn Point inside an object and the height of person varies.</span></span> 
    * <span data-ttu-id="56889-131">嘗試透過 **功能表 > 設定 > 適中 > 重設空間**）來重設您的世界</span><span class="sxs-lookup"><span data-stu-id="56889-131">Try resetting your World via **Menu > Settings > Moderate > Reset Space**</span></span>

<span data-ttu-id="56889-132">**有多個產生點，但是仍在相同的位置產生？**</span><span class="sxs-lookup"><span data-stu-id="56889-132">**Have multiple Spawn Points but still spawning in the same place?**</span></span>
<span data-ttu-id="56889-133">您可能會不幸地--這是隨機的。</span><span class="sxs-lookup"><span data-stu-id="56889-133">You might be unlucky--it's random after all.</span></span> <span data-ttu-id="56889-134">請在假設發生錯誤之前，先嘗試幾次重新進入至少五次。</span><span class="sxs-lookup"><span data-stu-id="56889-134">Try a few reentering at least five times before assuming there's an error.</span></span> 

<span data-ttu-id="56889-135">**人們不太舒服或他們的標頭是傾斜** 的您可能忘了檢查 **鎖定旋轉** 或設定旋轉的 X 和 Z 值。</span><span class="sxs-lookup"><span data-stu-id="56889-135">**People are uncomfortable or their head is tilted** You may have forgotten to check **Lock Rotation** or set the X and Z value for Rotation.</span></span> <span data-ttu-id="56889-136">除非您要建立外來世界，否則這些通常應該設定為0。</span><span class="sxs-lookup"><span data-stu-id="56889-136">Those should usually be set to 0 unless you're building an exotic World.</span></span> 

<span data-ttu-id="56889-137">**人們產生的時候？**</span><span class="sxs-lookup"><span data-stu-id="56889-137">**People falling when they spawn?**</span></span>
<span data-ttu-id="56889-138">請勿在物件上方設定產生點位置過高。</span><span class="sxs-lookup"><span data-stu-id="56889-138">Don't set the Spawn Point position too high above an object.</span></span> <span data-ttu-id="56889-139">如果它們太遠，則會 respawned 在原點。</span><span class="sxs-lookup"><span data-stu-id="56889-139">If they fall too far, they'll be respawned at the origin.</span></span>