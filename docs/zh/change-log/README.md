---
sidebar: auto
---

# 更新日志

## v1.2.0

* [ 修改 ] 新版首页
* [ 新增 ] 全局状态管理模块化并且重新设计了 API
* [ 新增 ] 全新的数据持久化 API
* [ 新增 ] 数据持久化现在不仅仅支持区分用户，还可以区分路由
* [ 新增 ] 路由快照功能
* [ 新增 ] 文档重构
* [ 新增 ] 菜单支持跳转到外部链接
* [ 修改 ] bug 修复
* [ 新增 ] 页面过渡动画设置加入全局状态管理并支持用户私有持久化
* [ 新增 ] $logAdd 和 $log 快速记录日志和打印日志，并提供演示页面
* [ 新增 ] 顶栏和侧边栏菜单支持 svg 图标

## v1.1.11

* [ 修改 ] 优化 v1.1.10 的更新代码
* [ 修改 ] 修正版本号

## v1.1.10

* [ 修改 ] 修复了多标签页使用右侧菜单关闭时的报错

## v1.1.9

* [ 新增 ] 优化了多标签页数据持久化取值逻辑，现在修改路由信息后，刷新页面时数据从持久化存储取值时会多经过一部数据处理，根据 name 字段匹配新的路由数据
* [ 新增 ] `d2adminUtilDb2VuexByUuid` 和 `d2adminUtilDb2Vuex` 新增第三个参数: handleFunction，该参数可以设置一个数据处理的回调函数，如果设置了该回调函数，在从持久化存储中取值时，如果成功取值，数据会首先经过该函数处理最后赋值到 store

## v1.1.8

* [ 新增 ] 增加了错误收集和日志收集功能
* [ 新增 ] 增加了一个表格示例页面
* [ 修改 ] bug 修复

## v1.1.7

* [ 修改 ] 多标签页右键菜单 bug 修复

## v1.1.6

* [ 新增 ] 新增加了多页控制组件 tab 按钮上的右键操作菜单，现在你可以在 D2Admin 中像使用浏览器一样操作多标签页

## v1.1.5

