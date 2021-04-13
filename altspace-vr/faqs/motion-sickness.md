---
title: AltspaceVR 會導致移動 sickness 嗎？
description: 隨時掌握最新的常見問題和解決方案，以在 VR 環境中 sickness 動作。
ms.date: 02/10/2021
ms.topic: article
keywords: 運動 sickness、vr、nausea
ms.openlocfilehash: 54f746bc2b213f011dbf94c2703ed039b4717d72
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212485"
---
# <a name="will-altspacevr-cause-motion-sickness"></a><span data-ttu-id="51040-104">AltspaceVR 會導致移動 sickness 嗎？</span><span class="sxs-lookup"><span data-stu-id="51040-104">Will AltspaceVR cause motion sickness?</span></span>

## <a name="why-do-some-people-feel-ill-in-vr"></a><span data-ttu-id="51040-105">為什麼某些人覺得在 VR 中不正確？</span><span class="sxs-lookup"><span data-stu-id="51040-105">Why do some people feel ill in VR?</span></span>

<span data-ttu-id="51040-106">所有的 VR 都會導致 vertigo 和 nausea。</span><span class="sxs-lookup"><span data-stu-id="51040-106">It's a popular belief that all VR causes vertigo and nausea.</span></span> <span data-ttu-id="51040-107">問題源自于您的眼睛之間的差異，以及內部 ear 如何傳送至您的大腦。</span><span class="sxs-lookup"><span data-stu-id="51040-107">The problem stems from a discrepancy between what your eyes are seeing, and what your inner ear is transmitting to your brain.</span></span> <span data-ttu-id="51040-108">當您的眼睛偵測到移動時，您的耳也會傳達您仍在使用的情況下，有些人的大腦可能會因引發 dizziness 和 nausea 而有反應。</span><span class="sxs-lookup"><span data-stu-id="51040-108">When your eyes detect motion, and your ears communicate that you're standing still, some individuals' brain may react by inducing dizziness and nausea.</span></span> <span data-ttu-id="51040-109">有些人更容易使用運動 sickness，可能會對此現象造成更大的影響，而其他人可能不會有問題。</span><span class="sxs-lookup"><span data-stu-id="51040-109">Some people who are more susceptible to motion sickness may be more sensitive to this phenomenon, while others may not have an issue with it.</span></span> 

<span data-ttu-id="51040-110">硬體層級有幾件事，還有一些 AltspaceVR 的軟體會在 VR 中大幅減少或完全排除 nausea 引發的動作。</span><span class="sxs-lookup"><span data-stu-id="51040-110">There are several things that are done at the hardware level, and some in AltspaceVR's software that severely reduces or completely eliminate the nausea-inducing motion in VR.</span></span>

## <a name="hardware-based-nausea-reduction"></a><span data-ttu-id="51040-111">Hardware-Based Nausea 縮減</span><span class="sxs-lookup"><span data-stu-id="51040-111">Hardware-Based Nausea Reduction</span></span>

<span data-ttu-id="51040-112">像是 Oculus Rift 和 HTC Vive 這類的現代的 VR 硬體，藉由以消除可能導致 nausea 的延遲率來呈現影片畫面，來減少運動 sickness。</span><span class="sxs-lookup"><span data-stu-id="51040-112">Contemporary VR hardware like the Oculus Rift and HTC Vive, reduces motion sickness by presenting video frames at a rate that eliminates the latency that can cause nausea.</span></span> <span data-ttu-id="51040-113">如果軟體已優化，而 AltspaceVR 為，則當您在 VR 中開啟標頭時，將不會有任何延遲。</span><span class="sxs-lookup"><span data-stu-id="51040-113">If the software is optimized, as AltspaceVR is, then there's no perceived delay when you turn your head in VR.</span></span> <span data-ttu-id="51040-114">HMD 中的加速計會以更快的速度來傳達移動和傳輸該遙測，而人類眼可以偵測到任何延遲。</span><span class="sxs-lookup"><span data-stu-id="51040-114">The accelerometers in the HMD are communicating movement and transmitting that telemetry faster than the human eye can detect any latency.</span></span> <span data-ttu-id="51040-115">在使用位置攝影機科系的 HMD 模型上，這會更進一步，不僅會呈現旋轉的移動，也是橫向 (側邊) 的動作。</span><span class="sxs-lookup"><span data-stu-id="51040-115">On HMD models outfitted with positional cameras, this goes a step further, not only is rotational movement represented, so is lateral (side to side) motion.</span></span>

## <a name="software-based-nausea-reduction"></a><span data-ttu-id="51040-116">Software-Based Nausea 縮減</span><span class="sxs-lookup"><span data-stu-id="51040-116">Software-Based Nausea Reduction</span></span>

<span data-ttu-id="51040-117">除了硬體改良和 framerates 之外，AltspaceVR 還實行了幾項功能，可協助人們減少和消除 nausea：</span><span class="sxs-lookup"><span data-stu-id="51040-117">In addition to hardware improvements and framerates, AltspaceVR has implemented several features that help people reduce and eliminate nausea:</span></span>

