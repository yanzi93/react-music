# 使用react实现音乐播放器

## 技术:
react 框架、懒加载、redux 数据管理、axios 数据通信、API 调用、跨域代理、ANT-Design-Mobile 第三方组件库使用等等

## 功能:
按歌手、歌曲名的维度进行搜索歌曲;
按条件标签展示歌曲列表;
实现了歌曲播放与歌词同步滚动以及开始、暂停、快进等等音乐播放器的基本功能; 
实现了通过 API 与后端的数据交互。

##目录
src
 - components
  - header                  //头部公共组件，包含顶层头部信息组件、返回组件、导航组件
  - playbottom              //音乐播放器组件，包含底部音乐播放器、歌词页面
  - tips                    //页面加载缓冲组件
  - getDataComponent.js     //数据请求高阶组件
- reducers
  - reducers.js   //处理action的状态改变
- router
  - config.js     //路由配置信息
- server
  - index.js  //封装axios请求方法
- style       //css，font，img等静态资源
- views       //展示页面
  - pnew      //新歌
  - plist     //歌单
  - rank      //排行
  - singer    //歌手
  - search    //搜索
  - common    //公共展示组件，包含详细信息、列表
  - routes.js //路由组件

##redux使用
歌曲列表组件和播放器组件通信使用redux。
原因： 组件嵌套复杂，相隔较远。
通信数据： 播放歌单，当前播放歌曲的hash

##懒加载使用
使用react的lozad组件，防止加载过多图片。
使用页面有歌单页面，歌手子页面中各类歌手页面。
只加载可是区域图片，未显示区域页面显示默认图片。




## 页面展示
![home](https://github.com/yanzi93/react-music/blob/master/showImg/home.png?raw=true)

![plist](https://github.com/yanzi93/react-music/blob/master/showImg/plist.png?raw=true)

![playing](https://github.com/yanzi93/react-music/blob/master/showImg/playing.png?raw=true)

![singer](https://github.com/yanzi93/react-music/blob/master/showImg/singer.png?raw=true)



