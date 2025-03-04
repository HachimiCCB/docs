# 东方夜雀食堂wiki

## 项目介绍

本项目是一个基于​	微信小程序 / WXS响应式编程开发的关于游戏《东方夜雀食堂》的Wiki百科，后端使用微信云开发（数据库+云函数），其主要功能是：
- 采集与商人系统
- 菜谱与食材系统
- 顾客图鉴系统



## 小组成员及分工

| 姓名                                | 学号         | 分工                     |
| ----------------------------------- | ------------ | ------------------------ |
| [吴浥人](https://github.com/heiseisunset) | 2212190113 | 前端核心开发+扩展模块    |
| [金逸胜](https://github.com/RheinXenon)     | 2212190110 | 后端服务+基础设施        |



## 项目结构

```mermaid
mindmap
  root((TodoApp))
    技术栈
      前端
        WXML/WXSS/JavaScript（微信小程序框架）
        Vant Weapp（UI组件库）
        Lodash（数据处理）
      后端
        微信云开发（数据库/云函数）
        Node.js
      其他工具
        Git（版本控制）
        Markdown解析库
    功能模块
      ​菜谱与食材系统
        菜谱列表展示
        材料反向查询
        客人喜好匹配系统
        价格区间分类
      ​采集与商人系统
        采集地图导航
        商人库存监控
        采集效率计算器
      顾客图鉴系统
        角色图鉴
        符卡
        点单要求
        相关对话
      基础功能
        搜索栏与分类导航
    测试方案
      单元测试
        Jest(前端)
        pytest(后端)
      集成测试
        Postman
```
