npm 升级
npm install npm -g
nodejs 升级:
npm install -g n
查看npm版本:
npm -v
查看nodejs 版本:
node -v
node模块可以本地(局部安装)或全局安装,如果想全部安装,则使用link:
npm link(切换到要使用的目录)
nodejs 可以异步,但是并非一定是,比如:readFile和readFileSync,前者可以异步,后者不能.
异步:非阻塞
非异步:阻塞;使用时需要注意,要将其卸载回调函数中,即:
xxx.func1(args[],function(args[]){
    xxx;
});
则func1为回调函数;
