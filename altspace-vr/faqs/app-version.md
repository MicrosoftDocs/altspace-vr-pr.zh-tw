---
title: 尋找 AltspaceVR 應用程式版本
description: 瞭解如何使用 AltspaceVR 應用程式、設定和用戶端記錄來尋找您目前正在執行的 AltspaceVR 版本。
ms.date: 02/10/2021
ms.topic: article
keywords: 應用程式版本
ms.openlocfilehash: 5d503d3b89cd213696dd53616c5c7e3013aeef01
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212404"
---
# <a name="finding-the-altspacevr-app-version"></a><span data-ttu-id="4e82c-104">尋找 AltspaceVR 應用程式版本</span><span class="sxs-lookup"><span data-stu-id="4e82c-104">Finding the AltspaceVR app version</span></span>

<span data-ttu-id="4e82c-105">在針對問題進行疑難排解的過程中，系統可能會詢問您目前正在執行的 AltspaceVR 應用程式版本。</span><span class="sxs-lookup"><span data-stu-id="4e82c-105">In the course of troubleshooting an issue, you may be asked what version of the AltspaceVR app you're currently running.</span></span>

## <a name="in-altspacevr"></a><span data-ttu-id="4e82c-106">在 AltspaceVR 中</span><span class="sxs-lookup"><span data-stu-id="4e82c-106">In AltspaceVR</span></span>

<span data-ttu-id="4e82c-107">若要在 AltspaceVR 中尋找應用程式版本，請流覽至 [ **設定] 功能表** ，並在左側導覽列中選取 [ **關於** ]。</span><span class="sxs-lookup"><span data-stu-id="4e82c-107">To find the app version in AltspaceVR, navigate to the **settings menu** and select **About** in the left navigation bar.</span></span> <span data-ttu-id="4e82c-108">這裡會報告 [應用程式版本]，如下列螢幕擷取畫面所示。</span><span class="sxs-lookup"><span data-stu-id="4e82c-108">The 'App Version' is reported here, as shown in the screenshot below.</span></span>

![設定功能表開啟時開啟 [關於面板開啟]](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a><span data-ttu-id="4e82c-110">在 Windows 系統設定中</span><span class="sxs-lookup"><span data-stu-id="4e82c-110">In Windows System Settings</span></span>

<span data-ttu-id="4e82c-111">如果您是透過 Microsoft Store 安裝 AltspaceVR，您可以另外在 Windows 系統設定中尋找應用程式版本。</span><span class="sxs-lookup"><span data-stu-id="4e82c-111">If you installed AltspaceVR via the Microsoft Store, you can additionally find the app version in the Windows system settings.</span></span>  <span data-ttu-id="4e82c-112">如果您無法成功登入用戶端，此案例適合用來報告應用程式版本。</span><span class="sxs-lookup"><span data-stu-id="4e82c-112">This scenario is a good fit when reporting the app version if you're unable to successfully log into the client.</span></span>

<span data-ttu-id="4e82c-113">若要在 [Windows 系統設定] 中尋找應用程式版本，請開啟 [ **開始] 功能表**，輸入 **應用程式 & 功能**]，然後選取結果。</span><span class="sxs-lookup"><span data-stu-id="4e82c-113">To find the app version in Windows system settings, open the **Start Menu**, type in **Apps & Features**, and select the result.</span></span> <span data-ttu-id="4e82c-114">流覽至應用程式清單中的 **AltspaceVR** 。</span><span class="sxs-lookup"><span data-stu-id="4e82c-114">Navigate to **AltspaceVR** in the list of apps.</span></span> <span data-ttu-id="4e82c-115">以滑鼠左鍵按一下 [AltspaceVR]，然後從出現的功能表中選取 [ **Advanced Options** ]。</span><span class="sxs-lookup"><span data-stu-id="4e82c-115">Left-click AltspaceVR and select **Advanced Options** from the menu that appears.</span></span>

![[應用程式和功能] 功能表開啟時已醒目提示 [advanced] 選項](images/app-version-img-02.png)

<span data-ttu-id="4e82c-117">在 [ **Advanced] 選項** 的 [ **規格** ] 標頭下， **應用程式版本** 應該會列在 [ **版本** ] 標籤的右邊。</span><span class="sxs-lookup"><span data-stu-id="4e82c-117">In the **Advanced Options**, under the **Specifications** header, the **App Version** should be listed to the right of the **Version** label.</span></span>

![醒目提示應用程式版本開啟的 Advanced options](images/app-version-img-03.png)

## <a name="in-client-logs"></a><span data-ttu-id="4e82c-119">在用戶端記錄中</span><span class="sxs-lookup"><span data-stu-id="4e82c-119">In Client Logs</span></span>

<span data-ttu-id="4e82c-120">AltspaceVR 會在應用程式啟動期間，將用戶端記錄檔中的應用程式版本報告為「Altspace 版本」。</span><span class="sxs-lookup"><span data-stu-id="4e82c-120">AltspaceVR reports the app version in the client logs file as "Altspace Version" during application startup.</span></span> <span data-ttu-id="4e82c-121">如果您無法成功登入用戶端，但它在失敗之前嘗試啟動，這會是取得應用程式版本的絕佳選項。</span><span class="sxs-lookup"><span data-stu-id="4e82c-121">This would be a good option to get the app version if you can't successfully log into the client, but it did attempt to start before failing.</span></span>

## <a name="windows"></a><span data-ttu-id="4e82c-122">Windows</span><span class="sxs-lookup"><span data-stu-id="4e82c-122">Windows</span></span>

<span data-ttu-id="4e82c-123">在 Windows 上，您可以透過 Windows 檔案總管在下列位置找到用戶端記錄檔：</span><span class="sxs-lookup"><span data-stu-id="4e82c-123">On Windows, the client logs file can be found via Windows Explorer at:</span></span>

```
%userprofile%\appdata\locallow\altspacevr\altspacevr\Player.log
%userprofile%\appdata\locallow\altspacevr\altspacevr\Player-prev.log
```

<span data-ttu-id="4e82c-124">每次啟動 AltspaceVR 時，都會覆寫此檔案。</span><span class="sxs-lookup"><span data-stu-id="4e82c-124">This file is overwritten each time you launch AltspaceVR.</span></span> <span data-ttu-id="4e82c-125">' Player. log ' 代表您最新的會話，而 ' Player-prev ' 代表前一個會話。</span><span class="sxs-lookup"><span data-stu-id="4e82c-125">'Player.log' represents your latest session, and 'Player-prev.log' represents the previous session.</span></span>

## <a name="via-powershell"></a><span data-ttu-id="4e82c-126">透過 PowerShell</span><span class="sxs-lookup"><span data-stu-id="4e82c-126">Via PowerShell</span></span>

<span data-ttu-id="4e82c-127">Advanced users 可以透過 PowerShell 搜尋此字串的用戶端記錄檔，如下所示：</span><span class="sxs-lookup"><span data-stu-id="4e82c-127">Advanced users can search the client logs for this string via PowerShell as follows:</span></span>

<span data-ttu-id="4e82c-128">輸入：</span><span class="sxs-lookup"><span data-stu-id="4e82c-128">Input:</span></span>

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

<span data-ttu-id="4e82c-129">輸出：</span><span class="sxs-lookup"><span data-stu-id="4e82c-129">Output:</span></span>

<span data-ttu-id="4e82c-130">[2.047] AltspaceVR 版本： 3.2.23. e66c2</span><span class="sxs-lookup"><span data-stu-id="4e82c-130">[2.047] AltspaceVR Version: 3.2.23.e66c2</span></span>