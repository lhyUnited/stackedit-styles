# stackedit-styles

> 本项目灵感来自[stackedit](https://github.com/benweet/stackedit)

## 背景

stackedit提供了导出至html的功能，当我们查看导出后的静态html，发现在头部插入了


```html
<link rel="stylesheet" href="https://stackedit.io/style.css" />
```

所以，这个静态html的所有样式都来自于[https://stackedit.io/style.css](https://stackedit.io/style.css)

但是呢，为了达到最好的**访问速度**，静态资源最好能上cdn，所以就有了这个仓库。

## 介绍

没什么特别的，我只是把stackedit的源码拔了下来，build一下，把打包后的产物传到github，然后就可以通过jsdelivr访问静态资源了。

## 使用

- 用任何编辑器打开导出后的`*.html`
- 将

```html
<link rel="stylesheet" href="https://stackedit.io/style.css" />
```

替换成

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/lhyUnited/stackedit-styles@latest/style.css" />
```

- 保存

