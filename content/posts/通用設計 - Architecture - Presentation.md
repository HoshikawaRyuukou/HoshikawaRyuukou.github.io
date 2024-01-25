---
title: "通用設計 - Architecture - Presentation"
date: 2024-01-20 21:05:00
draft: true

tags: ["Common Design", "Architecture"]
---




畫面設計
手機遊戲的畫面設計要求
・我想批量生產具有各種功能的螢幕。
主螢幕、卡片螢幕、任務螢幕、扭蛋螢幕、活動螢幕等。
我想支援螢幕之間的頻繁轉換
我想返回到上一個螢幕或在螢幕之間傳遞訊息。
需要一個能夠在螢幕之間平滑過渡並實現高效批量生產的平台。


階層關係
Scene - Window - Screen


Scene
- OnInitialize
- OnOpenIn
- OnCloseIn
- OnOpenOut
- OnCloseOut
- Close

Window
- Open
- Switch

Screen
- Close

樹狀結構
要做到疊加是相對方便
屏幕之間的頻繁轉換，以及在這些轉換期間需要交換的資訊 -> 通過按住和管理 >螢幕實現
需要更深入地過渡到層次結構 -> 通過擴展整個螢幕而不是單個螢幕來實現的

角色資訊頁 -> 角色強化頁


分成 
呈現 與 容器


情境 Extra1
AppScene -> CharaWindow -> CharaInfoScreen

AppScene -> CharaWindow -> CharaInfoScreen
         -> StoreWindow -> StuffInfoScreen
                        -> StuffBuyScreen





## 簡述

## 啟發

