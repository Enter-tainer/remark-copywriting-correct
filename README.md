# remark-copywriting-correct

[![version](https://img.shields.io/npm/v/remark-copywriting-correct.svg?style=flat-square)](http://npm.im/remark-copywriting-correct)
[![MIT License](https://img.shields.io/npm/l/remark-copywriting-correct.svg?style=flat-square)](http://opensource.org/licenses/MIT)
[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg?style=flat-square)](https://github.com/semantic-release/semantic-release)

给 Markdown 中英文自动插入空格的 [remark](https://github.com/wooorm/remark) 插件（使用 [https://github.com/rikakomoe/copywriting-correct](https://github.com/rikakomoe/copywriting-correct)）。

## Install

```bash
npm install remark-copywriting-correct
```

## Usage

```js
remark().use(pangu)
```

```js
const remark = require('remark')
const pangu = require('remark-copywriting-correct')

const doc = '中文abc中文$a_i$中文';
console.log(remark().use(pangu).process(doc).contents);
// => 中文 abc 中文 $a_i$ 中文
```

## LICENSE

[MIT](./LICENSE)
