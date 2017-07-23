# 上传身份证/驾照证 {#手机号登录}

### **API名称** {#api名称}

```
上传身份证/驾照证注册
```

### **路径** {#路径}

> user/info/{id_picture}

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
通过post请求，传入id_picture进行上传。
```

### **输入参数** {#输入参数}

| 字段名 | 中文名 | 说明 | 数据类型 |
| :--- | :--- | :--- | :--- |
| user_uuid | 消费者uuid |  | String |
| id_picture | 证件照片  | 用户证件照片  | String |

#### **示例** {#示例}

```
{

    "head": {},
    "body": {
        "id_picture": "",
        "user_uuid":""
    }
}
```

### **输出参数** {#输出参数}

| 字段名 | 中文名 | 说明 | 字段类型 |
| :--- | :--- | :--- | :--- |
| result | 结果 | 成功返回'0'，失败返回'1' | int |
| description | 描述 | 结果返回'1'时为错误信息 | String |
| id_picture | 证件照片  | 用户证件照片  | String |
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
        "id_picture":""
    }

}
```



