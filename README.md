#模仿的一个完整的vue-全家桶小项目
-----
时间：2017年8月26日星期六

##描述
-----
Vue-router处理路由
Axios做数据请求
Vuex管理组件间状态

##具体功能实现
-----
main.js  入口文件
routeConfig.js  路由配置文件

-----
+ main.js
  - 引入各插件，并use
  - 引入路由配置
  - 引入过滤器
  - 引入全局css
  - 一些其他的路由配置、axios配置
  - 挂载
+ routeConfig.js
  - 配置了header上三个路由、footer上三个路由
  - 中间是路由内容
+ App.vue
  - (loading)Header  Slider  Footer
  - 引用各部分拆分组件
  - 用watch监测路由变化
  - 用vuex和钩子函数监管操作动态
-----  
  
##vuex
-----
vuex单一状态树，用一个对象，包含全部的应用层级状态

+ State
  - 读取状态：在**计算属性**中返回某个状态
  - 从根组件中注册到所有子组件。通过**this.$store**访问
+ Getters  mapGetters
+ Mutations
  - 提交的事件
  - 同步事务
+ Action
  - 提交
  - 可以异步
  - 分发dispatch
  
  
-----
  
# simplenews

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build
```

For detailed explanation on how things work, consult the [docs for vue-loader](http://vuejs.github.io/vue-loader).
