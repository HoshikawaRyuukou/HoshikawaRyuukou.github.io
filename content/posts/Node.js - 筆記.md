---
title: "Node.js - 筆記"
date: 2024-03-13 21:11:00
draft: false

tags: ["Node.js"]
---

## 導讀
- [Node.js究竟是什么？初学者指南](https://zhuanlan.zhihu.com/p/648238863)

## 環境

### Windows
- [coreybutler/nvm-windows](https://github.com/coreybutler/nvm-windows)
- [nvm-windows 管理 Windows Node.js 版本](https://medium.com/@ray102467/nvm-windows-%E7%AE%A1%E7%90%86-windows-node-js-%E7%89%88%E6%9C%AC-68d789cf84d7)
- [解决Node.js的命令行输出中文乱码问题（也适用于Electron）](https://www.jianshu.com/p/a07eeb43d8b3)
- [如何在Node.js中使用TypeScript](https://juejin.cn/post/7174610946713714702)

### 建置
```console
npm init -y
npm install -D typescript
npm install -D ts-node
tsc --init
```
```json
package.json
"scripts": {
   "start": "ts-node ./src/index.ts"
}
```
```console
npm start
```

## Architecture
- [Enterprise Node + TypeScript | Khalil Stemmler](https://khalilstemmler.com/articles/categories/enterprise-node-type-script)

## Testing
- [Node.js Testing: Best Practices and Frameworks](https://medium.com/@vishwasacharya/node-js-testing-best-practices-and-frameworks-for-reliable-apps-656f1cc51426)

## Framework
- [electron/electron](https://github.com/electron/electron)

