# app1

[学习视频网址](https://www.bilibili.com/video/BV1Vf4y1T7bw?p=4)

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).


`**_jsconfig.json中给文件夹路径取别名_**
{ 
//编译程序任选项
"compilerOptions": {
//根目录
"baseUrl": "./",
//路径
"paths": {
“@”=>“src”
"@/*":[
"src/*"
]
}
},
//@不能在以下文件中使用
//exclude排除
"exclude": [
"node_modules",
"dist"
]
}`


`vue.config.js 关闭eslint校验工具
module.exports = {
// 关闭eslint校验工具
lintOnSave:false
}`

3.项目路由分析
vue-router
前端所谓路由:Kv键值对。
key: URL（地址栏中的路径)
value:相应的路由组件
注意:项目上中下结构
路由组件:
Home首页路由组件、
Search路由组件、
login登录路由、
Refister注册路由非路由组件:
Header【首页、搜索页】
Footer【在首页、搜索页】，但是在登录|注册页面没有