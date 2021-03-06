# 发送验证码

### **API名称**

```
 发送验证码
```

### **路径**

> user/captcha/{phone}

---

### **支持格式**

```
无
```

### **HTTP请求方式**

get

### **是否需要登录**

```
false
```

### **行为描述**

```
通过get方法向手机发送验证码，进行登录验证。
```

### **输入参数**

| 字段名 | 中文名 | 说明 | 数据类型 |
| :--- | :--- | :--- | :--- |
| phone | 手机号 | 用户手机号 | String |

#### **示例**

```javascript
 {host}user/captcha/15088648205
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
        "description": "发送验证码成功",

    }
}
```



