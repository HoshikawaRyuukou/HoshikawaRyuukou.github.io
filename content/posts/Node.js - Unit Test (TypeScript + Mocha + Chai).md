---
title: "Node.js - Unit Test ( TypeScript + Mocha + Chai )"
date: 2024-04-03 21:11:00
draft: false

tags: ["Node.js", "TypeScript", "Mocha", "Chai"]
---

## Guide
- [Setup a new TypeScript project with Mocha support](https://gist.github.com/ika18/7734820ab1475401d9813407b5c5101c)
- [如何在 TypeScript + ESM + Mocha + tsconfig-paths 下运行 Mocha 测试用例](https://shuizhongyueming.com/2024/02/29/mocha-with-typescript-esm-and-tsconfig-paths/)
- [Chai](https://www.chaijs.com/)

## Configure
```
npm install -D typescript mocha ts-mocha chai
npm install -D @types/node
npm install -D @types/mocha
npm install -D @types/chai 
```

> test 文件至於 根附錄 test/ 之下，使用 *.spec.ts 格式命名

.mocharc.json
```json
{
  "extension": [
    "ts"
  ],
  "spec": "test/**/*.spec.ts",
  "import": "tsx"
}
```

package.json
```json
{
  "scripts": {
    "test": "ts-mocha"
  }
}
```

simpleTest.spec.ts
```ts
describe('Simple Test', () => {
  it('should pass this simple test', () => {
    const x = 2;
    const y = 2;
    const sum = x + y;
    expect(sum).to.equal(4);
  });
});
```

```
npm test
```