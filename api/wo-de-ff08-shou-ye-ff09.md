# 首页

### **API名称** {#api名称}

### 首页

### 路径

user/info/{user_uuid}
 
---

### **支持格式** {#支持格式}

json

### **HTTP请求方式** {#http请求方式}

get

### **是否需要登录** {#是否需要登录}

false

### **输入参数** {#输入参数}

yes

|  |  |  |  |
| :--- | :--- | :--- | :--- |
| user_uuid |uuid |  | String |

### **输出参数** {#输出参数}

| 字段名 | 中文名 | 说明 | 字段类型 |
| :--- | :--- | :--- | :--- |
| result | 结果 | 成功返回'0'，失败返回'1' | int |
| description | 描述 | 结果返回'1'时为错误信息 | String |
| user_uuid | uuid |  | String |
| headimgurl | 头像 |  | String |
| phone | 手机号 |  | String |
| riders_status | 车主认证状态 | 1 未认证； 2 已认证 | int |
| balance | 账号余额 |  |  |
|  | 订单评价 |  |  |
|  | 收藏车辆 |  |  |

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
        "user_uuid":"",
        "headimgurl": "",
        "result": "0",
        "phone":"",
        "riders_status":""
        "balance":""

    }

}
```



