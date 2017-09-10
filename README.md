# jhipster
jhipster 使用心得

# 官方教程: http://www.jhipster.tech

## 完整环境
~~~
NodeJs
Maven
Sonar
Docker
DB（Mysql）
~~~

## 完整环境

> 安装 npm

> 安装 yarn

> 安装 phantomjs-2.1.1-windows.zip

> 安装 jhipster

> jhipster 初始化项目

> npm install 加载包

## 编译、部署

> yarn install 前端编译

> yarn start 前端启动 （npm start 命令启动报错）

> yarn start --port=9001 出现端口冲突，请添加端口参数

> http://localhost:9060/ 前端访问，端口根据自己项目 webpack\webpack.dev.js 的 devServer 和 plugins 节点设置  

> mvn clean package 后端编译

> java -jar target/*.war 后端启动 （Spring boot）

## 踩过的坑
~~~
1、安装时 phantomjs-2.1.1-windows.zip 下载慢或无法下载
2、npm start 启动报错，解决方式是安装 yarn-1.0.1.msi
3、yarn 启动端口冲突，执行yarn install后，使用yarn start --port=9001启动 （src\main\docker\sonar.yml 和 webpack\webpack.dev.js）文件中端口9000冲突
~~~
