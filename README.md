# vue-admin-template

[English](./README-en.md) | [简体中文](./README-zh.md)

> 使用[vue-admin-template]进行学习前台整合以及vue相关技术，本项目作为学习记录
>
> A minimal vue admin template with Element UI & axios & iconfont & permission control & lint

**项目代码:** <https://github.com/taoweidong/vue-admin-template>

# 2019年10月24日

- 克隆仓库，开始学习

- node-sass 安装失败的原因以及解决方法：https://segmentfault.com/a/1190000010984731?utm_source=tag-newest

- 修改git仓库地址：<https://blog.csdn.net/oLeiShen/article/details/84032089>

- 项目代码结构

  ├── build                      // 构建相关  
  ├── config                     // 配置相关
  ├── src                        // 源代码
  │   ├── api                    // 所有请求
  │   ├── assets                 // 主题 字体等静态资源
  │   ├── components             // 全局公用组件
  │   ├── directive              // 全局指令
  │   ├── filtres                // 全局 filter
  │   ├── icons                  // 项目所有 svg icons
  │   ├── lang                   // 国际化 language
  │   ├── mock                   // 项目mock 模拟数据
  │   ├── router                 // 路由
  │   ├── store                  // 全局 store管理
  │   ├── styles                 // 全局样式
  │   ├── utils                  // 全局公用方法
  │   ├── vendor                 // 公用vendor
  │   ├── views                   // view
  │   ├── App.vue                // 入口页面
  │   ├── main.js                // 入口 加载组件 初始化等
  │   └── permission.js          // 权限管理
  ├── static                     // 第三方不打包资源
  │   └── Tinymce                // 富文本
  ├── .babelrc                   // babel-loader 配置
  ├── eslintrc.js                // eslint 配置项
  ├── .gitignore                 // git 忽略项
  ├── favicon.ico                // favicon图标
  ├── index.html                 // html模板
  └── package.json               // package.json