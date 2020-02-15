# Vue-element-admin-books

使用vue-element-admin为基础开发的`前端读书管理系统`。


将vue-element-admin部分内容删掉后。
## 项目结构
* api：接口请求
* assets：静态资源
* components：通用组件
* directive：自定义指令
* filters：自定义过滤器
* icons：图标组件
* layout：布局组件
* router：路由配置
* store：状态管理
* styles：自定义样式
* utils：通用工具方法
  * auth.js：token 存取
  * permission.js：权限检查
  * request.js：axios 请求封装
  * index.js：工具方法
* views：页面
* permission.js：登录认证和路由跳转
* settings.js：全局配置
* main.js：全局入口文件
* App.vue：全局入口组件


## 登录流程如下
![image](https://www.youbaobao.xyz/admin-docs/assets/img/login_process.58cab9a5.png)

### 路由和权限校验
![](https://www.youbaobao.xyz/admin-docs/assets/img/router_process.9acaa55e.png)