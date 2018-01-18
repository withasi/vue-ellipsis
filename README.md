# vue-ellipsis


[![Version](https://img.shields.io/npm/v/vue-ellipsis2.svg)](https://www.npmjs.com/package/vue-ellipsis2) [![License](https://img.shields.io/npm/l/vue-ellipsis2.svg)](https://www.npmjs.com/package/vue-ellipsis2) [![Downloads](https://img.shields.io/npm/dt/vue-ellipsis2.svg)](https://www.npmjs.com/package/vue-ellipsis2)

fork from https://github.com/jypblue/vue-ellipsis

a multiline sentence ellipsis component of vue2.js

## Features
- Supports Vue2.js
- Compact size 2KB(1KB gzipped)

## Installation

### NPM
```
$ npm install vue-ellipsis2 --save
```
### Yarn
```
$ yarn add vue-ellipsis2
```

### Bower
```
$ bower install vue-ellipsis2
```

## Ellipsis Component Attributes

| 参数        | 说明           | 类型               | 默认值       |  必写   |
|------------|----------------|--------------------|--------------|----------------|
| data | 需要添加省略号的内容 | String | -   | true |
| line-clamp  | 显示几行 | Number | 1  | true |
| line-height | 单行高度(设定时与实际单行高度一致，若使用rem请自行计算转换)  | String | '22px'   | true |
| end-char | 句子末尾跟随字符串 | String |'...'| false |
| end-html | 句子末尾跟随HTML片段 | String| - | false |
| click | 点击回调函数 |  Function | - | false |


## How To Use

```
Import:
import Vue from 'vue'
import VueEllipsis from 'vue-ellipsis2'
Vue.use(VueEllipsis)

Component Use:

html: HTML String. just like '<span class="read-more">read more</span>'
handleClick: click callback function

<ellipsis
:data="msg"
:line-clamp="2"
:line-height="'24px'"
:end-char="'###'"
:end-html="html"
@click="handleClick"
>
</ellipsis>

```



## License

[MIT](http://opensource.org/licenses/MIT)
