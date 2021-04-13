---
title: 備份您的世界
description: 瞭解如何建立、管理和疑難排解 AltspaceVR 領域的備份快照集。
ms.date: 03/11/2021
ms.topic: article
keywords: 儲存
ms.openlocfilehash: fdef692c737bf2f92db315e04556831d60c2f377
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/08/2021
ms.locfileid: "107211865"
---
# <a name="backing-up-your-worlds"></a><span data-ttu-id="0e564-104">備份您的世界</span><span class="sxs-lookup"><span data-stu-id="0e564-104">Backing up your worlds</span></span>

<span data-ttu-id="0e564-105">備份是在特定時間點的「快照集」或全球所有物件的記錄。</span><span class="sxs-lookup"><span data-stu-id="0e564-105">A Backup is a “snapshot” or record of all the objects in a World at a specific point in time.</span></span> <span data-ttu-id="0e564-106">假設您正在建立您的夢想房子，而一天您不小心刪除了客廳。</span><span class="sxs-lookup"><span data-stu-id="0e564-106">Suppose you’re building your Dream House and one day you accidentally deleted the living room.</span></span> <span data-ttu-id="0e564-107">如果您之前曾建立過全球的備份，您可以還原該特定備份、重設您的世界，並避免發生異常攻擊。</span><span class="sxs-lookup"><span data-stu-id="0e564-107">If you had created a Backup of your World the day before, you could restore that particular backup, reset your World, and avoid a panic attack.</span></span> <span data-ttu-id="0e564-108">或者，您的每一季都有一個插槽的版本，而且想要在兩者之間來回切換—您可以使用備份來進行。</span><span class="sxs-lookup"><span data-stu-id="0e564-108">Or perhaps you have a version of your cabin-in-the-woods for every season and you like to switch back and forth between them—you can do that with Backups.</span></span> <span data-ttu-id="0e564-109">每個備份都是單一世界專屬的，而且不僅包含轉換 (位置、旋轉、縮放) ，也包含物件上的其他設定。</span><span class="sxs-lookup"><span data-stu-id="0e564-109">Each Backup is specific to a single World and contains not only the transforms (position, rotation, scale) but also other settings on the objects.</span></span> <span data-ttu-id="0e564-110">您可以為世界建立的備份數目沒有任何限制。</span><span class="sxs-lookup"><span data-stu-id="0e564-110">There's no limit to the number of Backups you can create for a World.</span></span>  

## <a name="whats-included-in-a-backup"></a><span data-ttu-id="0e564-111">備份包含哪些內容？</span><span class="sxs-lookup"><span data-stu-id="0e564-111">What’s included in a Backup?</span></span>

<span data-ttu-id="0e564-112">備份目前包含您可以使用「世界編輯器」來產生的大部分專案：</span><span class="sxs-lookup"><span data-stu-id="0e564-112">A Backup currently includes most things you can spawn with the World Editor:</span></span>
* <span data-ttu-id="0e564-113">構件 (套件物件) </span><span class="sxs-lookup"><span data-stu-id="0e564-113">Artifacts (Kit objects)</span></span>
* <span data-ttu-id="0e564-114">標籤</span><span class="sxs-lookup"><span data-stu-id="0e564-114">Labels</span></span>
* <span data-ttu-id="0e564-115">Teleporters</span><span class="sxs-lookup"><span data-stu-id="0e564-115">Teleporters</span></span>
* <span data-ttu-id="0e564-116">產生點</span><span class="sxs-lookup"><span data-stu-id="0e564-116">Spawn Points</span></span>
* <span data-ttu-id="0e564-117">照片</span><span class="sxs-lookup"><span data-stu-id="0e564-117">Photos</span></span>
* <span data-ttu-id="0e564-118">深入 SDK 應用程式</span><span class="sxs-lookup"><span data-stu-id="0e564-118">MRE SDK Apps</span></span>
* <span data-ttu-id="0e564-119">原生應用程式 (例如，針對現實的全像) </span><span class="sxs-lookup"><span data-stu-id="0e564-119">Native Apps (for example, Holograms Against Reality)</span></span>

<span data-ttu-id="0e564-120">不包含下列內容：</span><span class="sxs-lookup"><span data-stu-id="0e564-120">The following isn’t included:</span></span>

* <span data-ttu-id="0e564-121">版面配置覆寫</span><span class="sxs-lookup"><span data-stu-id="0e564-121">Layout overrides</span></span>
* <span data-ttu-id="0e564-122">Skyboxes 和環境音效</span><span class="sxs-lookup"><span data-stu-id="0e564-122">Skyboxes and ambient sound</span></span>
* <span data-ttu-id="0e564-123">範本</span><span class="sxs-lookup"><span data-stu-id="0e564-123">Templates</span></span>
* <span data-ttu-id="0e564-124">指示</span><span class="sxs-lookup"><span data-stu-id="0e564-124">Instructions</span></span>
* <span data-ttu-id="0e564-125">世界角色和內容相關角色</span><span class="sxs-lookup"><span data-stu-id="0e564-125">World roles and contextual roles</span></span>

