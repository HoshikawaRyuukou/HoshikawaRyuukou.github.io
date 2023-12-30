---
title: "Unity - Official - URP"
date: 2023-04-01 21:11:00
draft: true

tags: ["Unity"]
---

- [[Unity] 腳本模板 | 如何創建自定義腳本模板 | Script Templates](https://www.youtube.com/watch?v=uh9bDTX9T5E)
- [【Unity教學-Rendering】用URP提升渲染品質 | Unity基礎渲染](https://www.youtube.com/watch?v=LLwnmGInpC4)
- [【Unity】uGUIのリビルドによるパフォーマンス低下を防ぐ方法](https://light11.hatenadiary.com/entry/2019/06/02/214125)
- [使用Unity Cinemachine快速實現遊戲中的鏡頭跟隨功能｜Unity Cinemachine教學分享](https://delightcollab.com/programming-tpl-cinemachine-tutorial-2022/)
- [【游戏开发教程】Unity Cinemachine快速上手，详细案例讲解](https://blog.csdn.net/linxinfa/article/details/124537415?spm=1001.2014.3001.8079)
- [Doing basic unit testing in Unity/C#](https://www.minapecheux.com/articles/2022/01/03_doing-basic-unit-testing-in-unity-c/)
- [2D animation in Unity - The PERFECT workflow](https://www.youtube.com/watch?v=vLDK0eHwsho)
- [橙子SKODE](https://skode.blog.csdn.net/?type=blog)
- [Why Animation Curves In Unity Are So Useful](https://www.youtube.com/watch?v=Nc9x0LfvJhI)
- [壓縮](https://takap-tech.com/entry/2020/01/20/211934)
- [Unity 年度总结：一款游戏的从0到1](https://blog.csdn.net/mahuibao01/article/details/113681486)
- [基于Unity Audio Mixer的音效系统](https://blog.csdn.net/mahuibao01/article/details/113857193)
- [GF框架](https://blog.csdn.net/m0_37920739/category_9877543.html)
- [Ellan Jiang](https://github.com/EllanJiang)
- [Clean Settings UI](https://assetstore.unity.com/packages/tools/gui/clean-settings-ui-65588)
- [Unity I18N 小探](https://zhuanlan.zhihu.com/p/81159633)
- [如何设计本地化组件](http://www.liuocean.com/2022/08/14/ru-he-she-ji-ben-de-hua-zu-jian/)
- [【Unity】iOSネイティブプラグイン開発を完全に理解する - サンプルコードをSwiftだけで完結出来るように置き換える](https://qiita.com/mao_/items/07466e169d08cbeff221)
- [【Unity】iOSネイティブプラグイン開発を完全に理解する](https://qiita.com/mao_/items/5b33c90e533a538570b8#swift%E3%81%A7%E5%AE%9F%E8%A3%85%E3%81%97%E3%81%AA%E3%81%84%E3%81%AE%E3%81%8B)
- [Swift だけで Unity の iOS の Native Plugin を作る](https://qiita.com/fuziki/items/955c2b35514bcfc37969)
- [介接Unity Ads](https://www.goostudio.tw/post/%E4%BB%8B%E6%8E%A5unity-ads?fbclid=IwAR3Oa5MaKg_cZnnd3bvMULBAUwSVy6qwft0tuY02ZIOF0ZXXSpFEPAUtcBY)
- [The “Real” Modularization in Android](https://betterprogramming.pub/the-real-clean-architecture-in-android-modularization-e26940fd0a23)




---
愛使用Camera來畫UI的同學要注意了，在URP下，切記把Overlay Type的stacking Camera的DepthTexture設成Off，尤其是專案有使用到深度紋理的部份，否則會多做一次CopyDepth