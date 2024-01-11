# Taiji Encode
太极编码器

[![NPM version][npm-image]][npm-url]
[![Install size][install-size-image]][install-size-url]
[![NPM bundle size][npm-bundle-size-image]][npm-bundle-size-url]
[![NPM downloads][npm-download-image]][npm-download-url]

## 安装
```sh
npm install taiji-encode
```

## 使用
```javascript
import { taijiEncode, taijiDecode, isVaildTaiji } from `taiji-encode'

console.log(taijiEncode('Hello Taiji Encode!'))
// 输出: ䷜䷭䷾䷷䷹䷭䷠䷖䷾䷭䷣䷔䷮䷑䷳䷖䷂䷯䷘䷨䷹䷸䷂䷕䷏䷇☯☯
console.log(taijiDecode('䷜䷭䷾䷷䷹䷭䷠䷖䷾䷭䷣䷔䷮䷑䷳䷖䷂䷯䷘䷨䷹䷸䷂䷕䷏䷇☯☯'))
// 输出: Hello Taiji Encode!
console.log(taijiEncode('你好太极！'))
// 输出: ䷘䷵䷸䷖䷘䷮䷯䷌䷘䷮䷜䷿䷘䷔䷅䷗䷉䷉䷺䷗
console.log(taijiDecode('䷘䷵䷸䷖䷘䷮䷯䷌䷘䷮䷜䷿䷘䷔䷅䷗䷉䷉䷺䷗'))
// 输出: 你好太极！

console.log(isVaildTaiji('你好太极！'))
// 输出: false
console.log(isVaildTaiji('䷜䷭䷾䷷䷹䷭䷠䷖䷾䷭䷣䷔䷮䷑䷳䷖䷂䷯䷘䷨䷹䷸䷂䷕䷏䷇☯☯'))
// 输出: true
```

## TODO
* 支持自定义字符排序规则，用于简单混淆

## License
[MIT](LICENSE)

[npm-image]: https://img.shields.io/npm/v/taiji-encode.svg?style=flat-square
[npm-url]: https://www.npmjs.com/package/taiji-encode
[install-size-image]: https://img.shields.io/badge/dynamic/json?url=https://packagephobia.com/v2/api.json?p=taiji-encode&query=$.install.pretty&label=install%20size&style=flat-square
[install-size-url]: https://packagephobia.now.sh/result?p=taiji-encode
[npm-bundle-size-image]: https://img.shields.io/bundlephobia/minzip/taiji-encode?style=flat-square
[npm-bundle-size-url]: https://bundlephobia.com/package/taiji-encode@latest
[npm-download-image]: https://img.shields.io/npm/dm/taiji-encode.svg?style=flat-square
[npm-download-url]: https://npm-stat.com/charts.html?package=taiji-encode
