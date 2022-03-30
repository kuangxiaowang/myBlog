---
title: NPM指令
date: 2020-11-15 21:00:00
tags: 
      - 指令
      - 学习
categories: 指令
---

#### 一 npm 常用操作

##### 1.查看npm版本

```
npm -v
```

##### 2.查看当前电脑 IP 信息

```
ipconfig
```

##### 3.npm全局安装

```
-g：--global 的简写  全局安装
npm install jquery -g
```
<!-- more -->
##### 4.npm全局安装卸载

```
npm uninstall jquery -g
```

##### 5.npm运行

```
 npm start:npm run start 的简写
```

##### 6.npm本地安装-S

```
npm i xx -S：npm install xx --save 的简写
项目（运行时、发布到生产环境时）依赖；例：antd , element , react...
安装包信息会写入 dependencies 中
```

##### 7.npm本地安装-D

```
npm i xx -D：npm install xx --save-dev的简写
工程构建（开发时、“打包”时）依赖 ；例：xxx-cli , less-loader , babel-loader...
安装包信息写入 devDependencies 中
```

##### 7.   .npmrc文件

```
npm config edit
```



#### 二 nrm

##### 1.nrm安装

```
表示安装一个全局 nrm
npm i nrm -g
```

##### 2.nrm版本

```
nrm --version
```

##### 3.nrm检测镜像源地址

```
表示查看 nrm 镜像源地址网速
nrm test
```

##### 4. nrm查看镜像源地址

```
nrm ls
```

##### 5.nrm切换镜像源

```
表示切换到 taobao 镜像源地址
nrm use taobao
```

#### 三 vue脚手架 

##### 1.全局安装vue脚手架

```
npm i @vue/cli -g
```

##### 2.查看vue版本

```
vue --version
```

##### 3.全局安装yarn（vue创建项目可能需要yarn工具下载）

```
npm i yarn -g
```

##### 4.创建vue项目

```
vue create 项目名称
第一步 Manually select features 手动选择功能
第二步 Linter / Formatter 勾掉
      Babel,Choose Vue version 保留
      Router,Vuex, CSS Pre-processors（Sass/SCSS(with node-sass)） 按需选择
第三步 选择 2.x
第四步 Use history mode for router? 是使用history模式/否使用哈希模式 Y
第五步 选择 In package.json
第六步 Save this as a preset for future projects? 是否保存设置 N
```

##### 5.进入项目文件夹

```
cd 文件名
```

##### 6.启动项目

```
默认 npm run serve
```

#### 四 下载路由

```
npm i vue-router -S
```

#### 五 vueX

##### 1.vueX下载

```
npm i vuex -S
```

##### 2.持久化插件（本地存储）

```
npm i vuex-persistedstate -S
```

#### 六 下载swiper

```
npm i swiper@5.4.5 -S
```

#### 七 下载jquery

```
npm i jquery -S
```

#### 八 下载axios

```
npm i axios -S
```

#### 九 下载element-ui

```
npm i element-ui -S
```

#### 十  Json-server(模拟服务器)

##### 1.下载json-server

```
全局安装json-server
npm i json-server -g 
```

##### 2.启动json文件

```
进入json所在的文件夹运行cmd
json-server ./db.json
```

##### 3.编辑脚本到packjson文件里面启动json-server

```
scripts
	dev : json-server  文件地址   --port 3001   --host 192.168.8.74  --watch(json修改的时候自动重启)
```

#### 十一 mockjs  模拟数据

```
下载mockjs
npm i mockjs -S
```

#### 十二 创建package.json

```
创建package.json
npm init -y  
```

#### 十三 node-dev(每次修改文件，自动重启服务器)

##### 1. 下载node-dev

```
npm i node-dev -S
```

##### 2. 编辑启动命令到packjson文件里面

```
"scripts":{
	"dev" : "node-dev server(服务文件名.js后缀可省略)"(原来是"node server")
}
```

##### 3.启动服务

```
npm run dev
```

#### 十四 express(nodejs框架)

##### 1. 下载express

```
npm i express -S
```

##### 2. 下载express中间件（向req.body添加post请求参数，毫无用处，直接设置app.use(express.urlencoded());app.use(express.json());能达到一样效果，没用为啥要讲？）

```
npm i body-parser -S
```

##### 3.  下载md5(密码加密)

```
npm i md5 -S
```

##### 4. jsonwebtoken 插件(用户凭证token)    

```
下载jsonwebtoken 插件
npm i jsonwebtoken -S 
```

##### 5. multer 插件(上传文件)

```
npm i multer -S
```

#### 十五 express脚手架

##### 1.下载express生成器

```
全局安装express生成器
npm i express-generator -g
```

##### 2.创建express脚手架

```
express 项目名
```

#### 十六 mongodb(非关系型数据库)

##### 1. 添加全局环境

```
把C:\Program Files\MongoDB\Server\3.0\bin添加到环境变量的path中
```

