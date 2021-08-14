---
title: 尋找 AltspaceVR 應用程式版本
description: 瞭解如何使用 AltspaceVR 應用程式、設定和用戶端記錄來尋找您目前正在執行的 AltspaceVR 版本。
ms.date: 02/10/2021
ms.topic: article
keywords: 應用程式版本
ms.openlocfilehash: fbf67a8302a67ddb916772420949cf0509a0d4a60c472711975c651862438b93
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "119128238"
---
# <a name="finding-the-altspacevr-app-version"></a>尋找 AltspaceVR 應用程式版本

在針對問題進行疑難排解的過程中，系統可能會詢問您目前正在執行的 AltspaceVR 應用程式版本。

## <a name="in-altspacevr"></a>在 AltspaceVR 中

若要在 AltspaceVR 中尋找應用程式版本，請流覽至 [ **設定] 功能表** ，並在左側導覽列中選取 [ **關於** ]。 這裡會報告 [應用程式版本]，如下列螢幕擷取畫面所示。

![開啟時開啟的 [關於] 面板開啟的設定功能表](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a>在 Windows 系統設定

如果您是透過 Microsoft Store 安裝 AltspaceVR，您可以在 Windows 系統設定中另外尋找應用程式版本。  如果您無法成功登入用戶端，此案例適合用來報告應用程式版本。

若要在 Windows 系統設定中尋找應用程式版本，請開啟 [**開始] 功能表**，輸入 **應用程式 & 功能**，然後選取結果。 流覽至應用程式清單中的 **AltspaceVR** 。 以滑鼠左鍵按一下 [AltspaceVR]，然後從出現的功能表中選取 [ **Advanced Options** ]。

![[應用程式和功能] 功能表開啟時已醒目提示 [advanced] 選項](images/app-version-img-02.png)

在 [ **Advanced] 選項** 的 [ **規格** ] 標頭下， **應用程式版本** 應該會列在 [ **版本** ] 標籤的右邊。

![醒目提示應用程式版本開啟的 Advanced options](images/app-version-img-03.png)

## <a name="in-client-logs"></a>在用戶端記錄中

AltspaceVR 會在應用程式啟動期間，將用戶端記錄檔中的應用程式版本報告為「Altspace 版本」。 如果您無法成功登入用戶端，但它在失敗之前嘗試啟動，這會是取得應用程式版本的絕佳選項。

## <a name="windows"></a>Windows

在 Windows 上，您可以透過 Windows 檔案總管找到用戶端記錄檔：

```
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player.log
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player-prev.log
```

每次啟動 AltspaceVR 時，都會覆寫此檔案。 ' Player. log ' 代表您最新的會話，而 ' Player-prev ' 代表前一個會話。

## <a name="via-powershell"></a>透過 PowerShell

Advanced users 可以透過 PowerShell 搜尋此字串的用戶端記錄檔，如下所示：

輸入：

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

輸出：

[2.047] AltspaceVR 版本： 3.2.23. e66c2