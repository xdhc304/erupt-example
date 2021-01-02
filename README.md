<p align="center"><img src="https://www.erupt.xyz/demo/erupt.svg" height="150" alt="logo"/></p>
<h1 align="center"> Erupt 项目演示代码 </h1>

---

[码云仓库](https://gitee.com/erupt/erupt) &nbsp; | &nbsp; [github仓库](https://github.com/erupts/erupt) &nbsp; | &nbsp; 
[项目官网](https://www.erupt.xyz) &nbsp; | &nbsp; [使用文档](https://www.yuque.com/yuepeng/erupt) &nbsp; | &nbsp; 
[JavaDoc](https://apidoc.gitee.com/erupt/erupt/) &nbsp; | &nbsp; [环境搭建](https://www.yuque.com/yuepeng/erupt/tpq1l9) &nbsp; | &nbsp; 
[代码演示](https://www.erupt.xyz/#!/contrast) &nbsp; | &nbsp; [在线体验](https://www.erupt.xyz/demo)

### 使用方法：   
1. 前往 src/main/resources/application.yml 修改数据库连接配置
2. 前往 src/main/java/DemoApplication 运行main方法即可


### 将model下的类添加到菜单：

启动成功后，前往系统管理 → 菜单维护 → 新增，将已定义好的演示类添加到菜单中，填写数据如下：
  
| 菜单名称 |  菜单类型  | 类型值（类名） | 描述 |
|  ---- |  ----  | ----  | ----  |
| 入门示例 | 表格 | DemoSimple |  |
| 文章管理 | 表格 | Article |  |
| 树示例 | 树 | DemoTree |  |
| 组件示例 | 表格 | Components | 各类组件与事件代理使用方法 |
| 复杂示例 | 表格 | Complex | 动态下拉列表与定义按钮等功能 |


**配置项说明**
> 编码：确保唯一即可，建议是字母


### 常见问题
如果图片上传失败请前往 application.yml 修改 erupt.uploadPath 配置   
地图组件无法使用请前往 app.js 修改 eruptSiteConfig.amapKey 的值

### 目录说明
```lua
erupt-example
├── src.main
     ├── java -- 代码包
           └── com.example.demo
                ├── DemoApplication   -- 入口类
                └── model
                     ├──  DemoHyper   -- 复杂的示例
                     ├──  DemoSimple  -- 简单的示例
                     ├──  DemoTree    -- 树视图示例
                     └──  OperationHandlerImpl -- 按钮操作方法实现
     └── resources -- 配置包
           ├── application.yml -- 后台配置
           └── public
                ├── app.css    -- 前端样式
                ├── app.js     -- 前端配置
                └── home.html  -- 首页样式
└── pom.xml -- 依赖配置
```