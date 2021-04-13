---
title: 使用混合現實擴充功能
description: 瞭解如何使用混合現實延伸模組並進行疑難排解，以擴充及調整您的 AltspaceVR 世界。
ms.date: 03/11/2021
ms.topic: article
keywords: 混合的現實、延伸模組、疑難排解
ms.openlocfilehash: 498e71c48f7c67abc40ce4f4667c9eeac4c4e73b
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/08/2021
ms.locfileid: "107211861"
---
# <a name="using-a-mixed-reality-extension"></a><span data-ttu-id="528e2-104">使用混合現實擴充功能</span><span class="sxs-lookup"><span data-stu-id="528e2-104">Using a Mixed Reality Extension</span></span>

<span data-ttu-id="528e2-105">[混合現實延伸](https://developer.altvr.com/) 模組 (MREs) 是您可以在世界中使用的應用程式，從 [頭盔](https://account.altvr.com/mres/1173667287173955931) 到工作中的 [Stargate](https://account.altvr.com/mres/1152987031857529562)。</span><span class="sxs-lookup"><span data-stu-id="528e2-105">[Mixed Reality Extensions](https://developer.altvr.com/) (MREs) are apps you can use in your Worlds from [helmets](https://account.altvr.com/mres/1173667287173955931) to a working [Stargate](https://account.altvr.com/mres/1152987031857529562).</span></span> <span data-ttu-id="528e2-106">這就是使用程式設計經驗的社區成員可以擴充 Altspace，而單向世界產生器可以讓他們的世界更具互動性。</span><span class="sxs-lookup"><span data-stu-id="528e2-106">This is how community members with programming experience can extend Altspace and one-way World Builders can make their Worlds more interactive.</span></span> <span data-ttu-id="528e2-107">雖然世界上的任何人都可以使用 MREs，但只有全球大樓的人員能夠在世界各地流覽和產生 MREs。</span><span class="sxs-lookup"><span data-stu-id="528e2-107">While MREs can be used by anyone in a World, only people in the World Building Program can browse and spawn MREs in their Worlds.</span></span> 

1. <span data-ttu-id="528e2-108">流覽 [網站](https://account.altvr.com/mres)的 [深入] 區段。</span><span class="sxs-lookup"><span data-stu-id="528e2-108">Browse the MRE section of our [website](https://account.altvr.com/mres).</span></span> <span data-ttu-id="528e2-109">根據預設，您會看到自己的 MREs，因此請選取 [ **Altspace** ] 以查看官方 MREs 和 **精選** ，以查看來自社區的 MREs。</span><span class="sxs-lookup"><span data-stu-id="528e2-109">By default you'll see your own MREs so select on **Altspace** to see official MREs and **Featured** to see MREs from the community.</span></span> <span data-ttu-id="528e2-110">在您的世界中使用之前，先熟悉任何深入。</span><span class="sxs-lookup"><span data-stu-id="528e2-110">Get familiar with any MRE before you use it in your World.</span></span> 
2. <span data-ttu-id="528e2-111">流覽至 [ [頭盔](https://account.altvr.com/mres/1173667287173955931) ] 深入，然後選取 [ **複製到剪貼** 簿]。</span><span class="sxs-lookup"><span data-stu-id="528e2-111">Navigate to the [Helmets](https://account.altvr.com/mres/1173667287173955931) MRE and select **Copy to Clipboard**.</span></span> 
3. <span data-ttu-id="528e2-112">輸入您的世界，並開啟「世界編輯器」以 **> SDK 應用程式的基本概念**。</span><span class="sxs-lookup"><span data-stu-id="528e2-112">Enter your World and open the World Editor to **Basics > SDK App**.</span></span> <span data-ttu-id="528e2-113">將頭盔的 URL 貼到 [目標 URI] 欄位中，然後選取 [ **確認**]。</span><span class="sxs-lookup"><span data-stu-id="528e2-113">Paste in the URL for Helmets into the Target URI field and select **Confirm**.</span></span> <span data-ttu-id="528e2-114">深入物件應該會出現，並嘗試連線到在雲端中執行的深入。</span><span class="sxs-lookup"><span data-stu-id="528e2-114">The MRE Object should appear and attempt to connect to the MRE that's running in the cloud.</span></span> <span data-ttu-id="528e2-115">您現在應該會看到您可以按一下的一些頭盔。</span><span class="sxs-lookup"><span data-stu-id="528e2-115">You should now see some helmets you can click on.</span></span>
4. <span data-ttu-id="528e2-116">移動/旋轉或調整深入的方式，就像是任何其他世界物件一樣。</span><span class="sxs-lookup"><span data-stu-id="528e2-116">Move/rotate/scale the MRE just as you would any other World Object.</span></span>

<span data-ttu-id="528e2-117">恭喜！</span><span class="sxs-lookup"><span data-stu-id="528e2-117">Congratulations!</span></span> <span data-ttu-id="528e2-118">您目前使用的是 MREs--您太酷了！</span><span class="sxs-lookup"><span data-stu-id="528e2-118">You're using MREs now--you're so cool!</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="528e2-119">疑難排解</span><span class="sxs-lookup"><span data-stu-id="528e2-119">Troubleshooting</span></span>

<span data-ttu-id="528e2-120">**深入正在顯示哭表情**</span><span class="sxs-lookup"><span data-stu-id="528e2-120">**MRE is showing a frowning emoji**</span></span> 
    * <span data-ttu-id="528e2-121">確認 URL 是否正確</span><span class="sxs-lookup"><span data-stu-id="528e2-121">Verify that the URL is correct</span></span>
    * <span data-ttu-id="528e2-122">切換為物件上的 [**現正播放**] 選項，然後選擇 [**確認**]</span><span class="sxs-lookup"><span data-stu-id="528e2-122">Toggle **Is Playing** option on the Object and choose **confirm**</span></span>
    * <span data-ttu-id="528e2-123">嘗試重新進入</span><span class="sxs-lookup"><span data-stu-id="528e2-123">Try reentering</span></span>

<span data-ttu-id="528e2-124">**深入為延遲** 視裝載深入的位置而定，您可能會遇到一些網路延遲</span><span class="sxs-lookup"><span data-stu-id="528e2-124">**MRE is lagging** Depending on where an MRE is hosted you may experience some network latency</span></span>

<span data-ttu-id="528e2-125">**為什麼需要貼上 Url？**</span><span class="sxs-lookup"><span data-stu-id="528e2-125">**Why do we have to paste URLs?**</span></span>
<span data-ttu-id="528e2-126">未來，您可以管理和產生 MREs，就像從套件進行成品一樣。</span><span class="sxs-lookup"><span data-stu-id="528e2-126">In the future, you can manage and spawn MREs like you do Artifacts from Kits.</span></span> <span data-ttu-id="528e2-127">在那之前，我們將繼續使用 Url</span><span class="sxs-lookup"><span data-stu-id="528e2-127">Until then, we'll continue using URLs</span></span>