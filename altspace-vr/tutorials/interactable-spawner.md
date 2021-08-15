---
title: 使用 Interactables Spawner
description: 瞭解如何建立、使用和自訂 interactables spawner，以將專案放在您的 AltspaceVR 空間中。
ms.date: 02/10/2021
ms.topic: article
keywords: spawner，互動，自訂
ms.openlocfilehash: abeddec5c2b50e0612db5efb6bc2e3c5bd9de4a8b67c50b19afee18b17c5e746
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127386"
---
# <a name="using-the-interactables-spawner"></a>使用 Interactables Spawner

Interactables Spawner 可讓您將互動專案放置在您的活動、世界或家庭空間中。 這項功能目前是 [早期存取程式](../world-building/early-access.md) 的一部分，除非您選擇透過主功能表，否則無法使用此功能。

> [!NOTE]
> 雖然我們繼續試驗這項功能，但請注意，產生太多 interactables 可能會影響您的環境或事件的效能。 

## <a name="creating-an-interactable"></a>建立互動

若要將物件轉換成互動物件：

1. 將物件放在您的空間中。
2. 然後，在 [物件] 清單中尋找專案，然後選取旁邊的 **齒輪圖示** 以開啟其設定：

![以反白顯示的物件清單開啟的世界編輯器](images/interactables-spawner-img-01.png)

在 [設定] 頁面上，您會看到新的 **[物件 spawner**] 核取方塊，用來將它設為互動物件。

1. 核取該方塊，然後選取 [ **確認**]。
2. 在編輯模式中，您可以四處移動物件在空間中的產生位置。
3. **離開編輯模式** 以啟用專案互動。

![在 AltspaceVR 應用程式中開啟的更新成品視窗](images/interactables-spawner-img-02.png)

## <a name="other-customizations"></a>其他自訂內容

當您返回 [ **物件 spawner]** 之後，當您回到該物件的屬性時，將會有額外的設定，可讓您套用至產生的物件行為。

> [!NOTE]
> 互動物件縮放：這會在物件被挑選時設定物件的小數位數，相較于「調整」，這是物件在第一次挑選之前出現在世界中的比例。

套件製作者可能會注意到，AltspaceVR 正在執行時對套件所做的變更，在您重新開機 AltspaceVR 之前將不會生效。

最近我們已在 [**一般設定**] 索引標籤下新增名為 [**重載世界套件**] 的按鈕。 按一下這個按鈕會導致 (您) 重新輸入空間，再次重載所有套件，這只會下載您在 AltspaceVR 時更新的新套件版本。

![在 AltspaceVR 應用程式中開啟適中設定面板](images/interactables-spawner-img-03.png)