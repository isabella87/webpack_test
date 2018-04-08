# webpack 4.X 开发环境配置步骤



## 一，环境配置

1，创建工程目录（E:\webpack\webpack_test）； 
2，初始化工程目录：npm init。 
3，全局安装webpack-cli。 

?	`npm uninstall webpack-cli`
?	`npm install -g webpack-cli`

4，全局安装webpack。 

?	`npm uninstall webpack`
?	`npm install -g webpack`

5，webpack –mode development/production进行打包，可在package.json中配置dev和build的脚本，便只需运行npm run dev/build，作用相同。 
6，在webpack –mode development/production可串联设置其他参数。

7，其他参数配置

webpack --mode development --watch --progress --display-modules --colors --display-reasons



## 二，实例说明

1，创建src文件夹，并创建index.js入口文件（E:\webpack\webpack_test\src\index.js）

2，运行以下命令，打包以上文件，会生成打包后的文件main.js（E:\webpack\webpack_test\dist\main.js）

webpack –mode development/production

3，创建dist同级目录web并在其中创建文件index.html文件（E:\webpack\webpack_test\web\index.html），其中应用main,js文件，并用浏览器点击运行，查看页面效果。

打包完毕后只要dist和web两个文件夹内容即可实现页面的即时访问。



## 三，注意

1，`webpack4.x`以`'./src/index.js'`作为入口

2，`webpack4.x`以后，打包时不指定打包输出文件名和路径，会自动默认生成dist及生成main.js文件。 

也可以通过以下形式指定打包路径（最好别用）：

打包：npx webpack hello.js --output-filename hello.bundle.js --output-path . --mode development 
eg：
webpack hello.js --output-filename hello.bundle.js --output-path E:\webpack\webpack_test  --mode development



## 四，相关内容（当我不存在）

1，安装node
node -v

npm -v

2，安装并使用webpack
1）新建文件夹webpack/webpack_test
?	在该文件夹下运行 npm init
2）在以上文件夹下安装webpack
npm install webpack --save-dev