##### 2. 在C盘建data/db文件夹

##### 3. 启动数据库

```
mongod(出现27017说明成功)
```

##### 3. 查看数据库

```
mongo(操作命令详见菜鸟MongoDB)
1 show dbs 查看数据库
2 use 数据库名 切换数据库，没有就创建
3 db 进入数据库
4 show collections 查看数据表
5 db.数据表名字.drop() 删除数据表
6 db.数据表名字.find() 查看数据表内容
7 db.数据表名字.remove({条件}) 删除数据表指定内容
```

#### 十七 mongoose(在nodejs里操作mongodb数据库)

```
下载mongoose
npm i mongoose -S
```

#### 十八 下载富文本编辑器

```
npm i wangeditor -S
```

#### 十九 webpack(打包工具 ,打包js,打包html,打包css,打包压缩图片)

##### 1. 下载webpack

```
全局安装webpack
npm i webpack@4.32.2 webpack-cli@3.3.2 -g
```

##### 2. 本地安装webpack

```
本地安装webpack
npm i webpack@4.32.2 webpack-cli@3.3.2 -D
```

##### 2.  打包css(在js中require css文件)

```
npm i style-loader css-loader -D
```

##### 3. 打包scss(在js中require scss文件)

```
npm i sass-loader node-sass -D
```

##### 4.  HtmlWebpackPlugin(自动生成HTML文件index.html)

```
npm install --save-dev html-webpack-plugin
```

##### 5. webpack-dev-server(webpack配置服务器)

```
npm i webpack-dev-server -D
```

#### 二十 快捷键

```
vbc+tab键   --Vue快捷键
rcc+tab键   --React快捷键
```

#### 二十一  react指令

##### 1. 创建react项目(脚手架)

```
进入要创建项目的文件夹，执行
npx create-react-app 项目名
```

##### 2. 在react脚手架中使用scss

```
npm i node-sass -S
```

##### 3. 在react脚手架中使用路由

```
npm i react-router-dom -S
```

##### 4. 在react脚手架中使用redux

```
下载redux
npm  i redux -S
使用redux中间件thunk(可以执行异步请求)
npm i redux-thunk -S
使用redux中间件logger(可以打印日志)
npm i redux-logger -S
```

##### 5.  在react脚手架中使用react-redux

```
下载redux
npm  i redux -S
下载react-redux
npm i react-redux -S
```

##### 6. 在react脚手架中使用Ant Design(UI框架)

```
下载Ant Design
npm i antd -S
```

#### 二十二 nuxt(vue的一种脚手架)

##### 1. 创建nuxt项目

```
npx create-nuxt-app 项目名
```

#### 二十三 anywhere

```
下载anywhere
npm i anywhere -g
npm i anywhere
启动anywhere
anywhere
```

#### 二十四 npm更改仓库源

```
云漾私服npm地址
npm config set registry http://10.0.60.5:8081/repository/npm-group/ 废弃
npm config set registry http://maven.00bang.cn:8081/repository/npm-group/
改为淘宝镜像
npm config set registry http://registry.npm.taobao.org/
改为npm官方地址
npm config set registry http://registry.npmjs.org
```

#### 二十五 工作

```
 切换开发分支
 git checkout master-branch-develop
```

#### 二十六 nvm

```
nvm 安装地址https://github.com/coreybutler/nvm-windows/releases/tag/1.1.7
(先卸载node，第一个目录为nvm安装位置，第二个为node安装位置)
nvm install 13.0.1    安装node.js 13.0.1版本 会安装对应版本的npm
nvm use 13.0.1        使用node.js 13.0.1版本
nvm install 14.16.0    安装node.js 14.16.0版本 会安装对应版本的npm
nvm use 14.16.0       使用node.js 14.16.0版本
```

#### 二十七 jsdoc

```
全局安装jsdoc
%sudo npm i -g jsdoc 
生成jsdoc文件
%jsdoc publisher/manager.js publisher/live.js 
```

#### 二十八 md文档生成html

```
全局安装i5ting_toc
sudo npm install i5ting_toc -g
生成同级目录文档
%i5ting_toc -f README.md  
```

#### 二十九 git配别名查看分支

```
git config --global alias.lol 'log --oneline --decorate --graph --all' 
```

#### 三十 thinkjs

```
npm install -g think-cli
安装完全局会有thinkjs命令
thinkjs new 项目名       创建一个thinkjs脚手架
thinkjs --help          查看thinkjs命令
```

#### 三十一 hexo

```
npm install -g hexo-cli    安装hexo脚手架
npm init                   创建hexo项目
进入项目hexo server         启动本地服务
hexo new "新文章"           创建一篇新博文
npm install hexo-deployer-git --save   安装部署依赖
hexo deploy                一键部署
注：需要设置deploy:
  type: git
  repo: git@github.com:kuangxiaowang/kuangxiaowang.github.io.git
  branch: main(必须是github仓库默认分支！！！)
```

