---
title: 授與世界角色
description: 瞭解角色和能力系統，並取得在您的 AltspaceVR 領域中提供使用者角色的逐步指示。
ms.date: 03/11/2021
ms.topic: article
keywords: 角色
ms.openlocfilehash: f8cd55fbd8ede6cedd199724a3e6b2413c5bc3e6
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212201"
---
# <a name="granting-world-roles"></a><span data-ttu-id="fe2a6-104">授與世界角色</span><span class="sxs-lookup"><span data-stu-id="fe2a6-104">Granting world roles</span></span>

<span data-ttu-id="fe2a6-105">Altspace 具有角色和能力系統。</span><span class="sxs-lookup"><span data-stu-id="fe2a6-105">Altspace has a Roles and Abilities system.</span></span> <span data-ttu-id="fe2a6-106">每個人都可以有多個角色，而其角色可能會根據其所在位置而有所不同。</span><span class="sxs-lookup"><span data-stu-id="fe2a6-106">Each person can have multiple roles and their roles can be different depending on where they are.</span></span> <span data-ttu-id="fe2a6-107">每個角色接著會提供一或多個功能。</span><span class="sxs-lookup"><span data-stu-id="fe2a6-107">Each role, in turn, gives you one or more abilities.</span></span> <span data-ttu-id="fe2a6-108">例如，當您在自己的活動中時，您會自動收到展示者和 **仲裁\*\*\*\*者** 角色。</span><span class="sxs-lookup"><span data-stu-id="fe2a6-108">For example, when you're in your own event, you automatically receive the **presenter** and **moderator** roles.</span></span> <span data-ttu-id="fe2a6-109">有了這兩個角色，您就可以開始失去規則使用者，在階段也可能釋出紙屑。</span><span class="sxs-lookup"><span data-stu-id="fe2a6-109">With those two roles you can kick unruly users, be on stage, and maybe release the confetti.</span></span> 

1. <span data-ttu-id="fe2a6-110">**在 [VR** ] 區段中編輯您的世界， ([如何管理世界](managing-worlds.md)) </span><span class="sxs-lookup"><span data-stu-id="fe2a6-110">Edit your World and scroll down to the **In VR** section ([How to manage Worlds](managing-worlds.md))</span></span>

![在全球的 VR 區段中變更角色](images/granting-roles.png)

2. <span data-ttu-id="fe2a6-112">如果您想要將特定角色授與給此世界的特定使用者，請編輯 [ **角色** ] 欄位。</span><span class="sxs-lookup"><span data-stu-id="fe2a6-112">Edit the **Roles** field if you want to grant specific roles to specific users just for this World.</span></span> <span data-ttu-id="fe2a6-113">例如，如果您想要提供給我的展示 **者**  +  **仲裁** 者，並為 Calen **仲裁** 者提供，您可以新增下列各項，然後選取 [**儲存**]。</span><span class="sxs-lookup"><span data-stu-id="fe2a6-113">For example, if you want to give me **presenter** + **moderator** and give Calen **moderator**, you would add the following and select **Save**.</span></span> <span data-ttu-id="fe2a6-114">每一行的格式為 **{role}、{username 或 email}** 。</span><span class="sxs-lookup"><span data-stu-id="fe2a6-114">The format is **{role},{username or email}** on each line.</span></span> <span data-ttu-id="fe2a6-115">使用者名稱不區分大小寫。</span><span class="sxs-lookup"><span data-stu-id="fe2a6-115">Username is case-insensitive.</span></span> 

```
presenter,jimmy
moderator,jimmy
moderator,calen
```

3. <span data-ttu-id="fe2a6-116">如果您再次選取 [ **編輯** ]，您應該會在 [角色] 欄位上方看到下列。</span><span class="sxs-lookup"><span data-stu-id="fe2a6-116">If you select **Edit** again, you should see the following above the Roles field.</span></span> <span data-ttu-id="fe2a6-117">這就是您知道在資料庫中更新的方式。</span><span class="sxs-lookup"><span data-stu-id="fe2a6-117">That's how you know updated in the database.</span></span>

```
Presenters: jimmy
Moderators: jimmy,calen
```

* <span data-ttu-id="fe2a6-118">為了讓變更在 Altspace 生效，您應該重設世界，強制所有人重新加入。</span><span class="sxs-lookup"><span data-stu-id="fe2a6-118">In order for the change to take effect in Altspace, you should reset the world, forcing everyone to rejoin.</span></span> <span data-ttu-id="fe2a6-119">以下是完整的角色清單。</span><span class="sxs-lookup"><span data-stu-id="fe2a6-119">There's a full list of roles below.</span></span>

