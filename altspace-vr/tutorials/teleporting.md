---
title: 使用 teleporter
description: 瞭解如何使用 AltspaceVR 中的 teleporter，從某個事件或世界間移動到另一個活動或世界。
ms.date: 03/11/2021
ms.topic: article
keywords: teleporter
ms.openlocfilehash: afc199e958824bb5f0a9ff6d74865cbcd3f16868
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212509"
---
# <a name="using-the-teleporter"></a>使用 teleporter

從某個事件或世界傳送到另一個事件或世界，是讓您和您的小組探索 AltspaceVR 所提供之所有專案的絕佳方式。

## <a name="the-short-version"></a>簡短版本

![從編輯器面板 Teleporting 步驟以設定遙傳目的地](images/teleporter.png)

## <a name="the-slightly-longer-version"></a>稍長的版本

首先，請確定您是在 Homespace 中，在您已建立或已獲得 Terraformer 角色的事件或世界中。 如果您處於2D 模式，且看不到 UI 右下角的 [世界編輯器] 按鈕，請以滑鼠右鍵按一下滑鼠按鍵，開啟/關閉。 如果您仍然看不到 [World 編輯器] 按鈕，您可能會在其他人的空間中。 如果是這種情況，請要求主機提供 Terraformer 角色。

它也有助於： 
1. 先建立事件或世界
2. 移至您想要產生 Teleporter 的位置，讓您的活動/世界將填入 [Teleporter 目的地] 面板中，讓您更快速且更輕鬆地連接它們。

另一個可協助您以2D 模式流覽 Teleporters 的技巧是使用 Ctrl + 空格鍵。 它會顯示命令提示字元，您可以輸入： back，這會帶您回到您的最後一個空間！ 

現在移至您想要產生 Teleporter 的位置，然後選取 [世界編輯器]/[編輯器] 面板/[基本]/[Teleporter]。

這會顯示 [Teleporter 目的地] 面板。 您會看到三個可供選擇的類別：

* **我的空間** -您所建立的世界清單。
* **最近** 的清單：最近的活動清單。 如果您想要移動至某個事件，請使用此選項。這是唯一將您帶到事件的選項，其他2則只讓您在世界間移動。 注意：如果您要連接已匯入之世界的 Front Row 事件，請參閱下方的 Advanced，您必須在匯入的世界中產生並設定 Teleporters，而不是在實際的事件中。
* **精選** 清單：您可以將 Teleporter 設定為旅遊的精選領域。

選取您要使用的事件或世界，這會產生 Teleporter，並將事件或世界名稱的文字標籤稍微落後。 因此，您可以選取 [目前物件] 區段中的齒輪圖示來變更標籤名稱。

您可以在 Teleporter 上選取游標 (系統會詢問您是否可以在該處進行 misclick，以防它是) ，或將您的頭像移至 Teleporter，presto，您會前往目的地。 告訴我們大家好！

## <a name="advanced-features"></a>進階功能

如果您要使用 Front Row 與自訂世界 (例如，基礎世界、Unity 上傳空間範本、Re-Import 世界) 來建立會議、峰會或大型活動，您必須在基礎世界中設定 Teleporter，而不是在實際的活動中設定。 確定您正在設定 Teleporter 來移動到正確的事件 (必須來自您的基礎世界中的最新清單) ，然後在事件中 Re-Import 世界，讓 Teleporters 顯示在所有的 Front Row 事件空間中。

## <a name="faqs"></a>常見問題集

**錯誤： ' 抱歉，我們想要，但我們無法讓您在這裡**

事件可能會有附加的群組，因此只有群組中的使用者名稱可以進入該 Teleporter，以取得該私用群組事件。

**我可以在一個空間中使用多少 teleporters？**

Teleporters 使用具有動畫物件效果的透明紋理，因此最好不要在相同的點/重迭中使用太多，因為這可能會影響效能。 如果在您的空間中全部分散，請嘗試在相同區域中不超過4個，或超過10個。