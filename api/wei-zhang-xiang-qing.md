# 违章详情

### **API名称**

违章详情

### **路径**

> \_list

---

### **支持格式**

json

### **HTTP请求方式**

post

### **是否需要登录**

true

### **行为描述**

通过post方式传入pageSize、pageIndex等参数，获取用户违章列表

### **输入参数**

| 字段名 | 中文名 | 说明 | 数据类型 |
| :--- | :--- | :--- | :--- |
| pageIndex | 当前请求页数 | 请求页数不大于总页数 | int |
| pageSize | 请求条数 |  | int |
| ticketStatus | 罚单状态 | 正在进行状态为1，已处理2 | int |

#### **示例**

```javascript
 {
     "head": {
        "user_uuid": ""
    },
    "body":{
        "pageIndex": 1,
        "pageSize": 20,
        "ticketStatus":1
     }
}
```

### **输出参数**

| 字段名 | 中文名 | 说明 | 字段类型 |
| :--- | :--- | :--- | :--- |
| result | 结果 | 成功返回'0'，失败返回'1' | int |
| description | 描述 | 结果返回'1'时为错误信息 | String |
| total | 总页数 |  | int |
| page | 当前页数 |  | int |
| ticketList | 违章列表 |  |  |
| ticketList/id | 违章id |  | int |
| ticketList/orderNumber | 订单号 |  | String |
| ticketList/address | 违章地址 |  | String |
| ticketList/illegalTime | 违章时间 |  | Date |
| ticketList/money | 罚款金额 |  | float |
| ticketList/points | 扣分 |  | int |
| ticketList/illegalCode | 违法行为代码 |  | String |
|  |  |  |  |
|  |  |  |  |

#### **示例**

```javascript
{
    "head": {
        "returnCode": "000",
        "returnDescription": "验证通过",
        "sysTime": "2016-06-06 14:56:43"
    },
    "body": {
        "total": 1,
        "page": 1,
        "result": "0",
        "description": "查询成功",
        "ticketList": [
            {
                "id":"",
                "orderNumber": "",
                "address": "",
                "illegalTime": "",
                "money":"",
                "points": "",
                "illegalCode": ""
            },
            {
                "id":"",
                "orderNumber": "",
                "address": "",
                "illegalTime": "",
                "money":"",
                "points": "",
                "illegalCode": ""
            }
        ]
    }
}
```



