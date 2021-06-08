# electron-vue3-webpack

#### 介绍
electron-vue3-webpack构建的项目模板

#### 软件架构
.config: webpack打包配置文件
    
    dev.runner.js： 运行脚本

    pack.build.js： 打包脚本

    webpack.main.config.js： 主进程脚本配置

    webpack.renderer.config.js： 渲染脚本配置

src: 项目路径

    main:electron主进程目录

        index.js 主进程入口文件

    renderer: 渲染进程目录 （vue项目目录）

        route vue-router目录

        store vueX目录

        main.js 渲染进程入口文件

static: 静态资源路径('此处路径不会被打包，可以直接使用./访问路径')



#### 使用说明
请注意，再打包编译环境中，使用的是file://作为地址，无法使用histtory路由，且传统的Web网页路径也不可使用如：/，请求资源如src,href引用static下文件时，请使用./

1.  安装依赖

```
yarn install
```



2.  运行

```
npm run dev 
```



3.  编译

```
npm run build
```



#### 特点：
1.  形同VueCli基本的项目结构
2.  立即可用的 Vue 插件 (vue-router, vuex)
3.  开箱即用的Webpack配置
4.  less，less-loader预处理器
5.  开启热更新
6.  一键式NPM脚本
