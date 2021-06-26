---
title: 授與世界角色
description: 瞭解角色和能力系統，並取得在您的 AltspaceVR 領域中提供使用者角色的逐步指示。
ms.date: 04/14/2021
ms.topic: article
keywords: 角色
ms.openlocfilehash: 3a1d0f138b29fe545f52d851ff00062f156a860e
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923188"
---
# <a name="granting-world-roles"></a><span data-ttu-id="ba27d-104">授與世界角色</span><span class="sxs-lookup"><span data-stu-id="ba27d-104">Granting world roles</span></span>

<span data-ttu-id="ba27d-105">Altspace 具有角色和能力系統。</span><span class="sxs-lookup"><span data-stu-id="ba27d-105">Altspace has a Roles and Abilities system.</span></span> <span data-ttu-id="ba27d-106">每個人都可以有多個角色，而其角色可能會根據其所在位置而有所不同。</span><span class="sxs-lookup"><span data-stu-id="ba27d-106">Each person can have multiple roles and their roles can be different depending on where they are.</span></span> <span data-ttu-id="ba27d-107">每個角色接著會提供一或多個功能。</span><span class="sxs-lookup"><span data-stu-id="ba27d-107">Each role, in turn, gives you one or more abilities.</span></span> <span data-ttu-id="ba27d-108">例如，當您在自己的活動中時，您會自動收到 **主機** 和 **仲裁** 者角色。</span><span class="sxs-lookup"><span data-stu-id="ba27d-108">For example, when you're in your own event, you automatically receive the **host** and **moderator** roles.</span></span> <span data-ttu-id="ba27d-109">有了這兩個角色，您就可以開始失去規則使用者，在階段也可能釋出紙屑。</span><span class="sxs-lookup"><span data-stu-id="ba27d-109">With those two roles you can kick unruly users, be on stage, and maybe release the confetti.</span></span>

1. <span data-ttu-id="ba27d-110">編輯您的世界，並查看內容 **相關角色** 的右欄， ([如何管理世界](managing-worlds.md)) </span><span class="sxs-lookup"><span data-stu-id="ba27d-110">Edit your World and look over to the right column for **Contextual Roles** ([How to manage Worlds](managing-worlds.md))</span></span>

![在世界上變更內容相關角色的角色](images/granting-roles.png)

2. <span data-ttu-id="ba27d-112">如果您想要將特定角色授與此世界的特定使用者，請按一下 [內容 **相關角色**] 欄位底下的 [**新增使用者**]。</span><span class="sxs-lookup"><span data-stu-id="ba27d-112">Click **Add User** under the **Contextual Roles** field if you want to grant specific roles to specific users just for this World.</span></span> <span data-ttu-id="ba27d-113">例如，如果您想要為我提供 **主機**  +  **仲裁** 者，請新增上述程式，然後選取 [**儲存**]。</span><span class="sxs-lookup"><span data-stu-id="ba27d-113">For example, if you want to give me **host** + **moderator**, you would add the above and select **Save**.</span></span> <span data-ttu-id="ba27d-114">格式為使用者 **名稱**，使用者名稱不區分大小寫，請從下拉式功能表 **Terraformer** 中選擇角色，然後按一下 [加入使用者] 多次以繼續加入更多使用者，然後按一下 [ **更新**]。</span><span class="sxs-lookup"><span data-stu-id="ba27d-114">The format is **username**, username is case-insensitive, choose the role from the dropdown menu **Terraformer**, click Add User multiple times to keeping adding more users and then click **Update**.</span></span>

* <span data-ttu-id="ba27d-115">為了讓變更在 Altspace 生效，您應該重設世界強制所有人重新加入的空間，或讓每位使用者都有新的角色重新加入世界。</span><span class="sxs-lookup"><span data-stu-id="ba27d-115">In order for the change to take effect in Altspace, you should Reset Space the world forcing everyone to rejoin or have each user with a new role rejoin the world.</span></span>

