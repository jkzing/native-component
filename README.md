# Demo: 在原生微信小程序中使用 mpvue 组件

把使用 mpvue 写的组件编译后在原生小程序中使用

理想情况使用`mpvue-simple`编译就好了，但是那个 cli 好像有点问题，先用个完整的工程 demo

## 运行

### 安装依赖

```bash
cd mp-components && npm i
npm run build
```

### 构建 mpvue 组件

```bash
# 在 mp-components 目录下
npm run build
```

### 把根目录导入微信开发者工具

