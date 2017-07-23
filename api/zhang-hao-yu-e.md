# 账户余额

### **API名称**

```
 账户余额
```

### **路径**

> findBalance/{id}

---

### **支持格式**

```
无
```

### **HTTP请求方式**

get

### **是否需要登录**

```
true
```

### **行为描述**

```
通过get方法向服务器发送请求，查询用户账户余额
```

### **输入参数**

| 字段名 | 中文名 | 说明 | 数据类型 |
| :--- | :--- | :--- | :--- |
| id | 用户id |  | int |

#### **示例**

```javascript
 {host}findBalance/1
```

### **输出参数**

| 字段名 | 中文名 | 说明 | 字段类型 |
| :--- | :--- | :--- | :--- |
| result | 结果 | 成功返回'0'，失败返回'1' | int |
| description | 描述 | 结果返回'1'时为错误信息 | String |
| balance | 账户余额 |  | float |
| frozenBlance | 冻结金额 |  | float |

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
        "balance": "",
        "frozenBlance": ""
    }
}
```



