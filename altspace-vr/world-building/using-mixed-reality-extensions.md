---
title: 使用混合現實擴充功能
description: 瞭解如何使用混合現實延伸模組並進行疑難排解，以擴充及調整您的 AltspaceVR 世界。
ms.date: 03/11/2021
ms.topic: article
keywords: 混合的現實、延伸模組、疑難排解
ms.openlocfilehash: 1439ca76eaf4e0235c6552d037e55b6151e08407871bf470b3011b6cf8cbccd5
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "119125352"
---
# <a name="using-a-mixed-reality-extension"></a>使用混合現實擴充功能

[混合現實延伸](https://developer.altvr.com/) 模組 (MREs) 是您可以在世界中使用的應用程式，從 [頭盔](https://account.altvr.com/mres/1173667287173955931) 到工作中的 [Stargate](https://account.altvr.com/mres/1152987031857529562)。 這就是使用程式設計經驗的社區成員可以擴充 Altspace，而單向世界產生器可以讓他們的世界更具互動性。 雖然世界上的任何人都可以使用 MREs，但只有全球大樓的人員能夠在世界各地流覽和產生 MREs。 

1. 流覽 [網站](https://account.altvr.com/mres)的 [深入] 區段。 根據預設，您會看到自己的 MREs，因此請選取 [ **Altspace** ] 以查看官方 MREs 和 **精選** ，以查看來自社區的 MREs。 在您的世界中使用之前，先熟悉任何深入。 
2. 流覽至 [ [頭盔](https://account.altvr.com/mres/1173667287173955931) ] 深入，然後選取 [ **複製到剪貼** 簿]。 
3. 輸入您的世界，並開啟「世界編輯器」以 **> SDK 應用程式的基本概念**。 將頭盔的 URL 貼到 [目標 URI] 欄位中，然後選取 [ **確認**]。 深入物件應該會出現，並嘗試連線到在雲端中執行的深入。 您現在應該會看到您可以按一下的一些頭盔。
4. 移動/旋轉或調整深入的方式，就像是任何其他世界物件一樣。

恭喜！ 您目前使用的是 MREs--您太酷了！

## <a name="troubleshooting"></a>疑難排解

**深入正在顯示哭表情** 
    * 確認 URL 是否正確
    * 切換為物件上的 [**現正播放**] 選項，然後選擇 [**確認**]
    * 嘗試重新進入

**深入為延遲** 視裝載深入的位置而定，您可能會遇到一些網路延遲

**為什麼需要貼上 Url？**
未來，您可以像從套件 Artifacts 一樣來管理和產生 MREs。 在那之前，我們將繼續使用 Url