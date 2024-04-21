---
title: "Node.js - Note"
date: 2024-03-13 21:11:00
draft: false

tags: ["Node.js", "JavaScript", "TypeScript"]
---

## Guide
- [Node.js究竟是什么？初学者指南](https://zhuanlan.zhihu.com/p/648238863)

## Environment
- [coreybutler/nvm-windows](https://github.com/coreybutler/nvm-windows)
- [nvm-windows 管理 Windows Node.js 版本](https://medium.com/@ray102467/nvm-windows-%E7%AE%A1%E7%90%86-windows-node-js-%E7%89%88%E6%9C%AC-68d789cf84d7)
- [解决Node.js的命令行输出中文乱码问题（也适用于Electron）](https://www.jianshu.com/p/a07eeb43d8b3)
- [tsx: 替代 node 指令、支持运行 TypeScript & ESM 的 CLI 程序](https://www.bilibili.com/read/cv27094154/)


## Project Configure
```
-D: 等價於 --save-dev，套件添加到 package.json 的 devDependencies 
```

```bash
npm install -g typescript
```

```bash
npm init -y
npm install -D typescript
npm install -D tsx
npm install -D @types/node
tsc --init
```

# ESLint
- [Understanding ESLint Configuration: .eslintrc.js vs .eslintrc vs .eslintrc.json](https://medium.com/@ritz.sh/understanding-eslint-configuration-eslintrc-js-vs-eslintrc-vs-eslintrc-json-287ec5e95bf4)
- [How to use ESLint with TypeScript](https://khalilstemmler.com/blogs/typescript/eslint-for-typescript/)
- [[note] ESLint](https://pjchender.dev/webdev/note-eslint/)

```bash
npx eslint --init

npm install --save-dev @typescript-eslint/parser @typescript-eslint/eslint-plugin
```

## Project Structure
```
mkdir demo src test
mkdir src\domain\entities
mkdir test\domain\entities
```


<!-- 
## Other
- [Enterprise Node + TypeScript | Khalil Stemmler](https://khalilstemmler.com/articles/categories/enterprise-node-type-script)
- [electron/electron](https://github.com/electron/electron)
- [TypeScript 语言简介 | 阮一峰 TypeScript 教程](https://typescript.p6p.net/typescript-tutorial/intro.html)
- [《JavaScript 教程》](https://developer.mozilla.org/zh-CN/docs/learn/JavaScript)
- [ES6 教程](https://wangdoc.com/es6/)
- [TypeScript 教程 | 菜鸟教程](https://www.runoob.com/typescript/ts-tutorial.html) 
- [TypeScript 教程 阮一峰](https://typescript.p6p.net/)
- [如何在Node.js中使用TypeScript](https://juejin.cn/post/7174610946713714702)
-->