---
title: "Pattern - State"
date: 2024-06-27 21:05:00
draft: true

tags: ["Pattern"]
---

- [State · Design Patterns Revisited · Game Programming Patterns](https://gameprogrammingpatterns.com/state.html)




每次我們接觸這部分程式碼時，我們都會破壞一些東西。

複雜分支和可變狀態（隨時間變化的欄位）是兩種容易出錯的程式碼，

總而言之，要添加這種衝鋒攻擊，我們必須修改兩個方法並添加一個 chargeTime_字段，Heroine儘管它僅在閃避狀態下才有意義。
我們希望將所有程式碼和資料很好地封裝在一個地方。四人幫已經為我們提供了保障。