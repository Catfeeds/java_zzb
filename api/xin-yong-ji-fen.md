# 信用积分

### **API名称**

信用积分

### **路径**

> user/cerditScore

---

### **支持格式**

无

### **HTTP请求方式**

get

### **是否需要登录**

true

### **行为描述**

通过get方式查询用户信用积分

### **输入参数**

|  |  |  |  |
| :--- | :--- | :--- | :--- |
|  |  |  |  |
|  |  |  |  |

#### **示例**

```javascript

```

### **输出参数**

| 字段名 | 中文名 | 说明 | 字段类型 |
| :--- | :--- | :--- | :--- |
| result | 结果 | 成功返回'0'，失败返回'1' | int |
| description | 描述 | 结果返回'1'时为错误信息 | String |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
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



