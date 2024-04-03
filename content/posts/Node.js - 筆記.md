---
title: "Node.js - 筆記"
date: 2024-03-13 21:11:00
draft: false

tags: ["Node.js"]
---

## 導讀
- [Node.js究竟是什么？初学者指南](https://zhuanlan.zhihu.com/p/648238863)
- [TypeScript 语言简介 | 阮一峰 TypeScript 教程](https://typescript.p6p.net/typescript-tutorial/intro.html)
- [tsx: 替代 node 指令、支持运行 TypeScript & ESM 的 CLI 程序](https://www.bilibili.com/read/cv27094154/)
- [如何在 TypeScript + ESM + Mocha + tsconfig-paths 下运行 Mocha 测试用例](https://shuizhongyueming.com/2024/02/29/mocha-with-typescript-esm-and-tsconfig-paths/)

## 環境

### Windows
- [coreybutler/nvm-windows](https://github.com/coreybutler/nvm-windows)
- [nvm-windows 管理 Windows Node.js 版本](https://medium.com/@ray102467/nvm-windows-%E7%AE%A1%E7%90%86-windows-node-js-%E7%89%88%E6%9C%AC-68d789cf84d7)
- [解决Node.js的命令行输出中文乱码问题（也适用于Electron）](https://www.jianshu.com/p/a07eeb43d8b3)
- [如何在Node.js中使用TypeScript](https://juejin.cn/post/7174610946713714702)

## 指令

### npm
- npm help install : 查看 npm install 指令集
- -D: 等價於 --save-dev，套件添加到 package.json 的 devDependencies 


## 建置
```console
npm init -y
npm install -D typescript
npm install -D ts-node
tsc --init
```

package.json
```json
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
- [Setup a new TypeScript project with Mocha support](https://gist.github.com/ika18/7734820ab1475401d9813407b5c5101c)
- [Chai](https://www.chaijs.com/)

## Framework
- [electron/electron](https://github.com/electron/electron)