* <span data-ttu-id="51040-118">**Teleporting** -立即從點對點移動不會將動作傳達給大腦，藉此消除 sickness 的動作。</span><span class="sxs-lookup"><span data-stu-id="51040-118">**Teleporting** - Moving instantaneously from point-to-point doesn't communicate motion to the brain, thereby eliminating motion sickness.</span></span>
* <span data-ttu-id="51040-119">AltspaceVR 所有硬體的嵌入式 **管理單元**，在 VR 中提供「ratcheted」或「逐步」旋轉的意思。</span><span class="sxs-lookup"><span data-stu-id="51040-119">**Snap Turning** - On all hardware, AltspaceVR provides means for "ratcheted" or "stepped" rotation of the view in VR.</span></span> <span data-ttu-id="51040-120">換句話說，當您開啟時，您的視圖會旋轉大約20度的旋轉。</span><span class="sxs-lookup"><span data-stu-id="51040-120">In other words when turning, your view will pivot about 20 degrees of rotation.</span></span> <span data-ttu-id="51040-121">同樣地，這不會在大部分的人中觸發 nausea。</span><span class="sxs-lookup"><span data-stu-id="51040-121">Again, this doesn't trigger nausea in most people.</span></span>
* <span data-ttu-id="51040-122">**貼齊動作** -在特定硬體上，在觸控板上向前輕量會在不觸發運動 sickness 的遞增中向前移動透視。</span><span class="sxs-lookup"><span data-stu-id="51040-122">**Snap Motion** - On certain hardware, swiping forward on the touchpad will move the perspective forward in an increment that doesn't trigger motion sickness.</span></span> 
 
## <a name="suggestions-for-eliminating-motion-sickness"></a><span data-ttu-id="51040-123">消除運動 Sickness 的建議</span><span class="sxs-lookup"><span data-stu-id="51040-123">Suggestions for Eliminating Motion Sickness</span></span>

<span data-ttu-id="51040-124">**獨立式**</span><span class="sxs-lookup"><span data-stu-id="51040-124">**Stand Still**</span></span>

<span data-ttu-id="51040-125">試著不要使用控制器來移動太多，只是在 VR 中旋轉您的前端/或向上/向下尋找。</span><span class="sxs-lookup"><span data-stu-id="51040-125">Try not to move around too much using the controllers, just rotate your head/or up/down to look around in VR.</span></span>

<span data-ttu-id="51040-126">**請勿使用滑鼠/KB 或控制器**</span><span class="sxs-lookup"><span data-stu-id="51040-126">**Don't Use a Mouse/KB or Controller**</span></span>

<span data-ttu-id="51040-127">AltspaceVR 可讓使用者選擇使用標準遊戲週邊設備（例如滑鼠/鍵盤和遊戲控制器）在 VR 中移動，就像在視頻遊戲中一樣。</span><span class="sxs-lookup"><span data-stu-id="51040-127">AltspaceVR offers users the option to use standard gaming peripherals such as Mouse/Keyboard and Game controllers to move in VR as you would in a video game.</span></span> <span data-ttu-id="51040-128">這包括多方向移動、strafing 和 turbo 按鈕。</span><span class="sxs-lookup"><span data-stu-id="51040-128">This includes multi-directional movement, strafing, and a turbo button.</span></span> <span data-ttu-id="51040-129">我們建議您只在習慣採用 VR 之後才使用這些功能。</span><span class="sxs-lookup"><span data-stu-id="51040-129">We recommend using these only after becoming accustomed to being in VR.</span></span> <span data-ttu-id="51040-130">就算如此，還是會變慢。</span><span class="sxs-lookup"><span data-stu-id="51040-130">Even then, take it slow.</span></span>

<span data-ttu-id="51040-131">**您可以隨時退出**</span><span class="sxs-lookup"><span data-stu-id="51040-131">**You Can Always Bail Out**</span></span>

<span data-ttu-id="51040-132">如果您遇到 nausea，請立即移除您的 HMD。</span><span class="sxs-lookup"><span data-stu-id="51040-132">If you experience nausea, remove your HMD immediately.</span></span> <span data-ttu-id="51040-133">重新取得您的均衡、平靜您的 stomach，以及準備好返回 VR 環境。</span><span class="sxs-lookup"><span data-stu-id="51040-133">Regain your equilibrium, calm your stomach, and when ready return to the VR environment.</span></span> <span data-ttu-id="51040-134">請嘗試記住造成刺痛的移動，並避免重複。</span><span class="sxs-lookup"><span data-stu-id="51040-134">Try to remember the movement that caused the sensation and refrain from repeating it.</span></span>

<span data-ttu-id="51040-135">**知道何時結束 VR**</span><span class="sxs-lookup"><span data-stu-id="51040-135">**Know When it's Time to Exit VR**</span></span>

<span data-ttu-id="51040-136">最重要的是，知道何時需要休息。</span><span class="sxs-lookup"><span data-stu-id="51040-136">Most importantly, know when it's time to take a break.</span></span> <span data-ttu-id="51040-137">您知道您的內文，並在為您提供強指示，指出有問題，請聆聽。</span><span class="sxs-lookup"><span data-stu-id="51040-137">You know your body, and when it's giving you strong indication that something is wrong, listen.</span></span> <span data-ttu-id="51040-138">拿出中斷並取得一些空氣。</span><span class="sxs-lookup"><span data-stu-id="51040-138">Take a break and get some air.</span></span> <span data-ttu-id="51040-139">四處解說並重新調整您的均衡。</span><span class="sxs-lookup"><span data-stu-id="51040-139">Walk around and realign your equilibrium.</span></span> <span data-ttu-id="51040-140">同樣地，請回頭看看，我們相信這一方仍會繼續進行。</span><span class="sxs-lookup"><span data-stu-id="51040-140">Once you feel good again, come back, we're confident the party will still be going!</span></span>