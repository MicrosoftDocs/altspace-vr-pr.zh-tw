---
title: 上傳自訂套件
description: 瞭解如何在 AltspaceVR 中設定、產生及上傳您自己的自訂套件，以及疑難排解說明。
ms.date: 03/11/2021
ms.topic: article
keywords: 套件、上傳、疑難排解
ms.openlocfilehash: e5a1b9c2ef5339db0cb821cb6f7d21a930416451
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212553"
---
# <a name="uploading-custom-kits"></a><span data-ttu-id="945b1-104">上傳自訂套件</span><span class="sxs-lookup"><span data-stu-id="945b1-104">Uploading custom kits</span></span>

<span data-ttu-id="945b1-105">「世界編輯器」包含可在您的世界中產生的成品套件。</span><span class="sxs-lookup"><span data-stu-id="945b1-105">The World Editor has Kits containing Artifacts that you can spawn into your World.</span></span> <span data-ttu-id="945b1-106">例如， [Campfire 套件](https://account.altvr.com/kits/993516233267609824) 有許多類型的樹狀結構，每種類型的樹狀結構都是成品。</span><span class="sxs-lookup"><span data-stu-id="945b1-106">For example, the [Campfire Kit](https://account.altvr.com/kits/993516233267609824) has many types of trees--each type of tree is an Artifact.</span></span> <span data-ttu-id="945b1-107">若要建立您自己的套件，您必須建立 Unity AssetBundles 並上傳包含每個成品 Unity 預製專案的 .zip 檔案，並在我們的網站上註冊每個成品。</span><span class="sxs-lookup"><span data-stu-id="945b1-107">To create your own Kit, you have to create Unity AssetBundles and upload a .zip file containing a Unity Prefab for each Artifact and register each Artifact on our website.</span></span> <span data-ttu-id="945b1-108">幸運的是，社區驅動的 Unity 上傳程式會將大部分的工作流程自動化。</span><span class="sxs-lookup"><span data-stu-id="945b1-108">Fortunately, the community-driven Unity Uploader automates most of the workflow.</span></span> <span data-ttu-id="945b1-109">上傳之後，您可以從您自己的套件產生物件，讓其他使用者可以自動看見它們。</span><span class="sxs-lookup"><span data-stu-id="945b1-109">Once uploaded, you can spawn objects from your own Kits in your Worlds and other users can automatically see them.</span></span> <span data-ttu-id="945b1-110">稍後，您可以與您的朋友分享您的套件，也可以透過精選來與整個社區分享。</span><span class="sxs-lookup"><span data-stu-id="945b1-110">Later, you can share your Kit with your friends or even with the entire Community by being featured.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="945b1-111">必要條件</span><span class="sxs-lookup"><span data-stu-id="945b1-111">Prerequisites</span></span>

1. [<span data-ttu-id="945b1-112">安裝 Unity 中樞和 Unity</span><span class="sxs-lookup"><span data-stu-id="945b1-112">Install Unity Hub and Unity</span></span>](world-building-toolkit-getting-started.md)
2. <span data-ttu-id="945b1-113">下載最新版本的[Unity 上載](https://altvr.com/download-latest-unity-uploader/)程式</span><span class="sxs-lookup"><span data-stu-id="945b1-113">Download the latest version of the [Unity Uploader](https://altvr.com/download-latest-unity-uploader/)</span></span>

## <a name="setup"></a><span data-ttu-id="945b1-114">設定</span><span class="sxs-lookup"><span data-stu-id="945b1-114">Setup</span></span> 

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-1-Setup/player]

1. <span data-ttu-id="945b1-115">在我們的全球網站上建立套件 [> 套件](https://account.altvr.com/kits)</span><span class="sxs-lookup"><span data-stu-id="945b1-115">Create a Kit on our website at [Worlds > Kits](https://account.altvr.com/kits)</span></span>
2. <span data-ttu-id="945b1-116">從瀏覽器的網址列將套件識別碼複製到剪貼簿 (此步驟會在上傳版 0.9 + 中更簡單) </span><span class="sxs-lookup"><span data-stu-id="945b1-116">Copy the Kit ID from your browser's address bar to your clipboard (this step will be easier in Uploader versions 0.9+)</span></span>
3. <span data-ttu-id="945b1-117">建立新的 Unity 專案</span><span class="sxs-lookup"><span data-stu-id="945b1-117">Create a new Unity Project</span></span>
4. <span data-ttu-id="945b1-118">按兩下套件以匯入 Unity 上載程式</span><span class="sxs-lookup"><span data-stu-id="945b1-118">Import the Unity Uploader by double-clicking the package</span></span>

![匯入 unity 上載套件](images/custom-kits-img-01.png)

5. <span data-ttu-id="945b1-120">使用您的 Altspace 電子郵件和密碼登入上載程式</span><span class="sxs-lookup"><span data-stu-id="945b1-120">Sign in to the Uploader with your Altspace email and password</span></span>

![Unity 中的 AltspaceVR 登入介面](images/custom-kits-img-02.png)

## <a name="generate-and-upload-your-kit"></a><span data-ttu-id="945b1-122">產生並上傳您的套件</span><span class="sxs-lookup"><span data-stu-id="945b1-122">Generate and upload your kit</span></span>

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-2/player]

1. <span data-ttu-id="945b1-123">以套件識別碼填入套件 **資料夾名稱** 作為前置詞和主題 (例如 **1137484494681408069_Pirates**) ，並以套件識別碼填入 **套件資產名稱** 作為前置詞。</span><span class="sxs-lookup"><span data-stu-id="945b1-123">Fill in **Kit Folder Name** with your Kit ID as the prefix and a theme (for example, **1137484494681408069_pirates**) and fill in **Kit Asset Name** with your Kit ID as the prefix.</span></span> <span data-ttu-id="945b1-124">所有資產都必須有這個前置詞。</span><span class="sxs-lookup"><span data-stu-id="945b1-124">All the assets will need to have this prefix.</span></span>

![Unity 中具有套件資料夾名稱的 AltspaceVR 介面](images/custom-kits-img-03.png)

2. <span data-ttu-id="945b1-126">針對每個成品或一組構件：</span><span class="sxs-lookup"><span data-stu-id="945b1-126">For each Artifact or set of Artifacts:</span></span>
* <span data-ttu-id="945b1-127">將您的來源預製專案 (s) 拖曳至 [階層] 索引標籤</span><span class="sxs-lookup"><span data-stu-id="945b1-127">Drag your source Prefab(s) into the Hierarchy tab</span></span>
* <span data-ttu-id="945b1-128">選取您要包含在集合中的專案，例如五種類型的桶</span><span class="sxs-lookup"><span data-stu-id="945b1-128">Select the ones you want to include in a set, say five types of barrels</span></span>
* <span data-ttu-id="945b1-129">使用 **圓柱** 更新 **套件資產名稱**</span><span class="sxs-lookup"><span data-stu-id="945b1-129">Update the **Kit Asset Name** with **barrel**</span></span>
* <span data-ttu-id="945b1-130">Select **將 GameObject (s) 轉換為套件預製專案**</span><span class="sxs-lookup"><span data-stu-id="945b1-130">Select **Convert GameObject(s) to Kit Prefab**</span></span>
* <span data-ttu-id="945b1-131">確認已在資產/Prefabs 資料夾中建立新的 Prefabs 和螢幕擷取畫面</span><span class="sxs-lookup"><span data-stu-id="945b1-131">Verify that new Prefabs and Screenshots were created in the Assets/Prefabs folder</span></span>

![已選取成品的 Unity 中的 AltspaceVR 介面](images/custom-kits-img-04.png)

> [!NOTE]
> <span data-ttu-id="945b1-133">如果您想要對產生的預製專案進行任何修改，請將其拖曳回階層中，進行變更， **然後按一下 [** 檢查] 索引標籤中的 [套用] 來更新預製專案。</span><span class="sxs-lookup"><span data-stu-id="945b1-133">If you want to make any modifications to a generated Prefab, drag it back into the Hierarchy, make changes, and then click **Apply** in the Inspector tab to update the Prefab.</span></span> 

3. <span data-ttu-id="945b1-134">當您準備好時，請向下 [上傳] 索引標籤，讓我們準備產生具有資產套件組合的 zip 檔案</span><span class="sxs-lookup"><span data-stu-id="945b1-134">When you're ready, scroll down the Uploader tab and let's prepare to generate a zip file with the Asset Bundle</span></span>
4. <span data-ttu-id="945b1-135">若要更快速地進行反復專案，請取消核取 **Android 的組建套件？**。</span><span class="sxs-lookup"><span data-stu-id="945b1-135">For faster iteration, uncheck the **Build Kit for Android?**.</span></span> <span data-ttu-id="945b1-136">請記得在您完成反覆運算或想要與套件共用/功能時，建立並上傳 Android 版。</span><span class="sxs-lookup"><span data-stu-id="945b1-136">Remember to build and upload a version for Android later when you're done iterating or want to share/feature your Kit.</span></span> 
5. <span data-ttu-id="945b1-137">選取 **載入套件預製專案目錄**</span><span class="sxs-lookup"><span data-stu-id="945b1-137">Select **Load Kit Prefab Directories**</span></span>
6. <span data-ttu-id="945b1-138">選擇符合套件資料夾名稱的 [ **組建** ]。</span><span class="sxs-lookup"><span data-stu-id="945b1-138">Choose **Build** next to the one matching your Kit Folder Name.</span></span> <span data-ttu-id="945b1-139">通常會從相同的 Unity 專案產生多個套件。</span><span class="sxs-lookup"><span data-stu-id="945b1-139">It's common to produce multiple Kits from the same Unity project.</span></span> <span data-ttu-id="945b1-140">這可能需要一些時間，視您的套件大小而定。</span><span class="sxs-lookup"><span data-stu-id="945b1-140">This may take a while depending on the size of your Kit.</span></span> <span data-ttu-id="945b1-141">完成時，包含 zip 檔案的資料夾將會自動開啟。</span><span class="sxs-lookup"><span data-stu-id="945b1-141">When it's done, the folder containing your zip file will open automatically.</span></span> 
7. <span data-ttu-id="945b1-142">移至網站，編輯您稍早建立的套件，然後上傳您所產生的 zip 檔案。</span><span class="sxs-lookup"><span data-stu-id="945b1-142">Go to the website, edit the Kit you created earlier, and upload the zip file you produced.</span></span> <span data-ttu-id="945b1-143">視檔案大小而定，此上傳可能需要一段時間。</span><span class="sxs-lookup"><span data-stu-id="945b1-143">This upload may take a while depending on the file size.</span></span>
    * <span data-ttu-id="945b1-144">如果成功，您會在左側的「上傳」檔案大小、電腦和 Android，以及上次更新時間</span><span class="sxs-lookup"><span data-stu-id="945b1-144">If successful, you’ll see on the left side under “Uploads” the file sizes and for PC and Android and when they were last updated</span></span>
    * <span data-ttu-id="945b1-145">如果不成功，請確定您沒有任何腳本，我們不支援腳本，我們會檢查這些腳本是否有安全性，然後再試一次。</span><span class="sxs-lookup"><span data-stu-id="945b1-145">If unsuccessful, make sure you don't have any scripts, we don't support scripts, we check for those for security and try again.</span></span>

<span data-ttu-id="945b1-146">恭喜！</span><span class="sxs-lookup"><span data-stu-id="945b1-146">Congratulations!</span></span> <span data-ttu-id="945b1-147">您已經準備好使用自己的套件建立世界！</span><span class="sxs-lookup"><span data-stu-id="945b1-147">You're ready to build Worlds with your own Kit!</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="945b1-148">疑難排解</span><span class="sxs-lookup"><span data-stu-id="945b1-148">Troubleshooting</span></span> 

<span data-ttu-id="945b1-149">**有任何限制嗎？**</span><span class="sxs-lookup"><span data-stu-id="945b1-149">**Are there limits?**</span></span>
<span data-ttu-id="945b1-150">但不會有任何硬性限制，但請記住，即使只有一個成品，使用者仍需要針對整個套件下載其平臺的 AssetBundle。</span><span class="sxs-lookup"><span data-stu-id="945b1-150">There are no hard limits yet but remember that users need to download the AssetBundle for their platform for the entire Kit even if only one Artifact is used.</span></span> <span data-ttu-id="945b1-151">請嘗試將每個平臺的下載保持在 5 MB 以下。</span><span class="sxs-lookup"><span data-stu-id="945b1-151">Try to keep the download per-platform to 5 MB or less.</span></span> <span data-ttu-id="945b1-152">其中一種方法是將專案分割成較小的套件。</span><span class="sxs-lookup"><span data-stu-id="945b1-152">One way to do that is to split up things into smaller Kits.</span></span> <span data-ttu-id="945b1-153">例如，200 .props 應該以半個分割。</span><span class="sxs-lookup"><span data-stu-id="945b1-153">For example, 200 props should split in half.</span></span> 

<span data-ttu-id="945b1-154">**看到「分割眼睛」？**</span><span class="sxs-lookup"><span data-stu-id="945b1-154">**Seeing “split eye”?**</span></span>
<span data-ttu-id="945b1-155">重新匯入最新的上載者以取得正確的轉譯設定</span><span class="sxs-lookup"><span data-stu-id="945b1-155">Reimport the latest Uploader to get the right rendering settings</span></span>

<span data-ttu-id="945b1-156">**更新/變更未反映？**</span><span class="sxs-lookup"><span data-stu-id="945b1-156">**Updates/changes not reflected?**</span></span>
    * <span data-ttu-id="945b1-157">查看套件頁面上的更新時間</span><span class="sxs-lookup"><span data-stu-id="945b1-157">Check the updated time on the Kit page</span></span>
    * <span data-ttu-id="945b1-158">重新進入世界將無法運作--重新開機用戶端。</span><span class="sxs-lookup"><span data-stu-id="945b1-158">Reentering the World will not work-- restart client.</span></span> <span data-ttu-id="945b1-159">甚至可能需要幾分鐘的時間才會更新</span><span class="sxs-lookup"><span data-stu-id="945b1-159">Even then it may take a few minutes to update</span></span>
    * <span data-ttu-id="945b1-160">請確定您的資料夾名稱或預製專案名稱中沒有空格 **，例如「party_favors」與**「合作物件喜好」</span><span class="sxs-lookup"><span data-stu-id="945b1-160">Make sure there are no spaces in your folder names or prefab names **for example, 'party_favors' vs 'party favors'**</span></span>

<span data-ttu-id="945b1-161">**它會持續說我有腳本，但是我不** 會AssetBundle 瀏覽器有時會自動包含檔案。</span><span class="sxs-lookup"><span data-stu-id="945b1-161">**It keeps saying I have a script but I don't** The AssetBundle Browser automatically includes files sometimes.</span></span> <span data-ttu-id="945b1-162">請嘗試隔離您所攜帶的模型。</span><span class="sxs-lookup"><span data-stu-id="945b1-162">Try to isolate the model you're bringing in.</span></span> <span data-ttu-id="945b1-163">例如，不要將它拖曳到另一個預製專案的一部分。</span><span class="sxs-lookup"><span data-stu-id="945b1-163">For example, don't drag it in when it's part of another Prefab already</span></span>

<span data-ttu-id="945b1-164">**物件和動畫的意義為何？**</span><span class="sxs-lookup"><span data-stu-id="945b1-164">**What about Particle Systems and Animations?**</span></span>
<span data-ttu-id="945b1-165">在這些情況下，會在 1x1x1 Cube 下放置，並停用網格轉譯和碰撞。</span><span class="sxs-lookup"><span data-stu-id="945b1-165">For these, next them under a 1x1x1 Cube positioned at the origin with Mesh Rendering and Collision disabled.</span></span> <span data-ttu-id="945b1-166">物件應已啟用迴圈，並應將 **縮放比例** 設定 **為階層，以便** 我們可以在 Altspace 中適當地進行調整。</span><span class="sxs-lookup"><span data-stu-id="945b1-166">Particle Systems should have looping enabled and **Scaling** should be set to **Hierarchy** so that we can scale them in Altspace properly.</span></span> <span data-ttu-id="945b1-167">在產生所有動畫的 prefabs 之後，請針對每個動畫停用 **衝突** 物件的衝突。</span><span class="sxs-lookup"><span data-stu-id="945b1-167">After you generate the prefabs for all the animations, disable the collisions on the **collision** objects for each.</span></span>

<span data-ttu-id="945b1-168">**構件很暗** 您是否將模型的材質著色器設定為 **僅限行動/頂點的方向燈**？</span><span class="sxs-lookup"><span data-stu-id="945b1-168">**The Artifacts are dark** Did you set the model's material shader to **Mobile/Vertex lit-only directional lights**?</span></span>

<span data-ttu-id="945b1-169">成品 **未面對正確的方式** 旋轉 **模型** 和 **碰撞**，並更新預製專案。</span><span class="sxs-lookup"><span data-stu-id="945b1-169">**The Artifact isn't facing the right way** Rotate the **model** and **collider** and update the Prefab.</span></span> <span data-ttu-id="945b1-170">旋轉父系不會進行任何動作，而是會忽略該動作。</span><span class="sxs-lookup"><span data-stu-id="945b1-170">Rotating the parent won't do anything--that's ignored.</span></span> <span data-ttu-id="945b1-171">您可以使用 [ **旋轉覆寫** ] 欄位來輕鬆執行此動作。</span><span class="sxs-lookup"><span data-stu-id="945b1-171">You can use the **Rotation Override** field to do this easily.</span></span>

<span data-ttu-id="945b1-172">**這些成品可以搭配 SDK 的 **CreateFromLibrary** 函式使用嗎？**</span><span class="sxs-lookup"><span data-stu-id="945b1-172">**Can these Artifacts be used with the SDK's **CreateFromLibrary** function?**</span></span>
<span data-ttu-id="945b1-173">是</span><span class="sxs-lookup"><span data-stu-id="945b1-173">Yes</span></span>