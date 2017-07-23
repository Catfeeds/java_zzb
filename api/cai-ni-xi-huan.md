# 猜你喜欢

### **API名称**

```
 猜你喜欢
```

### **路径**

> like/{articleType}

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
通过get方式向服务器发送请求，查询猜你喜欢运营文章信息
```

### **输入参数**

| 字段名 | 中文名 | 说明 | 数据类型 |
| :--- | :--- | :--- | :--- |
| arcicleType | 类型 | 1：超值体验；2：新鲜车型；3：车型专区；4：猜你喜欢；5：发现 | int |

#### **示例**

```javascript
 {host}like/4
```

### **输出参数**

| 字段名 | 中文名 | 说明 | 字段类型 |
| :--- | :--- | :--- | :--- |
| result | 结果 | 成功返回'0'，失败返回'1' | int |
| description | 描述 | 结果返回'1'时为错误信息 | String |
| carList | 推荐车辆列表 |  |  |
| carList/id | 推荐车辆id |  | int |
| carList/carName | 推荐车辆名称 |  | String |
| carList/carBrand | 推荐车辆品牌 |  | String |
| carList/address | 取车地址 |  | String |
| carList/orderQuantity | 车辆接单量 |  | int |
| carList/collection | 用户收藏量 |  | int |
| carList/price | 租车价格 |  | float |
| carList/carImage | 车辆图片地址 |  | String |

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
        "carList":[
            {
                "id": "",
                "carName": "",
                "carBrand": "",
                "address": "",
                "orderQuantity": "",
                "collection": "",
                "price": "",
                "carImage": ""
            },
            {
                "id": "",
                "carName": "",
                "carBrand": "",
                "address": "",
                "orderQuantity": "",
                "collection": "",
                "price": "",
                "carImage": ""
            }
        ]
    }
}
```



