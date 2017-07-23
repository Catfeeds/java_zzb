# 银行卡

### **API名称**

```
 银行卡
```

### **路径**

> bankCard\_List

---

### **支持格式**

```
json
```

### **HTTP请求方式**

get

### **是否需要登录**

```
true
```

### **行为描述**

```
通过get方法向服务器发送请求，查询用户绑定的银行卡
```

### **输入参数**

无

### **输出参数**

| 字段名 | 中文名 | 说明 | 字段类型 |
| :--- | :--- | :--- | :--- |
| result | 结果 | 成功返回'0'，失败返回'1' | int |
| description | 描述 | 结果返回'1'时为错误信息 | String |
| bankCardList | 银行卡列表 |  |  |
| bankCardList/id | 银行卡id |  | int |
| bankCardList/cardIcon | 银行卡图标 |  | String |
| bankCardList/cardType | 银行卡类型 |  | String |
| bankCardList/bank | 银行名称 |  | String |
| bankCardList/cardNumber | 银行卡号（后四位） |  | String |

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
        "bankCardList": [
            {
                "id": "",
                "cardIcon": "",
                "cardType": "",
                "bank":"",
                "cardNumber": ""
            },
            {
                "id": "",
                "cardIcon": "",
                "cardType": "",
                "bank":"",
                "cardNumber": ""

            }
        ]
    }
}
```



