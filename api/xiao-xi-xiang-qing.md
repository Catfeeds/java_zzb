# 消息详情

### **API名称**

消息详情

### **路径**

> information/{id}

---

### **支持格式**

json

### **HTTP请求方式**

get

### **是否需要登录**

true

### **行为描述**

通过get方式向服务器发送请求，返回页面显示消息详情

### **输入参数**

| 字段名 | 中文名 | 说明 | 数据类型 |
| :--- | :--- | :--- | :--- |
| id | 消息id |  | int |

#### **示例**

```javascript
 {host}information/1
```

### **输出参数**

| 字段名 | 中文名 | 说明 | 字段类型 |
| :--- | :--- | :--- | :--- |
| result | 结果 | 成功返回'0'，失败返回'1' | int |
| description | 描述 | 结果返回'1'时为错误信息 | String |
| title | 消息标题 |  | String |
| content | 消息内容 |  | String |
| messageChildUuid | 子表消息uuid |  | String |

#### **示例**

```javascript
{
    "head": {
        "returnCode": "000",
        "returnDescription": "验证通过",
        "sysTime": "2016-06-06 14:56:43"
    },
    "body": {
        "result": "0",
        "description": "查询成功", 
        "tittle": "",
        "content": "",
        "messageChildUuid": "",
        "userUuid": "",
        "id": ""
    }
}
```