* [ 修改 ] vue-cli3 项目重构，目录调整
* [ 修改 ] 全局状态管理设计优化
* [ 修改 ] 多标签页操作全部转移至 vuex
* [ 修改 ] 修复了多标签页无法清除缓存的 bug
* [ 修改 ] bug fixed [#38](https://github.com/d2-projects/d2-admin/issues/38)
* [ 修改 ] bug fixed [#41](https://github.com/d2-projects/d2-admin/issues/41)
* [ 修改 ] 侧边栏和顶栏菜单数据控制转移到 vuex 集中管理
* [ 修改 ] 页面最小宽度设置
* [ 新增 ] d2-highlight 组件新增 format-html 参数
* [ 新增 ] 自动获取用户浏览器 UA
* [ 新增 ] playground 新增浏览器信息查看界面
* [ 修改 ] 登陆注销逻辑移至 vuex
* [ 新增 ] 登陆页面新增快速选择用户示例
* [ 新增 ] 侧边栏切换控制辑移至 vuex
* [ 新增 ] 判断手机浏览自动跳转至提示页面
* [ 修改 ] 侧边栏弹出菜单尺寸缩小以容纳更多菜单
* [ 修改 ] d2-container 组件重构，每种模式现都支持 scroll 属性以及 header footer 插槽
* [ 修改 ] 修复全屏按钮退出全屏状态不更新的 bug
* [ 修改 ] 修复多标签页缓存逻辑 bug
* [ 新增 ] 持久化存储根据系统版本区分数据，防止因更新导致数据错乱
* [ 新增 ] 注销画面灰度效果
* [ 新增 ] .d2-card 样式类，可以让 el-card 具有跟随主题变化的样式
* [ 新增 ] ElementUI 表格组件全部示例移植
* [ 新增 ] 全局状态管理 playground
* [ 新增 ] 用户私有持久化数据 playground
* [ 新增 ] 侧边栏和顶栏菜单设置 playground
* [ 新增 ] d2-container 组件 card 模式下 footer 样式优化
* [ 修改 ] 侧边栏折叠模式下弹出菜单尺寸缩小
* [ 修改 ] 默认取消了侧边栏的自定义滚动条显示
* [ 新增 ] cookie 读写包装
* [ 新增 ] 持久化存储读写包装，提供快速操作当前用户数据的 mutation
* [ 新增 ] 持久化存储读写包装，提供快速操作所有用户共享数据的 mutation
* [ 新增 ] 侧边栏折叠状态现在会根据用户区分记录，刷新页面保留之前的状态

## v1.1.4

* [ 修改 ] 全局状态管理设计优化
* [ 修改 ] 主题调优
* [ 新增 ] playground 模块，方便测试和展示一些功能实现方式/调用方法
* [ 新增 ] 灰度模式
* [ 新增 ] 多页模式
* [ 新增 ] 多页模式缓存
* [ 新增 ] 多页模式快速关闭（关闭左侧 右侧 全部 其它）
* [ 修改 ] 侧边栏滚动优化
* [ 新增 ] `d2-container` 填充模式自定义滚动条
* [ 新增 ] `d2-container` 组件卡片和隐形模式自定义滚动条
* [ 新增 ] 现在页面标题可以根据路由做出对应变化了
* [ 新增 ] 版本检查机制
* [ 新增 ] `d2-container` 隐形模式支持 header 插槽
* [ 新增 ] 版本检查可以设置为不显示提示框
* [ 新增 ] 集成 json 查看组件
* [ 新增 ] 添加了所有图表种类的演示页面
* [ 修改 ] 修改布局方式，解决了在 Firefox 上 better-scroll 初始化拿不到正确高度的 bug
* [ 新增 ] 右上角显示用户名，用户名持久存储

## v1.1.3

* [ 修复 ] 侧边栏在折叠时不显示的 bug
* [ 新增 ] v-charts 插件
* [ 新增 ] 一些演示图表（后续打算把 v-charts 文档上有示例性的演示都展示一下）
* [ 修改 ] D2Admin 经典主题颜色调整
* [ 新增 ] violet 主题
* [ 新增 ] 菜单图标
* [ 修改 ] 新制作了 Fork me 图片

## v1.1.2

* [ 修改 ] 删除了 G2 相关的依赖

## v1.1.1

* [ 修改 ] 删除了 G2 相关的代码（移除图表库）
* [ 优化 ] 侧边栏取值逻辑

## v1.1.0

* [ 修改 ] 顶栏和侧边栏菜单新的结构生成方式，新的方案使用 数据 + 递归组件 实现无限制多级菜单
* [ 修改 ] 路由注册回归最简单的写法
* [ 修复 ] 首次加载 loading 样式类名和程序内类名冲突，新的加载类名使用 d2-app-loading 前缀
* [ 修改 ] 所有类似 dd- 的样式前缀(包括自动注册图标的id前缀)统一改为 d2-
* [ 修复 ] 修复 d2-highlight 组件和 d2-markdown 组件的样式冲突
* [ 修改 ] 内置组件名称统一改为 d2- 前缀，统一使用横线连接 (kebab-case) 风格
* [ 修改 ] 顶栏 logo 阴影删除
* [ 新增 ] 主题系统
* [ 新增 ] 三个主题，分别为 d2admin 经典，简约线条，流星
* [ 修改 ] d2-markdown 组件 md 参数改名为 source
* [ 修改 ] 删除了 d2-markdown 组件中图片的白色背景
* [ 修改 ] 删除 timeago 插件，更换为更强大的 dayjs
* [ 新增 ] Tomorrow Night Blue 主题
* [ 修改 ] src/assets/style/public-class.scss 写法优化
* [ 新增 ] [vue-bigdata-table](https://github.com/lison16/vue-bigdata-table)组件
* [ 修复 ] 侧边栏内容超过一屏后显示错误
* [ 新增 ] 自定义滚动条演示页面
* [ 新增 ] 流星主题新增背景图片上层的半透明遮罩
* [ 修复 ] 主题设置失效bug
* [ 修复 ] router守卫验证登陆部分代码修改
* [ 修复 ] d2-container 组件改为同步注册（之前的异步注册会有 mounted 生命周期问题，即 slot 内的页面在 mounted 生命周期内拿不到 dom）
* [ 修复 ] d2-container 组件重构 flex 布局
* [ 新增 ] 404 page
* [ 新增 ] 顶栏联系方式
* [ 新增 ] 右键菜单组件
* [ 新增 ] 菜单配置支持空菜单（项目开发的时候有可能需要先把菜单做好查看效果）
* [ 优化 ] 页面左侧菜单滚动条优化
* [ 修复 ] CSS 边距工具类都加上了 `!important` 来保证在覆盖样式时生效
* [ 修复 ] IE11 兼容性修复

## v1.0.0

[https://github.com/d2-projects/d2-admin/releases/tag/v1.0.0](https://github.com/d2-projects/d2-admin/releases/tag/v1.0.0)

这是第一个版本，还有一点小问题，但是已经可用