## 本项目实现的最终作用是基于SSH个人记账本
## 分为2个角色
### 第1个角色为管理员角色，实现了如下功能：
 - 用户管理
 - 管理员登录
 - 管理员管理
### 第2个角色为用户角色，实现了如下功能：
 - 个人信息管理
 - 年收支查询
 - 月收支查询
 - 用户登录
 - 记账管理
## 数据库设计如下：
# 数据库设计文档

**数据库名：** ssh_jizhang

**文档版本：** 


| 表名                  | 说明       |
| :---: | :---: |
| [admin](#admin) | 管理员表 |
| [tong](#tong) |  |
| [user](#user) | 用户表 |
| [zhang](#zhang) |  |

**表名：** <a id="admin">admin</a>

**说明：** 管理员表

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | id |   int   | 10 |   0    |    N     |  Y   |       | 自增主键  |
|  2   | name |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 名字  |
|  3   | pass |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 密码  |

**表名：** <a id="tong">tong</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | id |   int   | 10 |   0    |    N     |  Y   |       | 自增主键  |
|  2   | user |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  3   | type |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 类型  |
|  4   | kind |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  5   | date |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 日期  |
|  6   | year |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  7   | month |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 月份  |
|  8   | shou |   int   | 10 |   0    |    Y     |  N   |   NULL    |   |
|  9   | zhi |   int   | 10 |   0    |    Y     |  N   |   NULL    |   |

**表名：** <a id="user">user</a>

**说明：** 用户表

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | id |   int   | 10 |   0    |    N     |  Y   |       | 自增主键  |
|  2   | name |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 名字  |
|  3   | sex |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 性别  |
|  4   | age |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 年龄  |
|  5   | pass |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  6   | tel |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 电话  |
|  7   | rname |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  8   | adddate |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 添加时间  |

**表名：** <a id="zhang">zhang</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | id |   int   | 10 |   0    |    N     |  Y   |       | 自增主键  |
|  2   | name |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 名字  |
|  3   | user |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  4   | rname |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  5   | TYPE |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 类型  |
|  6   | kind |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  7   | date |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 日期  |
|  8   | count |   int   | 10 |   0    |    Y     |  N   |   NULL    | 数量  |
|  9   | yong |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  10   | info |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |

