# 在vue-cli基础上按需加载elementUI。

### 项目技术架构

*   Vue.js+Vuex+axios+Vue-router+elementUI


### @vue/cli3 element-ui 按需加载的配置

* 安装插件

npm i element-ui -S
npm install babel-plugin-component -D
npm install @babel/preset-env -D


* 修改 babel.config.js 为

>
module.exports = {
  "presets": [
    '@vue/app'
  ],
  "plugins": [
    [
      "component",
      {
        "libraryName": "element-ui",
        "styleLibraryName": "theme-chalk"
      }
    ]
  ]
}
