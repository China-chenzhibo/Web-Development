# 网站开发笔记
*陈志博 2022年3月*
##  安装环境
1. **用vscode让window端远程linux端**
- vscode远程ssh连接Liunx虚拟机 [remote-ssh](https://blog.csdn.net/fengxiaolu311/article/details/104774530/) 
2. **下载node**
- 用[nvm](https://github.com/nvm-sh/nvm)(node version manager)下载[node.js](https://nodejs.org/en/)  
- 安装前要先清之前node版本,如果遇到[nvm访问不到raw.githubusercontent](https://www.cnblogs.com/Walker-lyl/p/14251301.html) 
- 给hosts增加识别IP ,raw.githubusercontent的IP经常换,所以要[查询IP](https://zhuanlan.zhihu.com/p/107334179)
- 其中nvm的下载最好是用当前用户（非root用户）各管各的 否则后续很麻烦 需要[修改nvm和npm路径](https://blog.csdn.net/qq_36231887/article/details/100703861)./bashrc
- 给nvm切换[淘宝镜像] 并且npm用cnpm（不一定要用cnpm）代替(https://blog.csdn.net/qq_14815199/article/details/1046101630)
- 给npm切换[淘宝镜像](https://zhuanlan.zhihu.com/p/339812994)    
`npm config set registry https://registry.npm.taobao.org`
- 下载vscode插件vetur 为了高亮vue的代码

3. **vue-cli脚手架的安装**
- cli代表的是command line interact 下面进行cli的安装  
`npm install -g @vue/cli | vue create cats | cd cats | npm run serve`

- 让虚拟机开放8080端口供window端的浏览器访问  
`sudo ufw status | sudo ufw allow 8080| sudo ufw reload`
- 让vscode点击运行就可以自动运行npm run serve，点击vscode的运行-添加配置，自动生成lauch.json，修改里面的npm命令  
- 让vscode一运行就能自动打开网页，只需要在package.json里面的scripts-serve将"vue-cli-service serve"修改为"vue-cli-service serve --open"



- vue3对应的element plus

///未完待续...

