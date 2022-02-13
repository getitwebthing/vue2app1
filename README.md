# app1

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


jsconfig.json中给文件夹路径取别名

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

}


vue.config.js 关闭eslint校验工具
module.exports = {
// 关闭eslint校验工具
lintOnSave:false

}