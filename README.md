# 划词翻译

[![Build Status](https://img.shields.io/travis/lmk123/crx-selection-translate/master.svg?style=flat-square)](https://travis-ci.org/lmk123/crx-selection-translate)
[![Coverage Status](https://img.shields.io/coveralls/lmk123/crx-selection-translate/master.svg?style=flat-square)](https://coveralls.io/github/lmk123/crx-selection-translate?branch=master)
[![dependencies Status](https://img.shields.io/david/lmk123/crx-selection-translate.svg?style=flat-square)](https://david-dm.org/lmk123/crx-selection-translate)
[![devDependencies Status](https://img.shields.io/david/dev/lmk123/crx-selection-translate.svg?style=flat-square)](https://david-dm.org/lmk123/crx-selection-translate#info=devDependencies)

[![available in the chrome web store](https://developer.chrome.com/webstore/images/ChromeWebStore_BadgeWBorder_v2_206x58.png)](https://chrome.google.com/webstore/detail/ikhdkkncnoglghljlkmcimlnlhkeamad)

让浏览任意语言的网站变得无比轻松的 Chrome 扩展程序。

**注意：**安装完成后需要重启浏览器让扩展生效！另外，划词翻译在 Chrome 网上应用店内是无效的，这是 Chrome 自身的安全限制，请在其他网站测试！

## 特点

 - 划词即显示翻译结果，简单、方便、迅速，并且支持多种语言的朗读。
 - 支持在 PDF 文档内使用。
 - 支持多种翻译引擎：[有道翻译](http://fanyi.youdao.com/)、[百度翻译](http://fanyi.baidu.com/)、[谷歌翻译](https://translate.google.com/)（含[谷歌中国翻译](http://translate.google.cn/)）、[必应词典](http://cn.bing.com/dict/)。
 - 集成[有道网页翻译](http://fanyi.youdao.com/web2/)、[必应网页翻译](http://www.bing.com/widget/translator)与[谷歌网页翻译](http://translate.google.com/manager/website/?hl=zh-CN)，弥补国内 Chrome 网页翻译总是出错的不足。

## 安装

 - 在 [Chrome 网上应用店](https://chrome.google.com/webstore/detail/ikhdkkncnoglghljlkmcimlnlhkeamad)安装
 - [下载 .crx 安装包](https://github.com/lmk123/crx-selection-translate/releases/latest)手动安装

**注意**：非官方渠道的划词翻译可能会被嵌入恶意代码，所以请一定使用以上两种方式安装。

## [捐助划词翻译](https://github.com/lmk123/crx-selection-translate/wiki/%E6%8D%90%E5%8A%A9%E5%88%92%E8%AF%8D%E7%BF%BB%E8%AF%91)

划词翻译是开源且免费的软件，我在工作之余花了大量的时间和精力开发和维护这个项目，你的捐助会给我坚持下去的动力。

## 相关链接

 + [发布日志](https://github.com/lmk123/crx-selection-translate/releases)
 + [报告问题或提议新功能](https://github.com/lmk123/crx-selection-translate/issues/new)
 + [Wiki](https://github.com/lmk123/crx-selection-translate/wiki)

## 参与开发

划词翻译欢迎并鼓励开发者参与开发！请按照以下步骤搭建开发环境：

 1. Fork 项目之后将代码克隆到本地。
 2. 运行 `npm i` 安装项目依赖。如果你使用的是 NPM 2.x，还需要运行 `npm i babel-runtime`。
 3. 运行 `npm run dev`，项目的 [src 文件夹](https://github.com/lmk123/crx-selection-translate/tree/master/src)下会生成一个名为 `bundle` 的文件夹
 4. 在 Chrome 浏览器的扩展程序页面（chrome://extensions/）勾选开发者模式，点击“加载已解压的扩展程序”，将路径指向代码库的 [src 文件夹](https://github.com/lmk123/crx-selection-translate/tree/master/src)。

之后，你就可以更改代码并在浏览器中查看效果了。

### 划词翻译的子项目

为了方便维护，划词翻译将一些功能分离了出来，如果你是想对以下功能进行调整，请前往对应的代码仓库：

 + [translation.js](https://github.com/lmk123/translation.js) - 划词翻译的翻译引擎。
 + [connect.io](https://github.com/lmk123/connect.io) - Chrome 扩展/应用里的实时、双向、基于事件且 Promise 友好的通信库，启发自 Socket.io。
 + [chrome-call](https://github.com/lmk123/chrome-call) - 将 Chrome API 的使用回调函数接收结果的调用形式改为返回 Promise 对象的调用形式。
 + [chrome-env](https://github.com/lmk123/chrome-env) - 给非扩展程序运行环境添加 `window.chrome`，被设计用于单元测试。

## 第三方开源库

划词翻译的诞生离不开这些优秀的开源程序：

 - [Vue.js](http://vuejs.org/)
 - [PDF.js](https://mozilla.github.io/pdf.js/)
 - [Bootstrap](http://getbootstrap.com/)
 - [Webpack](http://webpack.github.io/)
 - [Babel](http://babeljs.io/)
 - [Sass](http://sass-lang.com/)
 - [Gulp](http://gulpjs.com/)
 - [Jasmine](http://jasmine.github.io/)
 - [Karam](https://karma-runner.github.io/)

[package.json](https://github.com/lmk123/crx-selection-translate/blob/master/package.json) 的 `dependencies` 与 `devDependencies` 里列出了划词翻译使用到的所有第三方程序。

## 许可

[GNU General Public License Version 3](https://www.gnu.org/licenses/gpl.html)
