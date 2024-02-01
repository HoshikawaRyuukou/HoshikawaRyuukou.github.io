---
title: "Unity - Packages"
date: 2024-01-28 21:11:00
draft: false

tags: ["Unity"]
---

## Package Manager
### Installing Packages using UPM
1. Package manager ->  Advanced project settings
2. Add Scoped Registries

```
Name: package.openupm.com
URL: https://package.openupm.com
Scope(s): 
         com.cysharp.unitask
```
3. Package manager -> Packages: My Registries -> Install

- [Unity中 .asmdef文件的作用](https://zhuanlan.zhihu.com/p/139090680)
- [使用OpenUPM发布自己的Unity项目](https://zhuanlan.zhihu.com/p/146565975)
- [开发Unity PackageManager 插件包](https://www.jianshu.com/p/153841d65846)
- [Creating Custom Packages for Unity 2018.3](https://neogeek.dev/creating-custom-packages-for-unity-2018.3/)
- [How to remodel your project for asmdef and UPM](https://gametorrahod.com/how-to-asmdef-upm/?fbclid=IwAR31P12StjzcTi9IO1vDvwWJIwaKHxIEmUQLic6K1LGElmwv6OFRqe8sVig)
- [【Unity】Package Manager活用術](https://annulusgames-lab.blogspot.com/2023/01/unity-package-manager.html)

---

## Animation
- [PrimeTween](https://github.com/KyryloKuzyk/PrimeTween)

## Async
- [UniTask](https://github.com/Cysharp/UniTask)    
  - [Patterns & Practices for efficiently handling C# async/await cancel processing and timeouts](https://neuecc.medium.com/patterns-practices-for-efficiently-handling-c-async-await-cancel-processing-and-timeouts-b419ce5f69a4)
  - [精选Unity-Github开源库分享 最完美的异步操作解决方案 UniTask](https://www.bilibili.com/video/BV1NG411s7hN/?spm_id_from=333.788)
  - [C# Task 指南](http://www.liuocean.com/2022/10/11/c-task-zhi-nan/)
  - [async/await,disposableを使って素直で読みやすいコードを書く](https://learning.unity3d.jp/7224/)
  - [UniTaskCompletionSource Should Support CancellationToken](https://github.com/Cysharp/UniTask/issues/81)

## Debug
- [UnityIngameDebugConsole](https://github.com/yasirkula/UnityIngameDebugConsole)

## Dependency Injection
- [VContainer](https://github.com/hadashiA/VContainer)  
  - openupm - jp.hadashikick.vcontainer  
  - [How to avoid Dependency Injection constructor madness?](https://stackoverflow.com/questions/2420193/how-to-avoid-dependency-injection-constructor-madness)

## Dialogue 
- [YarnSpinner-Unity](https://github.com/YarnSpinnerTool/YarnSpinner-Unity) 

## Editor
- [NaughtyAttributes](https://github.com/dbrizov/NaughtyAttributes)  

## HotUpdate
- [HybridCLR](https://hybridclr.doc.code-philosophy.com/)

## Localization
- [Lean Localization](https://assetstore.unity.com/packages/tools/localization/lean-localization-28504)

## Media
- [UnityNativeCamera](https://github.com/yasirkula/UnityNativeCamera)

## Messaging 
- [MessagePipe](https://github.com/Cysharp/MessagePipe)    

## Persistence
- [PlayerPrefs Editor & Utilities](https://github.com/sabresaurus/PlayerPrefsEditor)

## Resource Management
- [YooAsset](https://github.com/tuyoogame/YooAsset)

## Rx (Reactive Extensions)
- [UniRx](https://github.com/neuecc/UniRx)    
  - [【Unity框架】UniRx精讲](https://www.bilibili.com/read/cv15236973)

## Serialization
- [Newtonsoft.Json](https://github.com/jilleJr/Newtonsoft.Json-for-Unity/wiki/Install-official-via-UPM)
  - git - com.unity.nuget.newtonsoft-json

## Sharing
- [Unity Native Share Plugin](https://github.com/yasirkula/UnityNativeShare)

## State Machine
- [UnityHFSM](https://github.com/Inspiaaa/UnityHFSM)

## UI
- [LoopScrollRect](https://github.com/qiankanglai/LoopScrollRect)
  - openupm - me.qiankanglai.loopscrollrect
  - [効率的なスクロールビューを実装するためのOSS『Loop Scroll Rect』使い方まとめ](https://light11.hatenadiary.com/entry/2022/05/16/201949)
