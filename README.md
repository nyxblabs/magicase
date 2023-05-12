[![cover][cover-src]][cover-href]
[![npm version][npm-version-src]][npm-version-href] 
[![npm downloads][npm-downloads-src]][npm-downloads-href] 
[![bundle][bundle-src]][bundle-href] 
[![License][license-src]][license-href]

# 🪄 Magicase

> 🔮 Magical utility for string casing

## 📥 Install:

```bash
# nyxi
nyxi magicase

# pnpm
pnpm add magicase

# npm
npm i magicase

# yarn
yarn add magicase
```

## 🔽 Import:

```ts
// CommonJS
const { pascalCase } = require('magicase')

// ESM
import { pascalCase } from 'magicase'
```

**Notice:** You may need to transpile the package for older environments.

## 🧰 Utils

### 🐪 `pascalCase(str)`

Splits the string and joins it in PascalCase convention (foo-bar ➡️ FooBar)

**Remarks:**

If an uppercase letter is followed by other uppercase letters (e.g., FooBAR), it is preserved.

### 🐫 `camelCase`

Splits the string and joins it in camelCase convention (foo-bar ➡️ fooBar)

### 🥙 `kebabCase(str)`

Splits the string and joins it in kebab-case convention (fooBar ➡️ foo-bar)

**Remarks:**

- It does **not** preserve case

### 🐍 `snakeCase`

Splits the string and joins it in snake_case convention (foo-bar ➡️ foo_bar)

### 🔠 `upperFirst(str)`

Converts the first character to uppercase.

### 🔡 `lowerFirst(str)`

Converts the first character to lowercase.

### 🧩 `splitByCase(str, splitters?)`

- 🧩 Splits the string by the provided splitters (default: ['-', '_', '/', '.']).
- 🔄 Splits when there is a case change from lowercase to uppercase or uppercase to lowercase.
- 🔢 Ignores numbers for case changes.
- 📝 Case is preserved in the returned value.
- ❌ This is an irreversible function since the splitters are omitted.

## Development

- 🐙 Clone this repository
- 📥 Install latest LTS version of [Node.js](https://nodejs.org/en/)
- 🧩 Enable [Corepack](https://github.com/nodejs/corepack) using corepack enable
- 📦 Install dependencies using pnpm install
- ▶️ Run interactive tests using pnpm dev

## 📜 License

[MIT](./LICENSE) - Made with 💞

<!-- Badges -->

[npm-version-src]: https://img.shields.io/npm/v/magicase?style=flat&colorA=18181B&colorB=14F195
[npm-version-href]: https://npmjs.com/package/magicase
[npm-downloads-src]: https://img.shields.io/npm/dm/magicase?style=flat&colorA=18181B&colorB=14F195
[npm-downloads-href]: https://npmjs.com/package/magicase
[bundle-src]: https://img.shields.io/bundlephobia/minzip/magicase?style=flat&colorA=18181B&colorB=14F195
[bundle-href]: https://bundlephobia.com/result?p=magicase
[license-src]: https://img.shields.io/github/license/nyxblabs/magicase.svg?style=flat&colorA=18181B&colorB=14F195
[license-href]: https://github.com/nyxblabs/magicase/blob/main/LICENSE

<!-- Cover -->
[cover-src]: https://raw.githubusercontent.com/nyxblabs/magicase/main/.github/assets/cover-github-magicase.png
[cover-href]: https://💻nyxb.ws
