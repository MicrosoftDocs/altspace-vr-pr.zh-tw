---
title: 使用多媒體主控台
description: 瞭解如何在 AltspaceVR 體驗中開始設定、發佈和控制多媒體主控台。
ms.date: 03/11/2021
ms.topic: article
keywords: 主控台，多媒體
ms.openlocfilehash: a24b3700f1687aed6bc00fd218aacd7cc12908e521af6239fac0ae97f48b4b9a
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127363"
---
# <a name="using-the-multimedia-console"></a>使用多媒體主控台

多媒體主控台是一種工具，可讓您在事件和世界中共用媒體。 您可以使用它來共用影像、簡報、投影片、livestreams、影片、播放清單等專案。 以下逐步指示說明如何使用多媒體主控台 **v 0.5.0 +**。 

## <a name="getting-started"></a>開始使用

開始使用多媒體主控台的程式分為兩個部分。  首先，您將使用入口網站來產生和發佈您在環境中放置之多媒體主控台會話的設定。  第二個是在您的環境中放置實際的多媒體主控台應用程式，並設定應該使用的設定程式碼。

### <a name="configuring-the-multimedia-console-with-the-web-portal"></a>使用入口網站設定多媒體主控台

1. 首先，您必須確定您的內容會在線上裝載，因為您將需要 URL。  (您可以將相片上傳至 altvr.com、線上裝載影片 .mp4 檔案，或使用 Dlive 即時串流連結： https://dlive.tv/yourlivestream) 
2. 流覽至多媒體主控台的入口網站，網址為： [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)
3. 您可以從入口網站產生和發佈多媒體主控台的設定。   (請參閱下文，以取得各種屬性) 的詳細資料。
4. 當您將媒體輸入媒體清單並設定 [一般] 設定之後，請選取應用程式右上方的 [發佈] 按鈕。
5. 發佈完成後，對話方塊會顯示兩個文字，讓您進入您所放置的多媒體主控台。
  
### <a name="placing-the-multimedia-console-in-your-environment"></a>將多媒體主控台放在您的環境中

1. 在 [ **世界編輯器] > 編輯器面板上，> SDK 應用程式 > 多媒體主控台**。  (不會移至 **> 基本 > SDK 應用程式的世界編輯器**，這適用于未註冊的應用程式。 )   
2. 將多媒體主控台定位到最適合您的空間和物件。
3. 按一下 [橙色編輯模式] 按鈕，即可退出編輯模式。
4. 系統會提示您提供 **媒體播放機擁有者嗎？** 如果您是此多媒體主控台會話的官方擁有者，請確認並繼續。  (其他許可角色也可供使用。 如需詳細清單，請參閱下方。 ) 
5. 選取 [是] 以確認您是主要主機。  
6. 對話方塊應該會出現，要求您從 web 入口網站輸入程式碼或有效的 JSON。  輸入入口網站中的兩個單字代碼，包括虛線，然後按 [確定]。  (JSON 是如下所述的 advanced 設定) 
7. 使用您在入口網站中建立的設定，會在幾秒後載入多媒體主控台。

### <a name="controlling-the-multimedia-console"></a>控制多媒體主控台

1. 輸入您的程式碼並完成設定程式之後，您會看到控制項按鈕顯示在媒體顯示下方。 
    * [**播放**] 會啟動媒體檢視器 (或在目前的專案重新開機（如果先前已停止）)  
    * **停止** 停止 media viewer，並隱藏目前的媒體。  
    * **下一個/** 上一個，跳到下一個或上一個媒體 
    * **x/x**  在 [媒體] 清單中顯示目前的索引，並可讓您跳到清單中的任何點
    * **Config** 允許從 web 入口網站重新進入新的程式碼，以在主控台中設定新的設定。 

現在您已經設定為透過多媒體主控台開始共用！  
 
## <a name="working-with-the-web-portal"></a>使用入口網站

入口網站是一種 web 應用程式，可讓您設定多媒體主控台的各種功能。  這些功能分為兩類：一般媒體主控台設定和媒體播放清單。

### <a name="multimedia-console-general-settings"></a>多媒體主控台的一般設定

**播放設定**

媒體清單的一般播放設定

* **迴圈媒體清單**-決定當您到達清單結尾時，媒體清單是否應迴圈。
* **啟動方法** -選取多媒體主控台應該啟動的方法。
    * 手動-等候在啟動媒體之前按下 [播放] 按鈕
    * 自動從開頭開始-自動從清單開頭開始進行媒體清單
    * 自動啟動隨機-自動啟動清單中的隨機起始點的媒體

**角色**

用來控制及設定多媒體主控台的角色指派。    這些角色會細分為下列集合：

* **僅擁有** 者-是多媒體主控台會話擁有者的使用者
* 提高 **許可權的使用者**-在媒體主控台原本設定的空間中，擁有仲裁者或主機角色的使用者
* **所有使用者** -所有使用者

這些角色的堆疊方式，是在這份清單中選擇的所有角色，也會獲得使用該功能的許可權。  範例：提高 **許可權的使用者** 即使在 AltspaceVR 中不是仲裁者或主機 * *，也會包含 **擁有** 者。 角色指派所控制的功能如下所示

* **可以控制媒體播放機** -決定哪些角色可以控制多媒體主控台的 media 播放按鈕
* **可以設定 media player** -藉由授與存取權給 [設定 **] 按鈕，** 判斷哪些角色可以設定多媒體主控台

### <a name="adding-photos-and-videos-to-the-media-list"></a>將相片和影片新增至媒體清單

媒體是多媒體主控台的核心。  影像和影片連結在多媒體主控台內可作為媒體類型來支援。  若要新增媒體，請選取 [ **新增影像** ] 或 [ **新增影片** ] 圖示，讓對話方塊快顯以進入媒體資訊和設定。  以下是媒體類型和相關設定的細目

**映像**

影像應該是標準影像類型，例如 jpeg、png 和兒子。 它們必須裝載在具有公用連結的某個位置。

* **名稱** - (需要您想要用來識別映射的) 名稱。
* **影像 url** - (影像的公用 Url) 必要項
* **跳過之後** -應略過影像的秒數

**影片**

影片可透過 Twitch 和 DLive 託管影片或即時資料流。   (其他支援可以與額外的工作一起運作，以取得適當的串流 url，但在多媒體主控台中並未完全支援) 

* **名稱** - (需要您想要用來識別影片的) 名稱。
* **影片 URL** - (需要) 影片裝載所在的公用 URL，或提供即時資料流。
* **跳過之後** -應略過影片的秒數

> [!NOTE]
> 必要：放入符合影片長度的時間，讓影片能夠正確轉寄。 例如，如果您的影片是5分鐘長的300秒，否則您的影片不會跳到下一段內容。

* **磁片** 區-從 0 (min) -1 (最大) 值的影片數量。
* **開始時間** -從影片開頭開始的秒數。
* 從 **開始距離開始**：當您從多媒體主控台移出時，磁片區開始落在世界中的距離（單位為量）
* **影片結束動作** -到達影片結尾時要採取的動作。
    * 停止-媒體清單在影片結束後停止
    * 迴圈-影片將會迴圈直到手動略過
    * 下一步-媒體清單中的下一個媒體會在目前的影片結束之後啟動。

## <a name="working-with-json-directly-advancedoptional"></a>直接使用 JSON (advanced/optional) 

多媒體主控台支援在 AltspaceVR 中直接將 JSON 輸入主控台的提示。  JSON 是啟用媒體播放機設定的內部機制。 公開直接設定 JSON 的功能，可讓更高階的使用者建立自己的工作流程，以將其需求和熟悉的 JSON 組成套件。  以下是 JSON 結構的簡短描述，以及 JSON 驗證的架構。 如需下列屬性的詳細說明，請參閱上述有關設定多媒體主控台的章節。  本節主要著重于 JSON 資料的架構範例和結構。

### <a name="global-media-settings"></a>全域媒體設定

```json
{
  "loopMediaList": true | false
  "startMethod": "manual" | "autostart-beginning" | "autostart-random"
  "controlMediaPlayer": "everyone" | "elevated" | "owner"
  "configureMediaPlayer": "elevated" | "owner"
  ...
}
```

### <a name="media-list"></a>媒體清單

媒體清單是在 JSON 結構的根目錄設定的屬性，例如角色和播放設定。  它是一個簡單的陣列，可包含下列其中一種媒體配置結構。  (請參閱上述屬性描述，以取得各項功能的詳細資料。 ) 

**影像範例**

*必要欄位： "name" 和 "imageUrl"*

```json
{
    "name": "Altspace Screenshot",
    "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
    "skipAfter": 10
}
```

**影片範例**

*必要欄位： "name" 和 "videoUrl"*

```json
{
    "name": "Ninja Twitch Live Stream",
    "videoUrl":"https://www.twitch.tv/ninja",
    "volume":0.2,
    "startTime":0,
    "endOfVideoAction":"play-next"
}
```

### <a name="example-json"></a>範例 JSON

```json
{
  "loopMediaList": false,
  "startMethod": "autostart-beginning",
  "controlMediaPlayer": "everyone",
  "configureMediaPlayer": "elevated",
  "mediaList": [
    {
      "videoUrl": "https://www.twitch.tv/ninja",
      "volume": 0.2,
      "startTime": 0,
      "endOfVideoAction": "play-next"
    },
    {
      "imageUrl": "http://www.hypergridbusiness.com/wp-content/uploads/2016/09/AltspaceVR-highrise.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://d1qb2nb5cznatu.cloudfront.net/startups/i/333629-6ffd7199b9bcf34d8957e8e09d974a38-medium_jpg.jpg?buster=1423092095",
      "skipAfter": 5
    },
    {
      "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://altvr-wpengine.netdna-ssl.com/wp-content/uploads/2019/05/Educators-in-VR-Social-VR-AltspaceVR.png",
      "skipAfter": 10
    },
    {
      "videoUrl": "https://www.twitch.tv/shroud",
      "volume": 1,
      "startTime": 0,
      "endOfVideoAction": "stop"
    }
  ]
}
```

### <a name="schema"></a>結構描述

```json
{
  "$schema": "https://json-schema.org/draft-04/schema#",
  "type": "object",
  "required": [
    "mediaList"
  ],
  "properties": {
    "loopMediaList": {
      "type": "boolean",
      "description": "Whether to loop through the media list when reaching the beginning or end of the list."
    },
    "controlMediaPlayer": {
      "type": "string",
      "enum": [
        "everyone",
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are able to control the media player. (Owner can always control player)"
    },
    "configureMediaPlayer": {
      "type": "string",
      "enum": [
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are allowed to configure the media play list.  Note: This role needs to be able to control the media player in order to configure it. (Owner can always configure media)"
    },
    "startMethod": {
      "type": "string",
      "enum": [
        "manual",
        "autostart-beginning",
        "autostart-random"
      ],
      "default": "manual",
      "description": "The method by which the media player should start"
    },
    "mediaList": {
      "description": "A list of images or videos to configure the media player to operate on.",
      "type": "array",
      "items": {
        "oneOf": [
          {
            "title": "Image",
            "type": "object",
            "description": "Configuration for an image media.",
            "properties": {
              "imageUrl": {
                "type": "string",
                "description": "The url for the image to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              }
            },
            "required": [
              "imageUrl"
            ]
          },
          {
            "title": "Video",
            "type": "object",
            "description": "Configuration for a video media.",
            "properties": {
              "videoUrl": {
                "type": "string",
                "description": "The url of the video to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              },
              "volume": {
                "type": "number",
                "minimum": 0,
                "maximum": 1,
                "default": null,
                "description": "The volume to play the video at. (Minimum 0, maximum 1)"
              },
              "startTime": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The time in seconds from the start of the video to begin playing the video at. (Minimum of 0)"
              },
              "rolloffStartDistance": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The distance in meters away from the media player that the volume will begin to fall off. (Minimum 0)"
              },
              "endOfVideoAction": {
                "type": "string",
                "enum": [
                  "stop",
                  "loop",
                  "play-next"
                ],
                "default": null,
                "description": "The type of action to take at the end of the video."
              }
            },
            "required": [
              "videoUrl"
            ]
          }
        ]
      }
    }
  }
}
```

> [!NOTE]
> 最新的多媒體主控台 v 0.5。0