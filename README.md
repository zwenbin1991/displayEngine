#DisplayEngine重构

### 开发背景
&nbsp;&nbsp;&nbsp;&nbsp;参照了云哥的displayEngine PPT，自己重新理解并总结了现有状况的问题：
&nbsp;&nbsp;&nbsp;&nbsp;

* 代码编写规范；
* 架构设计不合理，底层支持不够。**备注**：应用层代码写入到底层；
* 解析大型JSON数据生成DOM性能开销大；
* 作品图片未使用预加载；
* 语义化的容器结构、优化上下、左右方向切屏动画；
* 数据返回非结构化；

所以在代码组织中使用模块化，保证各个功能之间独立性和可维护性，使用前端自动化构建工具提高开发效率和有效的发布资源，和后台开发人员讨论数据返回结构化，使用git进行代码托管、备份，遵循git flow模型对开发任务进行合理划分。

### 开发分析


### 设计原理