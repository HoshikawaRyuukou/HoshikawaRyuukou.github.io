---
title: "Unity - Service - Google Play Install Referrer"
date: 2024-01-16 22:11:00
draft: true

tags: ["Unity"]
---

## 簡述

[Play Install Referrer](https://developer.android.com/google/play/installreferrer?hl=zh-tw)

- Play Install Referrer API : 非 Kotlin / Java 用戶使用
- Play Install Referrer Library : 將上者封裝更方便 Kotlin / Java 使用

透過該服務能對 App 的下載與使用者進行歸因分析，用於評估推廣服務得成效，進而提升推廣效果與報酬率。

## 版本

## 配置 

將依賴加在 maintemplate.gradle
```
dependencies {
    implementation("com.android.installreferrer:installreferrer:2.2")
}
```

- 文檔不全
- https://blog.csdn.net/HUandroid/article/details/119249924
- https://blog.csdn.net/hzqit520/article/details/128624927
- https://developers.google.com/analytics/devguides/collection/android/v4/campaigns?hl=zh-cn#general-campaigns


## 快速上手

## Referrer 格式
```
https://play.google.com/store/apps/details?id=${package name}&referrer=${parameter}
```

常見的參數有以下 5 項
- utm_source  
- utm_medium
- utm_campaign
- utm_term
- utm_content

連結可使用小工具生成 - [Play Campaign URL Builder](https://ga-dev-tools.google/campaign-url-builder/play/)

## Referrer 狀態

將手機連著 android studio 開啟 Logcat，透過連結前往商店發現有 4 種情境
  
- 未安裝 點連結
> Finsky 
> com.android.vending 
> Capture referrer for **package name** 

- 已安裝 點連結
> Finsky 
> com.android.vending 
> Dropped referrer for **package name** because dropped_already_captured

- 已安裝 但有版本差異
> Finsky 
> com.android.vending 
> Dropped referrer for **package name** because dropped_already_installed

- 移除app 會移除 referrer
> 但沒有 Finsky 相關 log

## 模擬測試

透過**Google Play Console 封閉式測試**是比較正規的測法，但如果沒有現成的產品，也可以借別人(架上的)的 package name 來測試
- 下載別人的產品但**不要載完(要取消)**，這時 referrer 還會保留
- 將本地測試的專案 package name 改成別人的 package name，就能使用到保留的 referrer 

## Ref
- [Android 下載歸因— GA與Play Install Referrer庫](https://juejin.cn/post/7305182777438683162)

