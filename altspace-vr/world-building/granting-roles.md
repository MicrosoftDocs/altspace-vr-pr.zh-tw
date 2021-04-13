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
# <a name="granting-world-roles"></a>授與世界角色

Altspace 具有角色和能力系統。 每個人都可以有多個角色，而其角色可能會根據其所在位置而有所不同。 每個角色接著會提供一或多個功能。 例如，當您在自己的活動中時，您會自動收到展示者和 **仲裁****者** 角色。 有了這兩個角色，您就可以開始失去規則使用者，在階段也可能釋出紙屑。 

1. **在 [VR** ] 區段中編輯您的世界， ([如何管理世界](managing-worlds.md)) 

![在全球的 VR 區段中變更角色](images/granting-roles.png)

2. 如果您想要將特定角色授與給此世界的特定使用者，請編輯 [ **角色** ] 欄位。 例如，如果您想要提供給我的展示 **者**  +  **仲裁** 者，並為 Calen **仲裁** 者提供，您可以新增下列各項，然後選取 [**儲存**]。 每一行的格式為 **{role}、{username 或 email}** 。 使用者名稱不區分大小寫。 

```
presenter,jimmy
moderator,jimmy
moderator,calen
```

3. 如果您再次選取 [ **編輯** ]，您應該會在 [角色] 欄位上方看到下列。 這就是您知道在資料庫中更新的方式。

```
Presenters: jimmy
Moderators: jimmy,calen
```

* 為了讓變更在 Altspace 生效，您應該重設世界，強制所有人重新加入。 以下是完整的角色清單。

4. 如果您想要將角色授與給每個加入您世界的角色，請編輯內容 **相關角色** 欄位。 例如，如果您想要讓人們飛出並使用擴音器，讓他們可以聽到彼此的聲音，請新增下列內容：

```
pilot,megaphone_only
```

選取 [ **更新**] 之後，請重設世界。 這只會影響此世界。 如果您想要將角色授與整個 Universe，請在 Universe 上編輯相同的欄位。 

## <a name="roles"></a>角色 

* 展示 **者** 功能，例如能夠在階段
* **仲裁** 者的能力 **，像是** 開始維護 decorum
* **Terraformer** -使用世界編輯器的能力
* **試驗** -切換即時模式並產生6DOF 航班工具的能力
* **Megaphone_only** 能夠在世界各地對使用者的耳說出什麼
* **Showcase_new_sdk** 能夠產生深入 sdk 應用程式

## <a name="troubleshooting"></a>疑難排解

**我可以刪除角色嗎？**
從現在的表單中，請在 help.altvr.com 提出支援要求，我們會為您處理

**當世界從另一個匯入時，是否複製了角色？**
否，不復制角色