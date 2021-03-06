# 坦克大战复刻版（Battle City Remake）

游戏地址: [http://shinima.pw/battle-city/](http://shinima.pw/battle-city/)

游戏详细介绍见知乎专栏文章: [https://zhuanlan.zhihu.com/p/35551654](https://zhuanlan.zhihu.com/p/35551654)

该 GitHub 仓库的版本是经典坦克大战的复刻版本，基于原版素材，使用 React 将各类素材封装为对应的组件。素材使用 SVG 进行渲染以展现游戏的像素风，可以先调整浏览器缩放再进行游戏，1080P 屏幕下使用 200% 缩放为最佳。此游戏使用网页前端技术进行开发，主要使用 React 进行页面展现，使用 Immutable.js 作为数据结构工具库，使用 redux 管理游戏状态，以及使用 redux-saga/little-saga 处理复杂的游戏逻辑。

目前游戏仍在开发中，只支持单人游戏，AI 设置不太合理。如果游戏过程中发现任何 BUG 的话，欢迎提 [issue](https://github.com/shinima/battle-city/issues/new)。(\*^\_^\*)

### 开发进度：

<details>
  <summary><b>Milestone 0.2 已完成</b></summary>

* [x] 游戏的基本框架
* [x] 给游戏中各个元素设置正确的生命周期
* [x] 从自定义的关卡中直接开始游戏
* [x] Gallery 页面重构
* [x] 已知 BUG 修复（有一部分难以重现的 BUG 被跳过了）

</details><br>

**Milestone 1.0（2018 暑假之后继续开发）**

* [x] 渲染性能优化
* [ ] 更合理的电脑玩家
* [ ] 完整的游戏音效
* [ ] 双人模式
* [ ] 完整的设计、开发文档

### 本地开发版本

1.  克隆该项目到本地目录
2.  运行 `yarn install` 来安装依赖 （或者使用 `npm install`）
3.  运行 `yarn start` 开启 webpack-dev-server，并在浏览器中打开 `localhost:8080`
4.  运行 `yarn build` 来打包生产版本，打包输出在 `build/` 文件夹下

`devConfig.js` 包含了一些开发用的配置项，注意修改该文件中的配置之后需要重启 webpack-dev-server
