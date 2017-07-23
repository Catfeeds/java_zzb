# 添加银行卡

### **API名称**

```
 添加银行卡
```

### **路径**

> addBankCard

---

### **支持格式**

```
json
```

### **HTTP请求方式**

post

### **是否需要登录**

```
true
```

### **行为描述**

```
通过post方式向服务器发送请求，实现用户添加绑定银行卡
```

### **输入参数**

| 字段名 | 中文名 | 说明 | 数据类型 |
| :--- | :--- | :--- | :--- |
| cardUserName | 持卡人姓名 |  | String |
| cardNumber | 银行卡号 |  | String |
| phone | 手机号 |  | String |

#### **示例**

```javascript
 {
     "head": {
        "user_uuid": ""
    },
    "body":{
        "cardUserName": "张三",
        "cardNumber": "123456789098832",
        "phone": "15089388235"
     }
}
```

### **输出参数**

| 字段名 | 中文名 | 说明 | 字段类型 |
| :--- | :--- | :--- | :--- |
| result | 结果 | 成功返回'0'，失败返回'1' | int |
| description | 描述 | 结果返回'1'时为错误信息 | String |

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
        "description": "添加银行卡成功",

    }
}
```



