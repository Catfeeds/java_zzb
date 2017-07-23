# 我的资料

### **API名称** {#api名称}

我的资料

### **路径** {#路径}

user/info/{user_uuid}

---

### **支持格式** {#支持格式}

json

### **HTTP请求方式** {#http请求方式}

post

### **是否需要登录** {#是否需要登录}

```
yes
```

### **行为描述** {#行为描述}

```
通过get方式发送请求，返回用户信息。
```

### **输入参数** {#输入参数}

| 字段名 | 中文名 | 说明 | 数据类型 |
| :--- | :--- | :--- | :--- |
| user_uuid | 消费者uuid |  | String |

#### **示例** {#示例}

```
 user/info/12584562555
```

### **输出参数** {#输出参数}

| 字段名 | 中文名 | 说明 | 字段类型 |
| :--- | :--- | :--- | :--- |
| result | 结果 | 成功返回'0'，失败返回'1' | int |
| description | 描述 | 结果返回'1'时为错误信息 | String |
| user_uuid | uuid |  | String |
| user_name | 姓名 |  | String |
| avater | 头像 |  | String |
| user_phone | 手机号 |  | String |
| id_picture | 证件类型 | 证件照片 | string |
| id_number | 证件号 |  | String |
| driving | 驾龄 |  | int |
| constellation | 星座 |  | String |
| authentication_status | 车主认证状态 | 1：未认证；2：已认证', | int |
| zm_open_id | 芝麻信用id |  | String |
| wx_open_id | 我的微信 |  | String |
| qq_open_id | 我的qq |  | String |

#### **示例** {#示例}

```
{
    {
     "head": {
        "returnCode": "000",
        "returnDescription": "验证通过",
        "sysTime": "2016-09-29 11:06:47"
    },
    "body": {
        "description": "登录成功",
        "result": "0",
        "user_uuid":"",
        "user_name":"",
        "avater":"",
        "user_phone":"",
        "id_picture":"",
        "id_number":"",
        "driving":"",
        "constellation":"",
        "authentication_status":"",
        "zm_open_id":"",
        "wx_open_id":"",
        "qq_open_id":""
    }

}
}
```



