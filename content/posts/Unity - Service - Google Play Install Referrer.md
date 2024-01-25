---
title: "Unity - Service - Google Play Install Referrer"
date: 2024-01-16 22:11:00
draft: true

tags: ["Unity"]
---

## 簡述

## 快速上手

- https://developer.android.com/google/play/installreferrer?hl=zh-tw
- https://blog.csdn.net/HUandroid/article/details/119249924
- https://blog.csdn.net/hzqit520/article/details/128624927
- 文檔不全
- https://blog.csdn.net/HUandroid/article/details/119249924
- https://blog.csdn.net/hzqit520/article/details/128624927
- https://developers.google.com/analytics/devguides/collection/android/v4/campaigns?hl=zh-cn#general-campaigns
- https://juejin.cn/post/7305182777438683162
- 








  

## Referrer 狀態

將手機連著 android studio 開啟 Logcat，透過連結前往商店發現有 4 種情境
  
未安裝 點連結
> Finsky 
> com.android.vending 
> Capture referrer for **package name** 

已安裝 點連結
> Finsky 
> com.android.vending 
> Dropped referrer for **package name** because dropped_already_captured

已安裝 但有版本差異
> Finsky 
> com.android.vending 
> Dropped referrer for **package name** because dropped_already_installed

移除app 也會移除
> 但沒有 Finsky 相關 log


## 模擬測試

可以借別人(架上的)的 package name 來測試
- 將本地測試的專案 package name 改成別人的 package name
- 下載別人的產品但不要載完(要取消)
- 就可以借到當時的 referrer 
