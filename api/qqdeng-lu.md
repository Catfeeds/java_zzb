# QQ联合登录 {#qq联合登录}

### **API名称** {#api名称}

```
 qq联合登录

```

### **路径** {#路径}

> user/qq/login

### **支持格式** {#支持格式}

json

### **HTTP请求方式** {#http请求方式}

post

### **是否需要登录** {#是否需要登录}

```
false

```

### **行为描述** {#行为描述}

```
  通过post请求，进行QQ登录参见[QQ文档](http://wiki.open.qq.com/wiki/mobile/SDK%E4%B8%8B%E8%BD%BD)。

```

### **输入参数** {#输入参数}

| 字段名 | 中文名 | 说明 | 数据类型 |
| :--- | :--- | :--- | :--- |
| openid | 唯一标识 |  | String |
| nickname | 昵称 |  | String |
| headimgurl | 头像 |  | String |

#### **示例** {#示例}

```
{
    "head": {},
    "body": {
        "openid": "",
        "nickname": "",
        "headimgurl": ""
    }
}

```

### **输出参数** {#输出参数}

| 字段名 | 中文名 | 说明 | 字段类型 |
| :--- | :--- | :--- | :--- |
| result | 结果 | 成功返回'0'，失败返回'1' | int |
| description | 描述 | 结果返回'1'时为错误信息 | String |
| user\_uuid | 用户uuid |  | String |

#### **示例** {#示例}

```
{
    "head": {
        "returnCode": "000",
        "returnDescription": "验证通过",
        "sysTime": "2016-09-29 11:06:47"
    },
    "body": {
        "description": "登录成功",
        "result": "0",
        "user_uuid": "b78576329192051ed87a3178311afadb",
    }
}
```



