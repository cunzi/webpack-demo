# webpack-demo

以下所有的代码和示例均来源于以下网站
[webpack](https://v4.webpack.docschina.org/guides/getting-started/)
起步

##首先初始化项目，并且准备基础代码素材。
* 初始化项目使用如下代码
``` bat
npm init -y
npm install webpack webpack-cli --save-dev
```
* 修改 package.json
``` json
{
    "name": "webpack-demo",
    "version": "1.0.0",
    "description": "",
+   "private": true,
-   "main": "index.js",
    "scripts": {
      "test": "echo \"Error: no test specified\" && exit 1"
    },
    "keywords": [],
    "author": "",
    "license": "ISC",
    "devDependencies": {
    "webpack": "^4.20.2",
    "webpack-cli": "^3.1.2"
    },
    "dependencies": {}
  }
```
现在你可以在浏览器中打开index.html文件了

## 创建一个 bundle
* 安装lodash 依赖
``` bat
npm install --save lodash
```
* npx命令打包
``` bat
npx webpack
```