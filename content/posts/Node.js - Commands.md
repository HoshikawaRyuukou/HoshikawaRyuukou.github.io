---
title: "Node.js - Commands"
date: 2024-05-26 21:11:00
draft: false

tags: ["Node.js"]
---

## Install

| 特性/用途                    | npm install                                | npm ci (npm clean-install) |
| ---------------------------- | ------------------------------------------ | -------------------------- |
| 安裝依據                     | 根據 `package.json` 和 `package-lock.json` | 只根據 `package-lock.json` |
| 安裝來源                     | 使用本地緩存來加快安裝速度                 | 直接從註冊表下載軟體包     |
| 是否需要 `package-lock.json` | 否                                         | 是                         |
| 是否更新 `package-lock.json` | 是，可能會更新                             | 否，不會更新               |
| 是否清理 `node_modules`      | 否                                         | 是                         |
| 速度                         | 較慢 (需要解析和更新 `package-lock.json`)  | 較快                       |
| 一致性                       | 可能不同次安裝結果不同                     | 保證一致，每次安裝結果相同 |
| **使用場景**                 | **開發環境**                               | **CI/CD 環境**             |

### npm install args
| args           | 作用                         |
| -------------- | ---------------------------- |
| -g, --global   | 全局安裝                     |
| -D, --save-dev | 套件將添加到 devDependencies |

## Package
- npm pack : 以 `.tgz` 導出 package