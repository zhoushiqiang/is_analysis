<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# “注册”用例 [返回](../README.md)

## 1. 用例规约

|用例名称|注册|
|-------|:-------------|
|功能|注册平台|
|参与者|学生或老师|
|前置条件| |
|后置条件|注册成功后，跳转到登录页面|
|主事件流| 1. 输入用户名和密码，选择用户类型<br/>2.系统判断用户名，密码，用户类正确，允许注册<br/>3.系统在客户端以Cookie形式存储注册用户信息，保持注册的持久性。|
|备选事件流|1a. 输入的用户名或者密码为空 <br/>&nbsp;&nbsp; 1.提示重新输入 <br/> &nbsp;&nbsp; 2.重新提交注册信息 <br/>2a.系统判断用户名，密码，用户类不正确，不允许注册 <br/>&nbsp;&nbsp; 1.提示重新输入 <br/> &nbsp;&nbsp; 2.重新提交注册信息 |

## 2. 业务流程
无

## 3. 界面设计
- 界面参照: https://zhoushiqiang.github.io/is_analysis/test6/ui/adminregedit.html
- https://zhoushiqiang.github.io/is_analysis/test6/ui/sturegedit.html
- API接口调用
    - 接口1：[regedit](../接口/login.md)

## 4. 算法描述 [源码](../src/注册.puml)
![注册认证流程图](../img/基于GitHub的实验管理平台--注册用例的顺序图.png)
    
## 5. 参照表

- [USERS](../数据库表/数据库表.md/#USERS)
