# num2chn

> 🚄 Convert numbers to Chinese

---
![NPM](https://img.shields.io/npm/l/@bryanadamss/num2chn)
[![GitHub issues](https://img.shields.io/github/issues/BryanAdamss/num2chn)](https://github.com/BryanAdamss/num2chn/issues)


## Links

[https://github.com/BryanAdamss/num2chn](https://github.com/BryanAdamss/num2chn)

## Install
```javascript
npm i @bryanadamss/num2chn
```
or
```javascript
<script src="https://unpkg.com/@bryanadamss/num2chn@latest/dist/num2chn.umd.js"></script>
```

## How to use
```javascript
import Num2Chn from '@bryanadamss/num2chn'

const instance= new Num2Chn()

instance.transform(123)
```

## Demos
- https://github.com/BryanAdamss/num2chn/tree/master/examples

## API
Num2Chn(options)
- `options` is not required

- `default options`
```javascript
// 默认参数
{
  unitChars:['', '十', '百', '千'], // 节内权位
  sectionUnitChars: ['', '万', '亿', '万亿', '亿亿'], // 节权位
  numChars:['零', '一', '二', '三', '四', '五', '六', '七', '八', '九'], // 数字映射表
  dotChar:'点', // 小数点
  signChar:'负' // 符号
}
 
```
- `methods`
- 😂Most of the scenes, you only need to use `instance.transform()` method
```typescript
  /**
   * 获取数字对应中文
   *
   * @param {number} n 数字
   * @returns {string} 数字对应中文
   * @memberof Num2Chn
   */
  getNumChar(n: number): string {}

  /**
   * 获取节内权位
   *
   * @param {number} i 索引
   * @returns {string} 对应中文
   * @memberof Num2Chn
   */
  getUnitChar(i: number): string {}

  /**
   * 获取节权位
   *
   * @param {number} i 索引
   * @returns {string} 对应中文
   * @memberof Num2Chn
   */
  getSectionUnitChar(i: number): string {}

  /**
   * 获取点号对应中文
   *
   * @param {string} dotPart 点号部分
   * @returns {string} 点号对应中文
   * @memberof Num2Chn
   */
  getDotPartChn(dotPart: string): string {}

  /**
   * 获取符号对应中文
   *
   * @param {string} signPart 符号部分
   * @returns {string} 符号对应中文
   * @memberof Num2Chn
   */
  getSignPartChn(signPart: string): string {}

  /**
   * 获取小数部分的中文表示
   *
   * @param {(number | string)} n 小数部分
   * @returns {string} 小数部分的中文表示
   * @memberof Num2Chn
   */
  getDecimalPartChn(n: number | string): string {}

  /**
   * 获取整数部分小节
   *
   * @param {(number | string)} n 整数
   * @returns {number[]} 小节数组
   * @memberof Num2Chn
   */
  getIntergerSections(n: number | string): number[] {}

  /**
   * 翻译小节
   *
   * @param {(number|string)} section 4位长度的小节
   * @returns {string} 小节对应中文
   * @memberof Num2Chn
   */
  getSectionsChn(section: number | string): string {}

  /**
   * 获取整数部分对应中文
   *
   * @param {(number|string)} intergerPart 整数部分
   * @returns {string} 整数部分对应中文
   * @memberof Num2Chn
   */
  getIntergetPartChn(intergerPart: number | string): string {}

  /**
   * 浮点数转中文数字
   *
   * @export
   * @param {(number | string)} n 需要转换的数字
   * @returns {string} 数字对应中文
   */
  transform(n: number | string): string {}
```


## Changelog

[changelog](https://github.com/BryanAdamss/num2chn/blob/master/CHANGELOG.md)

Detailed changes for each release are documented in the [release notes](https://github.com/BryanAdamss/num2chn/releases).

## License
[MIT](https://opensource.org/licenses/MIT)

Copyright (c) 2019-present, bryanadamss GuangHui.

