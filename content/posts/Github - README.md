---
title: "Github - README"
date: 2023-06-06 21:11:00
draft: true

tags: ["Github"]
---

## Quick Chat
README.md 是 Repository 的門面這是無庸置疑的。文檔是任何軟體專案的重要組成部分，應該從一開始就認真對待。最好的開始方式是創建一個好的自述文件，向用戶顯示基本信息，而不是用他們可能不需要的內容來淹沒他們，以便開始使用您的專案。

> 當一個人可以在不需要查看你的模組程式碼的情況下使用它時，你的文件才算是完整的。
> 這點非常重要。這使你能夠將模組的文件化介面與其內部實現（內部運作機制）分離開來。
> 這樣做是有好處的，因為這意味著只要介面保持不變，你就可以自由地更改模組的內部結構。
> -- [Ken Williams]

這不就是抽象設計嗎? 果然寫文件和寫程式碼，其實殊途同歸。文件和程式碼都是為了讓別人能夠理解和使用你的工作成果。


## Guide
- [你知道對專案來說，README.md 有多麼重要嗎？ ── 工程師血淚史](https://medium.com/dean-lin/%E4%BD%A0%E7%9F%A5%E9%81%93%E5%B0%8D%E5%B0%88%E6%A1%88%E4%BE%86%E8%AA%AA-readme-md-%E6%9C%89%E5%A4%9A%E9%BA%BC%E9%87%8D%E8%A6%81%E5%97%8E-%E5%B7%A5%E7%A8%8B%E5%B8%AB%E8%A1%80%E6%B7%9A%E5%8F%B2-c0fb0908343e)
- [README 的藝術](https://github.com/hackergrrl/art-of-readme/blob/master/README-zh-TW.md)
- [在 GitHub 上写入](https://docs.github.com/zh/get-started/writing-on-github)

## Markdown + Vscode 
- [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
- [Markdown Preview Github Styling](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-preview-github-styles) 

## Template
- [README-Template.md](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)

## Strategy 
筆者之前寫的 README 總有一種廉價感(結構?)，因此去 github 觀摩大佬的 README 是怎麼寫的，更不用說大家都是用 Markdown 寫的，會覺得不足，肯定是駕駛員的問題。結論一些在筆者覺得有問題的要避免習慣。

### README 為誰而寫

之前沒意識到讀文件的人分成使用者和開發人員

**以使用者角度**
- Tutorial
- Reference  

**以開發者角度**
- 開發環境設定指南
- Getting Started。
- 測試方法
- 部署・發布方法
- 設計資料・編碼規範等連結
- 開發流程

### README 過長/過短

此文件夾的內容大概就像：

installation.md - 詳細顯示如何安裝項目的文檔。
usage.md - 項目使用情況和主要命令的更詳細視圖。
advanced.md - 包含一些進階使用選項和用例的文檔。
指向 CONTRIBUTING.md 文檔的鏈接，其中包含有關用戶如何為您的專案做出貢獻的詳細訊息

當 將 README 拆分為其他文檔
對於存儲庫中的文檔，您可以在應用程式的根目錄中創建一個“/docs”目錄，並使用“/docs/README.md”文件作為文檔的入口點或索引。



### 三級段落太多

下面是原本的寫作方式下意識的使用不少的三級標題 `### Header`，筆者揣測當時的心理，寫做十做十作者可能過度關注細節，試圖在文檔中盡可能多地涵蓋所有信息，以便讀者不會錯過任何重要內容。
``` 
## Header2

### Header3
分段...

### Header3
分段...
```

但實際在讀文件時 順著讀下來也不用多做一些特別的分段，原本以為會很難閱讀 但實際上體驗下來似乎不會
``` 
## Header2
直接承接本文段落...
```
