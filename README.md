# hello-dodo

## node >= 10.13.0

## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
- yarn mock
- yarn serve
```

### Compiles and minifies for production
```
yarn build
```

### Lints and fixes files
```
yarn lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

### 注意点
1. 嵌套子路由：
  - 父路由一定要有个模板文件，添加 `<router-view />` 用于展示里面的子路由内容
  - 子路由path一定一定一定不要加 '/' 前缀，否则匹配不到
2. mock数据安装：npm install -g json-server
3. 使用vuex-ts版本时，初始访问页面，getter上不一定有值，如果不做兼容会报错

### BUG
1. vue  Cannot convert object to primitive value
  - template上设置本该为string的值为对象

### 其他
1. ERROR: Failed to download Chromium r686378! Set "PUPPETEER_SKIP_CHROMIUM_DOWNLOAD" env variable to skip download.
  - npm config set puppeteer_download_host=https://npm.taobao.org/mirrors
  - node node_modules/puppeteer/install.js