3. <span data-ttu-id="ba27d-116">如果您想要將角色授與給每個加入您世界的角色，請在 [VR] 區段 **中** 編輯 [**預設內容角色**] 欄位。</span><span class="sxs-lookup"><span data-stu-id="ba27d-116">Edit the **Default Contextual Roles** field, under the **In VR** section, if you want to grant a role to every one that joins your World.</span></span> <span data-ttu-id="ba27d-117">例如，如果您想要讓人們飛出並使用擴音器，讓他們可以聽到彼此的聲音，請新增下列內容：</span><span class="sxs-lookup"><span data-stu-id="ba27d-117">For example, if you want to let people fly and use the megaphone so they can hear each other while far part, add the following:</span></span>

```
pilot,megaphone_only
```

<span data-ttu-id="ba27d-118">選取 [ **更新**] 之後，請重設世界中的空間。</span><span class="sxs-lookup"><span data-stu-id="ba27d-118">After you select **Update**, Reset Space in the World.</span></span> <span data-ttu-id="ba27d-119">這只會影響此世界。</span><span class="sxs-lookup"><span data-stu-id="ba27d-119">This will only affect this World.</span></span> <span data-ttu-id="ba27d-120">如果您想要將角色授與整個 Universe，請在 Universe 上編輯相同的欄位。</span><span class="sxs-lookup"><span data-stu-id="ba27d-120">If you want to grant roles to an entire Universe, edit the same fields on the Universe.</span></span> <span data-ttu-id="ba27d-121">事件的相同之處，如果您希望事件中的每個人都擁有這些角色，您必須將此專案新增至事件本身的 **預設 Contexual 角色** 。</span><span class="sxs-lookup"><span data-stu-id="ba27d-121">The same goes for events, if you want everyone in your event to have these roles you'll need to add this to the **Default Contexual Roles** of the event itself.</span></span>

## <a name="roles"></a><span data-ttu-id="ba27d-122">角色</span><span class="sxs-lookup"><span data-stu-id="ba27d-122">Roles</span></span>

* <span data-ttu-id="ba27d-123">**Megaphone_only** 能夠在世界各地對使用者的耳說出什麼</span><span class="sxs-lookup"><span data-stu-id="ba27d-123">**Megaphone_only** - ability to speak into users' ears wherever they are in the World</span></span>
* <span data-ttu-id="ba27d-124">**仲裁** 者的能力 **，像是** 開始維護 decorum</span><span class="sxs-lookup"><span data-stu-id="ba27d-124">**Moderator** - abilities like **kick** to maintain decorum</span></span>
* <span data-ttu-id="ba27d-125">**試驗** -切換即時模式並產生6DOF 航班工具的能力</span><span class="sxs-lookup"><span data-stu-id="ba27d-125">**Pilot** - ability to toggle fly mode and spawn the 6DOF flight tool</span></span>
* <span data-ttu-id="ba27d-126">**主機** 能力，例如能夠在階段進行，擴音器</span><span class="sxs-lookup"><span data-stu-id="ba27d-126">**Host** - abilities like being able to be on stage, have megaphone</span></span>
* <span data-ttu-id="ba27d-127">**Terraformer** -在 [事件、世界、群組及 AltspaceVR 中](../getting-started/roles.md) 使用 (角色的詳細資訊，讓您能夠使用世界編輯器) </span><span class="sxs-lookup"><span data-stu-id="ba27d-127">**Terraformer** - ability to use the World Editor More information about ([Roles in events, worlds, groups, and in AltspaceVR](../getting-started/roles.md))</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="ba27d-128">疑難排解</span><span class="sxs-lookup"><span data-stu-id="ba27d-128">Troubleshooting</span></span>

<span data-ttu-id="ba27d-129">**我可以刪除角色嗎？**</span><span class="sxs-lookup"><span data-stu-id="ba27d-129">**Can I delete roles?**</span></span>
<span data-ttu-id="ba27d-130">是，請編輯您的世界，按一下您想要刪除的角色下方的 [**移除**]，然後按一下 [**更新**]。</span><span class="sxs-lookup"><span data-stu-id="ba27d-130">Yes, edit your world, click **Remove** below the role you'd like to delete and click **Update**</span></span>

<span data-ttu-id="ba27d-131">**當世界從另一個匯入時，是否複製了角色？**</span><span class="sxs-lookup"><span data-stu-id="ba27d-131">**Are roles copied when a World is importing from another?**</span></span>
<span data-ttu-id="ba27d-132">否，不復制角色</span><span class="sxs-lookup"><span data-stu-id="ba27d-132">No, roles aren't copied</span></span>