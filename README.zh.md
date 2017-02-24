# 代码笔记

代码阅读笔记  

## webpack.config.js

定义了webpack打包的文件输出路径，以及export webConfig、weexConfig两个变量

```
var webConfig = getBaseConfig()
webConfig.output.filename = '[name].web.js'
webConfig.module.loaders[1].loaders.push('vue')

var weexConfig = getBaseConfig()
weexConfig.output.filename = '[name].weex.js'
weexConfig.module.loaders[1].loaders.push('weex')

module.exports = [webConfig, weexConfig]
```
## package.json  
定义了包的依赖以及各个npm命令
```
    "build": "webpack",
    "dev": "webpack --watch",
    "copy:android": "cp dist/index.weex.js android/app/src/main/assets/index.js",
    "copy:ios": "cp dist/index.weex.js ios/assets/index.js",
    "copy": "npm run copy:android && npm run copy:ios",
    "serve": "serve -p 8080",
    "test": "echo \"Error: no test specified\" && exit 1"
```
## router.js
定义了vue router   
```
// Story view factory
function createStoriesView (type) {
  return {
    name: `${type}-stories-view`,
    render (createElement) {
      return createElement(StoriesView, { props: { type }})
    }
  }
}
```
上一段代码待细看

## entry.js
入口JS?  
导入了各个JS文件，注册mix混合，注册store和route到子component，在任意地方使用this.$router和this.$store  

## App.vue
定义<router-view>，导出back函数

## /views /store
views文件夹定义不同的页面，包含了components中提供的基本页面    
store文件夹定义了基本的函数，如fetch函数  
mixins文件夹定义了jump函数，用于页面跳转(基于router实现)  
filters定义了一些util函数  
components文件夹定义了一些基本的vue  
dist文件夹保存了生成的js文件  

> 注：/components和/views需细看
>vuex
