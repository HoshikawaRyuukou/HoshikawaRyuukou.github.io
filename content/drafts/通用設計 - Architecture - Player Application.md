---
title: "通用設計 - Architecture - Player Application"
date: 2024-01-19 21:05:00
draft: trye

tags: ["Common Design", "Architecture"]
---

- 以本次的應用來說 從server 接收資料並呈現
- 基本沒有什麼 業務邏輯 就算有也是 應用邏輯
- 但用 port 將 變化隔離是可行的 / fake 時也有用
- 對 api 的要求如果不是對應到單畫面 
- 在 api 取回的資料比較雜的狀況下 則須考慮較全局的狀態管理



- 沒有明確的進入點 多個 mono awake 併發
- 靜態數據設定可以拉到 ScriptableObject
- 動態數據用單例到是無妨 但依賴方向要對
- 無法單獨測試動畫 因為 view 不是被動的
- 應該要很容易模擬所以 case 而不是真的用 server + 記錄檔來看 case
- slot 大獎通知?

- 依賴 inspector 的結果
- 掛一堆 Mono 
- 難以追蹤腳本使用


- client 的目的是要顯示數據  
- 以 client / Server 來說 client 沒有業務邏輯 事務腳本倒是有

