---
title: 使用 Interactables Spawner
description: 瞭解如何建立、使用和自訂 interactables spawner，以將專案放在您的 AltspaceVR 空間中。
ms.date: 02/10/2021
ms.topic: article
keywords: spawner，互動，自訂
ms.openlocfilehash: 7f4b87591b2e11b2084af4d2bf83748ed51fd193
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212576"
---
# <a name="using-the-interactables-spawner"></a><span data-ttu-id="a693b-104">使用 Interactables Spawner</span><span class="sxs-lookup"><span data-stu-id="a693b-104">Using the Interactables Spawner</span></span>

<span data-ttu-id="a693b-105">Interactables Spawner 可讓您將互動專案放置在您的活動、世界或家庭空間中。</span><span class="sxs-lookup"><span data-stu-id="a693b-105">The Interactables Spawner allows you to place interactable items in your event, world, or home-space.</span></span> <span data-ttu-id="a693b-106">這項功能目前是 [早期存取程式](../world-building/early-access.md) 的一部分，除非您選擇透過主功能表，否則無法使用此功能。</span><span class="sxs-lookup"><span data-stu-id="a693b-106">This feature is currently part of our [Early Access Program](../world-building/early-access.md) and won't be available unless you've opted in through your Main Menu.</span></span>

> [!NOTE]
> <span data-ttu-id="a693b-107">雖然我們繼續試驗這項功能，但請注意，產生太多 interactables 可能會影響您的環境或事件的效能。</span><span class="sxs-lookup"><span data-stu-id="a693b-107">While we continue to pilot this feature please be aware that spawning too many interactables may affect the performance of your environment or event.</span></span> 

## <a name="creating-an-interactable"></a><span data-ttu-id="a693b-108">建立互動</span><span class="sxs-lookup"><span data-stu-id="a693b-108">Creating an interactable</span></span>

<span data-ttu-id="a693b-109">若要將物件轉換成互動物件：</span><span class="sxs-lookup"><span data-stu-id="a693b-109">To turn your object into an interactable object:</span></span>

1. <span data-ttu-id="a693b-110">將物件放在您的空間中。</span><span class="sxs-lookup"><span data-stu-id="a693b-110">Place the object in your space.</span></span>
2. <span data-ttu-id="a693b-111">然後，在 [物件] 清單中尋找專案，然後選取旁邊的 **齒輪圖示** 以開啟其設定：</span><span class="sxs-lookup"><span data-stu-id="a693b-111">Then, find the entry in the object list, and select the **gear icon** next to it to open its settings:</span></span>

![以反白顯示的物件清單開啟的世界編輯器](images/interactables-spawner-img-01.png)

<span data-ttu-id="a693b-113">在 [設定] 頁面上，您會看到新的 **[物件 spawner**] 核取方塊，用來將它設為互動物件。</span><span class="sxs-lookup"><span data-stu-id="a693b-113">On the settings page you’ll find a new checkbox **“Object spawner“**, which is used to make it an interactable object.</span></span>

1. <span data-ttu-id="a693b-114">核取該方塊，然後選取 [ **確認**]。</span><span class="sxs-lookup"><span data-stu-id="a693b-114">Check the box and select **confirm**.</span></span>
2. <span data-ttu-id="a693b-115">在編輯模式中，您可以四處移動物件在空間中的產生位置。</span><span class="sxs-lookup"><span data-stu-id="a693b-115">While in edit mode, you can move around the object’s spawn location in the space.</span></span>
3. <span data-ttu-id="a693b-116">**離開編輯模式** 以啟用專案互動。</span><span class="sxs-lookup"><span data-stu-id="a693b-116">**Exit edit mode** to enable item interaction.</span></span>

![在 AltspaceVR 應用程式中開啟的更新成品視窗](images/interactables-spawner-img-02.png)

## <a name="other-customizations"></a><span data-ttu-id="a693b-118">其他自訂內容</span><span class="sxs-lookup"><span data-stu-id="a693b-118">Other customizations</span></span>

<span data-ttu-id="a693b-119">當您返回 [ **物件 spawner]** 之後，當您回到該物件的屬性時，將會有額外的設定，可讓您套用至產生的物件行為。</span><span class="sxs-lookup"><span data-stu-id="a693b-119">After enabling **“Object spawner”** when you go back into the properties for that object, there will be an extra setting you can apply to how the spawned object behaves.</span></span>

> [!NOTE]
> <span data-ttu-id="a693b-120">互動物件縮放：這會在物件被挑選時設定物件的小數位數，相較于「調整」，這是物件在第一次挑選之前出現在世界中的比例。</span><span class="sxs-lookup"><span data-stu-id="a693b-120">Interactable object scale: This sets the scale of the object when it gets picked up, compared to “Scale” which is the scale of how the object appears in the world prior to picking it up for the first time.</span></span>

<span data-ttu-id="a693b-121">套件製作者可能會注意到，AltspaceVR 正在執行時對套件所做的變更，在您重新開機 AltspaceVR 之前將不會生效。</span><span class="sxs-lookup"><span data-stu-id="a693b-121">Kit makers may notice that changes to your Kit while AltspaceVR is running won't take effect until you restart AltspaceVR.</span></span>

<span data-ttu-id="a693b-122">最近我們已在 [ **一般設定** ] 索引標籤下新增名為 [ **重載世界套件**] 的按鈕。</span><span class="sxs-lookup"><span data-stu-id="a693b-122">Recently we’ve added a button under the **Moderate Settings** tab called **Reload Worlds Kits**.</span></span> <span data-ttu-id="a693b-123">按一下這個按鈕會導致 (您) 重新輸入空間，再次重載所有套件，這只會下載您在 AltspaceVR 時更新的新套件版本。</span><span class="sxs-lookup"><span data-stu-id="a693b-123">Clicking this button causes (just you) to reenter the space, reloading all Kits again, which will download only new versions of the Kits that have been updated while you were in AltspaceVR.</span></span>

![在 AltspaceVR 應用程式中開啟適中設定面板](images/interactables-spawner-img-03.png)