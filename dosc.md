> svg-vuejs 是基于 vuejs 2.0 项目量身定制的 SVG 解决方案，所以目前只支持 vue.js 2.0。 由于目录结构的限制，需要在项目根目录下的 src 文件夹下手动创建 svg 文件夹，用于存放将要使用的 svg 文件。

## 安装 svg-vuejs

<p style="color: #5e6d82; font-size: 14px;">
命令行进入项目根目录执行下面命令，安装最新稳定版，当然你也可以指定版本号安装对应
    <a href="/#/changelog-v4.1.0">版本</a>
</p>

```Shell
$ npm install svg-vuejs
```

## 在项目中引入并使用 vueSvg 组件

<p style="color: #5e6d82; font-size: 14px;">在 main.js 中写入以下内容:</p>

```js
// 当前位置 main.js

import Vue from 'vue';
import vueSvg from 'svg-vuejs'
import App from './App.vue';

Vue.use(vueSvg);

new Vue({
  el: '#app',
  render: h => h(App)
});
```

## 文件存放目录结构说明

<p style="color: #5e6d82; font-size: 14px;">
需要在项目根目录中的 src 文件夹下创建名为 svg 的文件夹，所有的 svg 文件都应该存放在 /src/svg/ 下，也可以在 svg 文件夹下继续创建文件夹用于区分管理图片。
</p>

```
├── build
├── config
├── src
│   │── assets
│   │── components
│   │── router
│   │── svg                  手动创建 （必须）   
│   │   ├── 子文件夹            可选创建
│   │   └── 子文件夹            可选创建
│   │   └── *.svg
│   │   └── *.svg
│   │   └── *.svg
│   │   └── *.svg
│   │   └── ...
│   │── App.vue
│   └── main.js
│
├── static
├── .babelrc
├── .editorconfig
├── .eslintignore
├── .eslintrc.js
├── .gitignore
├── .postcssrc.js
├── index.html
├── package.json
└── README.md
```


## 在页面中使用

<p style="color: #5e6d82; font-size: 14px;">
由于在 main.js 入口文件出全局引入并启用了 vueSvg 组件，所以在项目下所有的 vue 页面中, 都可以直接使用。
</p>

```vue
<!-- 当前位置 *.vue -->

<!-- 将会在 src 文件夹中 的 svg 文件夹里，寻找到名为 icon 的文件夹，渲染文件名为 wechat.svg 的图片 -->
<vue-svg name="wechat" path="icon/"></vue-svg>
```
