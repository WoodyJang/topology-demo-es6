# topology-demo

es6+webpack 编译成 es5 的 js 的 demo

# Development

## 1. 安装依赖库

```
[demo#] yarn
# 或
[demo#] npm install

```

## 2. 编写 es6

需要使用 topology 的业务逻辑在 index.js 中，通过下面命令编译成 es5 的文件，使 index.html 直接使用。

```
# build
[demo#] npm run build

```

## 3.在 index.html 中使用

参考 index.html

# 如何在原生 html 的 es5 中使用

参考分支 es5。虽然推荐使用 es6，但仅仅只需灵活变通就可以在 es5 中使用。

## 步骤 1

[es5 分支] 在 index.html 中引入 topology.js

## 步骤 2

[es5 分支] 在 index.html 中添加 id 为"topo-canvas"的 div。id 必须为"topo-canvas"，不可修改。

```
<div class="canvas" id="topo-canvas"></div>
```

## 步骤 3

[es5 分支] 在 js 中使用 window.canvas 作为 es6 中 canvas 的实例即可：

```
window.canvas.render(data, true);
```

# License

MIT © le5le.com
