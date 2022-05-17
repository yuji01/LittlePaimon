<p align="center" >
  <a href="https://github.com/CMHopeSunshine/LittlePaimon/tree/nonebot2"><img src="https://cherishmoon.oss-cn-shenzhen.aliyuncs.com/LittlePaimon/readme/logo.png" width="256" height="256" alt="LittlePaimon"></a>
</p>
<h1 align="center">小派蒙|LittlePaimon</h1>
<h4 align="center">✨基于<a href="https://github.com/Ice-Cirno/HoshinoBot" target="_blank">HoshinoBot</a>|<a href="https://github.com/nonebot/nonebot2" target="_blank">NoneBot2</a>和<a href="https://github.com/Mrs4s/go-cqhttp" target="_blank">go-cqhttp</a>的原神Q群机器人✨</h4>

<p align="center">
    <a href="https://cdn.jsdelivr.net/gh/CMHopeSunshine/LittlePaimon@master/LICENSE"><img src="https://img.shields.io/github/license/CMHopeSunshine/LittlePaimon" alt="license"></a>
    <img src="https://img.shields.io/badge/Python-3.8+-yellow" alt="python">
    <a href="https://qun.qq.com/qqweb/qunpro/share?_wv=3&_wwv=128&inviteCode=MmWrI&from=246610&biz=ka"><img src="https://img.shields.io/badge/QQ频道交流-尘世闲游-green?style=flat-square" alt="QQ guild"></a>
</p>

## 简介

原神多功能机器人，通过米游社接口查询uid的游戏信息，并提供WIKI查询和各种各样的好玩的功能。

本README为NoneBot2版的介绍，Hoshino版详见：

+ [Github主页](https://github.com/CMHopeSunshine/LittlePaimon)
+ [README博客](https://blog.cherishmoon.fun/bot/LittlePaimon-hoshino.html)

## 功能示例

<img src="https://cherishmoon.oss-cn-shenzhen.aliyuncs.com/LittlePaimon/readme/ys.jpg" alt="ys">

<details>
<summary>角色背包</summary>
<img src="https://cherishmoon.oss-cn-shenzhen.aliyuncs.com/LittlePaimon/readme/ysa.jpg" alt="ysa">
</details>

<details>
<summary>角色详情</summary>
<img src="https://cherishmoon.oss-cn-shenzhen.aliyuncs.com/LittlePaimon/readme/ysc.jpg" alt="ysc">
</details>

<details>
<summary>深渊信息</summary>
<img src="https://cherishmoon.oss-cn-shenzhen.aliyuncs.com/LittlePaimon/readme/sy12.jpg" alt="sy">
</details>

<details>
<summary>模拟抽卡</summary>
<img src="https://cherishmoon.oss-cn-shenzhen.aliyuncs.com/LittlePaimon/readme/十连.jpg" alt="十连">
</details>

<details>
<summary>实时便签</summary>
<img src="https://cherishmoon.oss-cn-shenzhen.aliyuncs.com/LittlePaimon/readme/ssbq.jpg" alt="ssbq">
</details>

<details>
<summary>每月札记</summary>
<img src="https://cherishmoon.oss-cn-shenzhen.aliyuncs.com/LittlePaimon/readme/myzj.jpg" alt="myzj">
</details>

<details>
<summary>角色材料</summary>
<img src="https://cherishmoon.oss-cn-shenzhen.aliyuncs.com/LittlePaimon/readme/material.png" alt="material">
</details>

<details>
<summary>抽卡记录</summary>
<img src="https://cherishmoon.oss-cn-shenzhen.aliyuncs.com/LittlePaimon/readme/gachalog.jpg" alt="gachalog">
</details>

## 功能列表

详见[功能列表](https://blog.cherishmoon.fun/bot/NoneBot2FuncList.html)

## 部署方法
### 我很熟悉NoneBot2：

 + 部署NoneBot2和go-cqhttp

 + 克隆本项目
   - `git clone -b nonebot2 https://github.com/CMHopeSunshine/LittlePaimon `
   
 + 安装依赖
   - ```shell
     # 定时任务插件
     nb plugin install nonebot-plugin-apscheduler
     # 需要的依赖库
     pip install aiohttp xlsxwriter sqlitedict matplotlib aiofiles
     ```
 + 启用插件
   - ```python
     # 编辑bot.py，添加：
     nonebot.load_plugins("LittlePaimon")
     ```
     
### 我不熟悉NoneBot2：
**详细部署教程：**

- [Linux](https://blog.cherishmoon.fun/bot/NoneBot2Deploy.html#linux)
- [安卓系统](https://blog.cherishmoon.fun/bot/NoneBot2Deploy.html#%E5%9C%A8%E5%AE%89%E5%8D%93%E6%89%8B%E6%9C%BA%E4%B8%8A%E9%83%A8%E7%BD%B2)
- [Windows](https://blog.cherishmoon.fun/bot/NoneBot2Deploy.html#windows)

### 添加公共cookie

部署完成后，你还需要至少添加一条**公共cookie**，小派蒙才能使用查询功能。

登录米游社网页版，在地址栏粘贴：

```
javascript:(function(){prompt(document.domain,document.cookie)})();
```

复制得到的cookie，向小派蒙发送**`添加公共ck`**和粘贴的内容，即可开始使用

## 感谢

代码水平很烂，站在巨人的肩膀上努力学习ing......

- [NoneBot2](https://github.com/nonebot/nonebot2) - 跨平台异步机器人框架
- [go-cqhttp](https://github.com/Mrs4s/go-cqhttp) - Onebot标准的框架实现
- [Nwflower](https://github.com/Nwflower) - 部分图片的美工大大和武器攻略图提供
- [egenshin](https://github.com/pcrbot/erinilis-modules/tree/master/egenshin) - 参考了它的抽卡代码和资源
- [bluemushoom](https://bbs.nga.cn/nuke.php?func=ucp&uid=62861898) - 全角色收益曲线和参考面板攻略图来源
- [genshin-gacha-export](https://github.com/sunfkny/genshin-gacha-export) - 抽卡记录导出参考
- [西风驿站](https://bbs.mihoyo.com/ys/collection/307224) - 角色攻略一图流来源
- [游创工坊](https://space.bilibili.com/176858937) - 深渊排行榜数据来源
