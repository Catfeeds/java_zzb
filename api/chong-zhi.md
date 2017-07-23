# 充值

### **API名称**

```
 充值
```

### **路径**

> toRecharge

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
通过post方法向服务器发送请求，用户进行充值
```

### **输入参数**

| 字段名 | 中文名 | 说明 | 数据类型 |
| :--- | :--- | :--- | :--- |
| userUuid | 用户uuid |  | String |
| payType | 支付方式 | 1：支付宝；2：微信；3：银行卡 | int |
| money | 充值金额 |  | float |

#### **示例**

```javascript
 {
     "head": {
        "user_uuid": ""
    },
    "body":{
        "payType": 1,
        "money": 200
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
        "description": "充值成功",

    }
}
```



