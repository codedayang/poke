#### 总览

构建

```
yarn
```

运行

```
yarn run dev:weapp
```

打包

```
yarn run build:weapp
```

生成页面模板

```
yanr run tpl 页面名
```

#### 目录结构

├─config	taro编译配置
└─src 
    ├─components	无state组件
    ├─config	小程序配置（服务端地址，常量、开关等）
    ├─models	dva模型（可能两个页面共享的状态可以放进这里）
    ├─pages	页面
    │  ├─index	（页面配置.config.ts、页面文件.tsx、页面样式.scss）
    │  └─test
    ├─service	网络请求
    ├─static	静态文件
    │  └─css	全局样式
    │  └─images	图片
    └─utils	一些封装（网络请求、dva）

#### note

如果一个状态不会在多个页面之间共享，可以不写model，自己更新状态