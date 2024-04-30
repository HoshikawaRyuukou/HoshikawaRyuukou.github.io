---
title: "Node.js - Configure"
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

## ESLint
- [Understanding ESLint Configuration: .eslintrc.js vs .eslintrc vs .eslintrc.json](https://medium.com/@ritz.sh/understanding-eslint-configuration-eslintrc-js-vs-eslintrc-vs-eslintrc-json-287ec5e95bf4)
- [How to use ESLint with TypeScript](https://khalilstemmler.com/blogs/typescript/eslint-for-typescript/)
- [[note] ESLint](https://pjchender.dev/webdev/note-eslint/)
- [尝鲜ESLint v9版本 扁平模式(Flat Mode)如何配置](https://juejin.cn/post/7359505949319233548)

```bash
npm install -D eslint@8.57.0
npm install -D typescript-eslint
npm install -D @typescript-eslint/parser 
npm install -D @typescript-eslint/eslint-plugin
```

## Prettier 
- [How to use Prettier with ESLint and TypeScript in VSCode](https://khalilstemmler.com/blogs/tooling/prettier/)

```bash
npm install -D prettier  
npm install -D eslint-config-prettier  
npm install -D eslint-plugin-prettier
```

> ⚠️ 如果已經啟用 auto format，但並未生效
> ![format](/images/vscode-format-setting.png)
> 可能是有多個 formatter 同時作用，需指定預設 formatter (vscode 右下角應該會提示要選擇一種為預設)


## Project Architecture
- [domain-driven-hexagon](https://github.com/Sairyss/domain-driven-hexagon/tree/master?tab=readme-ov-file)
- [Enterprise Node + TypeScript | Khalil Stemmler](https://khalilstemmler.com/articles/categories/enterprise-node-type-script)
