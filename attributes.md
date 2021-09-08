## name
 - 必传
 - 类型: String
 - 描述: <br>svg 文件名, 例如: `name="wechat"`, 那么在 `/src/svg/` 目录下（包括子目录，具体根据 `path` 属性来确认）, 就应当存在对应的 `wechat.svg` 文件
 - 示例

```vue
<vue-svg name="wechat"></vue-svg>
```


## path

> v3.0.0 新增

- 可选
- 类型: String
- 描述: <br>svg 文件存放路径, 默认 svg 存放路径在 `/src/svg/` 下, 如果图片太多需要分组管理，可以在该目录下手动创建文件夹存, 这个 `path` 属性就是手动创建的文件夹的名称，如果有子文件夹使用 `/` 间隔, 最后一个文件夹名后面必须带上 `/` 表示路径结束，它将与 `name` 属性的值拼接成一串完整的路径。
- 示例

```vue
<!-- 将会在 src 文件夹中 的 default 文件夹里，寻找到名为 icon 的文件夹，渲染文件名为 wechat.default 的图片 -->
<vue-svg name="wechat" path="icon/"></vue-svg>
```

## type

- 可选
- 类型: String
- 描述: 类型，单色图标、多色图标、插画

## color
- 可选
- 类型: String
- 描述: 插画、多色图标无法使用 color 属性来控制颜色

## width
- 可选
- 类型: Number
- 描述: 单色图标、多色图标默认宽度为 20px

## height
- 可选
- 类型: String
- 描述: 单色图标、多色图标默认高度为 20px
