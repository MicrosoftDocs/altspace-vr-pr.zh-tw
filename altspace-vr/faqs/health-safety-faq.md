---
title: 健全狀況和安全性的常見問題
description: 對健康情況和安全性相關問題的疑難排解和支援。
ms.date: 8/16/2021
author: qianw211
ms.author: v-qianwen
ms.topic: article
keywords: vr、AlspaceVR、疑難排解、支援、健康情況、安全性、以 VR 縮減 nausea
ms.openlocfilehash: fb4a6c020857bc393ea7367b6b5c71b94bd4f948
ms.sourcegitcommit: 5c452a9092297c0bfbc8efabebf395e7ee31853f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/30/2021
ms.locfileid: "129311852"
---
# <a name="frequently-asked-questions-on-health-and-safety"></a>健全狀況和安全性的常見問題

## <a name="why-do-some-people-feel-ill-in-vr"></a>為什麼某些人覺得在 VR 中不正確？

所有的 VR 都會導致 vertigo 和 nausea。 問題源自于您的眼睛之間的差異，以及內部 ear 如何傳送至您的大腦。 當您的眼睛偵測到移動時，您的耳也會傳達您仍在使用的情況下，有些人的大腦可能會因引發 dizziness 和 nausea 而有反應。 有些人更容易使用運動 sickness，可能會對此現象造成更大的影響，而其他人可能不會有問題。 

硬體層級有幾件事，還有一些 AltspaceVR 的軟體會在 VR 中大幅減少或完全排除 nausea 引發的動作。

## <a name="hardware-based-nausea-reduction"></a>以硬體為基礎的 nausea 縮減

像是 Oculus Rift 和 HTC Vive 這類的現代的 VR 硬體，藉由以消除可能導致 nausea 的延遲率來呈現影片畫面，來減少運動 sickness。 如果軟體已優化，而 AltspaceVR 為，則當您在 VR 中開啟標頭時，將不會有任何延遲。 HMD 中的加速計會以更快的速度來傳達移動和傳輸該遙測，而人類眼可以偵測到任何延遲。 在使用位置攝影機科系的 HMD 模型上，這會更進一步，不僅會呈現旋轉的移動，也是橫向 (側邊) 的動作。

## <a name="software-based-nausea-reduction"></a>以軟體為基礎的 nausea 縮減

除了硬體改良和 framerates 之外，AltspaceVR 還實行了幾項功能，可協助人們減少和消除 nausea：

* **Teleporting** -立即從點對點移動不會將動作傳達給大腦，藉此消除 sickness 的動作。
* AltspaceVR 所有硬體的嵌入式 **管理單元**，在 VR 中提供「ratcheted」或「逐步」旋轉的意思。 換句話說，當您開啟時，您的視圖會旋轉大約20度的旋轉。 同樣地，這不會在大部分的人中觸發 nausea。
* **貼齊動作** -在特定硬體上，在觸控板上向前輕量會在不觸發運動 sickness 的遞增中向前移動透視。 
 
## <a name="how-to-eliminate-motion-sickness"></a>如何消除動作 sickness

**獨立式**

試著不要使用控制器來移動太多，只是在 VR 中旋轉您的前端/或向上/向下尋找。

**請勿使用滑鼠/KB 或控制器**

AltspaceVR 可讓使用者選擇使用標準遊戲週邊設備（例如滑鼠/鍵盤和遊戲控制器）在 VR 中移動，就像在視頻遊戲中一樣。 這包括多方向移動、strafing 和 turbo 按鈕。 我們建議您只在習慣採用 VR 之後才使用這些功能。 就算如此，還是會變慢。

**您可以隨時退出**

如果您遇到 nausea，請立即移除您的 HMD。 重新取得您的均衡、平靜您的 stomach，以及準備好返回 VR 環境。 請嘗試記住造成刺痛的移動，並避免重複。

**知道何時結束 VR**

最重要的是，知道何時需要休息。 您知道您的內文，並在為您提供強指示，指出有問題，請聆聽。 拿出中斷並取得一些空氣。 四處解說並重新調整您的均衡。 同樣地，請回頭看看，我們相信這一方仍會繼續進行。

## <a name="support"></a>支援

AltspaceVR 團隊的問題或意見反應？ 

> [!div class="nextstepaction"]
> [按一下這裡以傳送支援要求](https://help.altvr.com/hc/requests/new)