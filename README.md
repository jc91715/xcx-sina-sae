# xcx-sina-sae

## 使用对象

小白用户，即使你不会代码。按着教程一步步配置，也可以运行一套包含前后端的小程序

## 使用之前
* 已有一个小程序[链接](https://mp.weixin.qq.com/cgi-bin/registermidpage?action=index&lang=zh_CN&token=)，（有个邮箱就可以申请）
* 注册[新浪sae](https://www.baidu.com/link?url=K0NWX_VBHhWcbo0bUKMs1VGEVAKVAWhsc-Yvo4yFrTilzn-Tq3rP931Hdg1A1_Jz&wd=&eqid=d5be52b600031955000000045c5d06c3)
* npm 已安装。安装起来，也很方便
## 为什么
当我们开发一款小程序的时候，对于初级用户的使用成本还是蛮大的，既要购买服务器，又要购买数据库，域名，还要备案。
这一整套下来，是让人很难受的，不能专心的去实现功能。有没有这样的一个平台，我只要把代码上传上去，它就可以运行，
成本可以低点就更好了。在我的开发过程中，我发现[新浪的sae](https://www.baidu.com/link?url=K0NWX_VBHhWcbo0bUKMs1VGEVAKVAWhsc-Yvo4yFrTilzn-Tq3rP931Hdg1A1_Jz&wd=&eqid=d5be52b600031955000000045c5d06c3)挺不错的，正好可以解决这一痛点

## 2 如何使用
该仓库的是小程序的前端仓库，使用[wepy](https://tencent.github.io/wepy/)框架，后端建议使用自己写的一个简单[mvc框架](https://github.com/jc91715/php-simple-mvc/tree/xcx-sina-sae)，

### 下载代码

```
git clone https://github.com/jc91715/xcx-sina-sae.git project
```
### 安装依赖

```
cd project && npm install
```
### 监听
```
npm run --watch
```

### 修改配置
在src/app.wpy 文件中
```
  globalData = {
    userInfo: null,
    domain: 'xxxx'
  }
  
```
xxx 改为你自己的域名，我的是jc91715.applinzi.com

### 打开小程序开发工具，指向dist目录，就可以运行了

## api接口

提供两个api接口，一个是获得文章列表，两一个是获得文章详情。
假如你的新浪sae配置好的话，访问 
* 文章列表https://yourdomain.com/xcx/posts 
* 文章详情 https://yourdomain.com/xcx/show/10 10是文章id 



