---
title: "Unity - Package - VContainer"
date: 2023-12-28 21:11:00
draft: true

tags: ["Unity"]
---

## Resource
- [hadashiA/VContainer](https://github.com/hadashiA/VContainer)
- [Doc](https://vcontainer.hadashikick.jp/)

## 前述

VContainer 作為一個 DI library，在其的幫助下對象之間的依賴處理方便了很多。但還是必須要說 DI library 不是必要的，最基本實現依賴注入的方式便是 Composition Root ，也被稱作窮人的 DI。這裡主要紀錄應用時的得到的一些理解

### LifetimeScope 
- Lifetime.Singleton : 單例
- Lifetime.Scoped : 同範圍等同單例
- LifeTime.Transient : 每一個都是新的實例

LifetimeScope 能建立樹狀結構關係，在處理依賴時從離自己最近的開始往 Parent LifetimeScope 尋找


## 應用情境 - 共用資源

單例


## 應用情境 - LifetimeScope

以模組的角度來看生命週期





