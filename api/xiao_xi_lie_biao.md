# 消息列表

### **API名称**

消息列表（分页）

### **路径**

> info\_list

---

### **支持格式**

json

### **HTTP请求方式**

post

### **是否需要登录**

true

### **行为描述**

通过post方式传入pageSize、pageIndex等参数，获取用户消息列表，包含是否已读等信息

### **输入参数**

| 字段名 | 中文名 | 说明 | 数据类型 |
| :--- | :--- | :--- | :--- |
| pageIndex | 当前请求页数 | 请求页数不大于总页数 | int |
| pageSize | 请求条数 |  | int |

#### **示例**

```javascript
 {
     "head": {
        "user_uuid": ""
    },
    "body":{
        "pageIndex": 1,
        "pageSize": 20
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
| infoList | 消息列表 |  |  |
| infoList/id | 消息id |  | int |
| infoList/tittle | 消息标题 |  | String |
| infoList/content | 消息内容 |  | String |
| infoList/isRead | 是否已读 | 1：未读；2：已读 | int |
| infoList/createAt | 创建时间 |  |  |
| infoList/messageChildUuid | 消息uuid |  | String |

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
        "infoList": [
            {
                "messageChildUuid": "",
                "tittle": "",
                "content": "",
                "isRead":"",
                "userUuid": "",
                "id": "",
                "createAt": ""
            },
            {
               "messageChildUuid": "",
                "tittle": "",
                "content": "",
                "isRead":"",
                "userUuid": "",
                "id": "",
                "createAt": ""
            }
        ]
    }
}
```



