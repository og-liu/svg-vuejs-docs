## 文件名
### name
 - 必传
 - 类型: String
 - 描述: svg 文件名, 例如: `name="wechat"`, 那么在 `path` 指定的目录下就应当存在对应的 `wechat.svg` 文件, path 属性默认指向 `/src/svg/`

```vue
<vue-svg name="wechat"></vue-svg>
```

```
├── build
├── config
├── src
│   │── assets
│   │── components
│   │── router
│   │── svg                             手动创建 （必须）   
│   │   └── wechat.svg                  自己添加的 svg 文件，文件名必须与组件的 name 值一样
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


## 文件路径
### path
- 可选
- 类型: String
- 描述: svg 文件存放路径, 默认 svg 存放路径在 `/src/svg/` 下, 如果图片太多需要分组管理，可以在该目录下手动创建文件夹存, 这个 `path` 属性就是用于指定手动创建的文件夹的名称，如果有子文件夹使用 `/` 间隔, 最后一个文件夹名后面必须带上 `/` 表示路径结束，它将与 `name` 属性的值拼接成一串完整的路径。

```vue
<!-- 将会在 src 文件夹中 的 svg 文件夹里，寻找到名为 icon 的文件夹，渲染文件名为 wechat.svg 的图片 -->
<vue-svg name="wechat" path="icon/"></vue-svg>

<!-- 将会在 src 文件夹中 的 svg 文件夹里，寻找到名为 icon 的文件夹下面的名为 multiple 的文件夹，渲染文件名为 phone.svg 的图片 -->
<vue-svg name="phone" path="icon/multiple/"></vue-svg>
```

```
├── build
├── config
├── src
│   │── assets
│   │── components
│   │── router
│   │── svg
│   │   └── icon
│   │        └── multiple
│   │               └── phone.svg
│   │        └── wechat.svg
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


## 设置颜色
### color
- 可选
- 类型: String
- 描述: 用于设置 `单色图标` 的颜色，默认展示为 `单色图标`

```vue
<vue-svg name="wechat" color="red"></vue-svg>
<vue-svg name="wechat" color="#333333"></vue-svg>
<vue-svg name="wechat" color="rgba(255, 0, 255, 0.8)"></vue-svg>
```


## 启用多色图标
### multipleColor
- 可选
- 类型: Boolean
- 描述: 接收一个布尔值，用于决定是否展示 `多色图标`，`多色图标` 无法通过 `color` 属性改变图标颜色，除非图标原本就没有颜色

```vue
<vue-svg name="wechat" :multipleColor="true"></vue-svg>
<vue-svg name="wechat" :multipleColor="false"></vue-svg>
<vue-svg name="wechat" multipleColor></vue-svg>
```


## 设置宽度
### width
- 可选
- 类型: String or Number
- 描述: 单色图标、多色图标默认宽度为 20px, 如果需要改动尺寸则可以通过 `width` 和 `height` 属性来设置

```vue
<vue-svg name="wechat" :width="100"></vue-svg>
<vue-svg name="wechat" width="100"></vue-svg>
<vue-svg name="wechat" width="100" height="100"></vue-svg>
```

## 设置高度
### height
- 可选
- 类型: String or Number
- 描述: 单色图标、多色图标默认高度为 20px, 如果需要改动尺寸则可以通过 `width` 和 `height` 属性来设置

```vue
<vue-svg name="wechat" :height="100"></vue-svg>
<vue-svg name="wechat" height="100"></vue-svg>
<vue-svg name="wechat" width="100" height="100"></vue-svg>
```