## <a name="managing-backups"></a><span data-ttu-id="0e564-126">管理備份</span><span class="sxs-lookup"><span data-stu-id="0e564-126">Managing Backups</span></span>

<span data-ttu-id="0e564-127">您可以藉由開啟您的世界編輯器/Altspace，然後按一下 [備份] 來建立備份。</span><span class="sxs-lookup"><span data-stu-id="0e564-127">You can create a Backup by opening your World Editor / Altspace and clicking on “Backups”.</span></span> <span data-ttu-id="0e564-128">第一個按鈕會是 [新增備份] 按鈕。</span><span class="sxs-lookup"><span data-stu-id="0e564-128">The first button will be the “New Backup” button.</span></span> <span data-ttu-id="0e564-129">建立備份時，系統會要求您提供簡短名稱。</span><span class="sxs-lookup"><span data-stu-id="0e564-129">When creating a Backup, you’ll be asked to provide a short name.</span></span> <span data-ttu-id="0e564-130">這是選擇性的，但強烈建議您這麼做，因為它會讓您快速混淆。</span><span class="sxs-lookup"><span data-stu-id="0e564-130">This is optional but highly recommended because it will get confusing fast.</span></span> <span data-ttu-id="0e564-131">現有的備份會列在 [建立] 按鈕之後。</span><span class="sxs-lookup"><span data-stu-id="0e564-131">Existing backups will be listed after the “Create” button.</span></span> <span data-ttu-id="0e564-132">按一下現有的備份將會開始還原。</span><span class="sxs-lookup"><span data-stu-id="0e564-132">Clicking on an existing Backup will start a restore.</span></span> <span data-ttu-id="0e564-133">還原備份時，您的世界會在幾分鐘後重設，但您可能不會看到變更反映出來。</span><span class="sxs-lookup"><span data-stu-id="0e564-133">When restoring a Backup, your World will reset after a few moments but you may not see the changes reflected.</span></span> <span data-ttu-id="0e564-134">等候一或兩分鐘，然後再次重設您的世界。</span><span class="sxs-lookup"><span data-stu-id="0e564-134">Wait a minute or two and reset your World again.</span></span> <span data-ttu-id="0e564-135">**目前沒有任何方法可以在 VR 中編輯或刪除備份**。</span><span class="sxs-lookup"><span data-stu-id="0e564-135">**There's currently no way to edit or delete a Backup in VR**.</span></span> <span data-ttu-id="0e564-136">您現在必須在我們的網站上管理您的備份。</span><span class="sxs-lookup"><span data-stu-id="0e564-136">You'll need to manage your Backups on our website for now.</span></span> <span data-ttu-id="0e564-137">在 VR (的備份管理將于近期內改進。</span><span class="sxs-lookup"><span data-stu-id="0e564-137">(Backup management in VR will be improved soon.</span></span> <span data-ttu-id="0e564-138">在此同時，請與我們) 。</span><span class="sxs-lookup"><span data-stu-id="0e564-138">In the meantime, bear with us).</span></span>

<span data-ttu-id="0e564-139">若要在我們的網站上管理您的備份：</span><span class="sxs-lookup"><span data-stu-id="0e564-139">To manage your Backups on our website:</span></span>

