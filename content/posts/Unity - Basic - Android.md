---
title: "Unity - Basic - Android"
date: 2023-03-01 21:11:00
draft: true

tags: ["Unity"]
---

- [UnityからAndroidのクラスや関数を呼び出す](https://zenn.dev/sunmax/articles/e079dd3ba7c487)


---


- gradleTemplate.properties : 是專案級別的 Gradle 配置檔，我們可以在裡面做一些 Gradle 檔的全域性的配置
- AndroidManifest.xml ：每個應用專案必須在專案源設置的根目錄中加入 AndroidManifest.xml， 該檔會向 Android 構建工具、Android 作業系統和 Google Play 描述應用的基本資訊。
- launcherManifest.xml 配置啟動時的圖示適配資訊
- mainTemplate.gradle：包含有關如何將 Unity 構建為庫的說明，改gradle為添加依賴的地方。
- launcherTemolate.gradle ：包含有關如何構建 Android 應用程式的指令
- baseProjectTemplate.gradle：所含的配置會在其他所有範本/Gradle 專案之間共用




---
- [Unity 不通過Android studio 打包接SDK](https://www.jianshu.com/p/9058daafa130)