4. <span data-ttu-id="fe2a6-120">如果您想要將角色授與給每個加入您世界的角色，請編輯內容 **相關角色** 欄位。</span><span class="sxs-lookup"><span data-stu-id="fe2a6-120">Edit the **Contextual Roles** field if you want to grant a role to every one that joins your World.</span></span> <span data-ttu-id="fe2a6-121">例如，如果您想要讓人們飛出並使用擴音器，讓他們可以聽到彼此的聲音，請新增下列內容：</span><span class="sxs-lookup"><span data-stu-id="fe2a6-121">For example, if you want to let people fly and use the megaphone so they can hear each other while far part, add the following:</span></span>

```
pilot,megaphone_only
```

<span data-ttu-id="fe2a6-122">選取 [ **更新**] 之後，請重設世界。</span><span class="sxs-lookup"><span data-stu-id="fe2a6-122">After you select **Update**, reset the World.</span></span> <span data-ttu-id="fe2a6-123">這只會影響此世界。</span><span class="sxs-lookup"><span data-stu-id="fe2a6-123">This will only affect this World.</span></span> <span data-ttu-id="fe2a6-124">如果您想要將角色授與整個 Universe，請在 Universe 上編輯相同的欄位。</span><span class="sxs-lookup"><span data-stu-id="fe2a6-124">If you want to grant roles to an entire Universe, edit the same fields on the Universe.</span></span> 

## <a name="roles"></a><span data-ttu-id="fe2a6-125">角色</span><span class="sxs-lookup"><span data-stu-id="fe2a6-125">Roles</span></span> 

* <span data-ttu-id="fe2a6-126">展示 **者** 功能，例如能夠在階段</span><span class="sxs-lookup"><span data-stu-id="fe2a6-126">**Presenter** - abilities like being able to be on stage</span></span>
* <span data-ttu-id="fe2a6-127">**仲裁** 者的能力 **，像是** 開始維護 decorum</span><span class="sxs-lookup"><span data-stu-id="fe2a6-127">**Moderator** - abilities like **kick** to maintain decorum</span></span>
* <span data-ttu-id="fe2a6-128">**Terraformer** -使用世界編輯器的能力</span><span class="sxs-lookup"><span data-stu-id="fe2a6-128">**Terraformer** - ability to use the World Editor</span></span>
* <span data-ttu-id="fe2a6-129">**試驗** -切換即時模式並產生6DOF 航班工具的能力</span><span class="sxs-lookup"><span data-stu-id="fe2a6-129">**Pilot** - ability to toggle fly mode and spawn the 6DOF flight tool</span></span>
* <span data-ttu-id="fe2a6-130">**Megaphone_only** 能夠在世界各地對使用者的耳說出什麼</span><span class="sxs-lookup"><span data-stu-id="fe2a6-130">**Megaphone_only** - ability to speak into users' ears wherever they are in the World</span></span>
* <span data-ttu-id="fe2a6-131">**Showcase_new_sdk** 能夠產生深入 sdk 應用程式</span><span class="sxs-lookup"><span data-stu-id="fe2a6-131">**Showcase_new_sdk** - ability to spawn MRE SDK apps</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="fe2a6-132">疑難排解</span><span class="sxs-lookup"><span data-stu-id="fe2a6-132">Troubleshooting</span></span>

<span data-ttu-id="fe2a6-133">**我可以刪除角色嗎？**</span><span class="sxs-lookup"><span data-stu-id="fe2a6-133">**Can I delete roles?**</span></span>
<span data-ttu-id="fe2a6-134">從現在的表單中，請在 help.altvr.com 提出支援要求，我們會為您處理</span><span class="sxs-lookup"><span data-stu-id="fe2a6-134">Not from the form right now so file a Support request at help.altvr.com and we'll take care of it for you</span></span>

<span data-ttu-id="fe2a6-135">**當世界從另一個匯入時，是否複製了角色？**</span><span class="sxs-lookup"><span data-stu-id="fe2a6-135">**Are roles copied when a World is importing from another?**</span></span>
<span data-ttu-id="fe2a6-136">否，不復制角色</span><span class="sxs-lookup"><span data-stu-id="fe2a6-136">No, roles aren't copied</span></span>