1. <span data-ttu-id="0e564-140">流覽至您的世界 [>](https://account.altvr.com/users/sign_in)、找出您的世界，然後按下系統管理員控制項中的「備份」：</span><span class="sxs-lookup"><span data-stu-id="0e564-140">Navigate to [Worlds > Mine](https://account.altvr.com/users/sign_in), find your World, and press “Backups” in the Administrator Controls:</span></span>

![具有備份面板的全球網站系統管理員控制項開啟](images/world-backup-img-01.png)

2. <span data-ttu-id="0e564-142">您可以建立、編輯和刪除您的備份、檢查其中有多少物件，甚至是上傳預覽影像：</span><span class="sxs-lookup"><span data-stu-id="0e564-142">You can create, edit, and delete your Backups, check how many objects are inside, and even upload a preview image:</span></span> 

![醒目提示 [建立]、[編輯] 和 [刪除] 命令的 [備份] 視窗](images/world-backup-img-02.png)

<span data-ttu-id="0e564-144">備份數目沒有任何限制，而且有更多備份不會影響您世界的效能。</span><span class="sxs-lookup"><span data-stu-id="0e564-144">There's no limit to the number of Backups and having more Backups won't impact the performance of your World.</span></span>

## <a name="other-ways-to-back-up-your-worlds"></a><span data-ttu-id="0e564-145">備份您的世界的其他方式</span><span class="sxs-lookup"><span data-stu-id="0e564-145">Other ways to back up your Worlds</span></span>

* <span data-ttu-id="0e564-146">建立另一個世界、顯示先進的選項，以及從世界匯入。</span><span class="sxs-lookup"><span data-stu-id="0e564-146">Create another World, Show Advanced Options, and Import from World.</span></span> <span data-ttu-id="0e564-147">從下拉式功能表中選擇您想要備份的世界。</span><span class="sxs-lookup"><span data-stu-id="0e564-147">Choose the World you want to back up from the dropdown menu into the new one.</span></span> <span data-ttu-id="0e564-148">Imports 沒有任何限制。</span><span class="sxs-lookup"><span data-stu-id="0e564-148">There no limit for imports.</span></span>
* <span data-ttu-id="0e564-149">如果您使用 Unity 上載者，強烈建議您使用版本控制。</span><span class="sxs-lookup"><span data-stu-id="0e564-149">If you’re using the Unity Uploader, we strongly recommend you use version control.</span></span> <span data-ttu-id="0e564-150">例如， [適用于 Unity 的 Github](https://unity.github.com)。</span><span class="sxs-lookup"><span data-stu-id="0e564-150">For example, [Github for Unity](https://unity.github.com).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="0e564-151">疑難排解</span><span class="sxs-lookup"><span data-stu-id="0e564-151">Troubleshooting</span></span>

<span data-ttu-id="0e564-152">**協助！我不小心還原了備份，也** 不需要擔心我的工作。</span><span class="sxs-lookup"><span data-stu-id="0e564-152">**Help! I accidentally restored a Backup and my work is gone** Don’t worry.</span></span> <span data-ttu-id="0e564-153">我們會自動建立新的備份，然後再還原舊的備份。</span><span class="sxs-lookup"><span data-stu-id="0e564-153">We automatically create a new Backup before restoring old one.</span></span> <span data-ttu-id="0e564-154">使用正確的時間戳記，尋找名稱開頭為 **Auto** 的名稱，並還原該一個 (例如， **auto 2019-01-14T08：23： 33-08： 00**) 。</span><span class="sxs-lookup"><span data-stu-id="0e564-154">Look for one with a name starting with **Auto** with the right timestamp and restore that one (for example, **Auto 2019-01-14T08:23:33-08:00**).</span></span>  <span data-ttu-id="0e564-155">如果未正常運作，請提交 [支援要求](https://help.altvr.com/hc/requests/new)</span><span class="sxs-lookup"><span data-stu-id="0e564-155">If that doesn’t work submit a [Support request](https://help.altvr.com/hc/requests/new)</span></span>

<span data-ttu-id="0e564-156">**我已還原備份，但缺少某些物件** 如果有任何相片，這些相片是否已刪除？</span><span class="sxs-lookup"><span data-stu-id="0e564-156">**I restored a Backup and some objects are missing** If any were photos, were those photos deleted?</span></span> <span data-ttu-id="0e564-157">基於隱私權原因，我們無法還原已刪除的相片。</span><span class="sxs-lookup"><span data-stu-id="0e564-157">We can’t restore deleted photos for privacy reasons.</span></span> <span data-ttu-id="0e564-158">提交 [支援要求](https://help.altvr.com/hc/requests/new) 以便進行調查</span><span class="sxs-lookup"><span data-stu-id="0e564-158">Submit a [Support request](https://help.altvr.com/hc/requests/new) so we can investigate</span></span>

<span data-ttu-id="0e564-159">**我看不到任何變更** 備份會以非同步方式還原，這表示可能需要幾分鐘的時間來還原，視物件數目而定。</span><span class="sxs-lookup"><span data-stu-id="0e564-159">**I don’t see any changes** Backups are restored asynchronously meaning they can take a few minutes to restore depending on the number of objects.</span></span> <span data-ttu-id="0e564-160">請記得重設您的世界，如果在幾分鐘之後看不到任何時間，請重試一次。</span><span class="sxs-lookup"><span data-stu-id="0e564-160">Remember to reset your World and if you don’t see anything after a few minutes try resetting again.</span></span> <span data-ttu-id="0e564-161">未來，我們可以針對還原流程的狀態提供更多的意見反應</span><span class="sxs-lookup"><span data-stu-id="0e564-161">In the future, we can provide more feedback on the status of the restoration process</span></span>