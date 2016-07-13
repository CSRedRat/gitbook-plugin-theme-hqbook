# DIY A Gitbook theme for hqbook

![Image](./_assets/preview.png)

## 使用方法

安装您的插件使用:

```bash
$ gitbook install
OR
$ npm i -D gitbook-plugin-theme-hqbook
```

将主题添加到您的图书配置 `book.json` 或者 `book.js`中:

```json5
{
    "plugins": [
        "theme-hqbook"
    ]
}
```

## 配置

整体配置

```json5
{
    "plugins": [
        "theme-hqbook"
    ],
    "variables": {
        "themeHqbook":{
            "nav":[
                {
                    "url": "https://www.baidu.com",
                    "target": "_blank",
                    "name": "百度一下"
                },
                // { ... }
            ]
        },
    },
    "pluginsConfig": {
        "theme-hqbook":{
            "favicon": "./favicon.ico",
            "logo":"./logo.png",
            "search-placeholder":"输入关键字搜索",
            "hide-elements": [
                ".summary .gitbook-link"
            ]
        }
    }
}
```

### favicon
自定义`favicon`地址，修改标题栏图标

### logo
自定义`logo`地址，修改logo

### search-placeholder
搜索框提示信息

### hide-elements
隐藏元素，比如导航栏中Published by GitBook

### nav
顶部导航栏，nav为数组，将需要的导航添加到变量`themeHqbook`中

## 推荐和以下插件配合使用

```
plugins: [
    "-highlight",
    "-lunr",
    "-search",
    "theme-hqbook",
    "chapter-fold",
    "code",
    "flexible-alerts",
    "lightbox",
    "prism",
    "splitter",
    "search-pro"
    //...
]
```

## 更新内容

### version 1.0.1 (2016-07-13T01:54:38)

* fix: 修改默认滚动条样式

### version 1.0.0 (2016-07-13T16:54:38)

* 创建和发布自开发Gitbook主题 theme-hqbook

## Keywords

[hqbook](https://github.com/HaoqiangChen/hqbook)
[gitbook](http://gitbook.com/)
[theme](https://github.com/HaoqiangChen/gitbook-plugin-theme-hqbook)

## License

[MIT](http://opensource.org/licenses/MIT)

Copyright (c) 2016-present, HaoqiangChen

