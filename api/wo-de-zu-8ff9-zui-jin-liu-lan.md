# 我的足迹

### **API名称**

我的足迹

### **路径**

> user/browse\_list

---

### **支持格式**

json

### **HTTP请求方式**

post

### **是否需要登录**

true

### **行为描述**

通过post方式传入pageSize、pageIndex等参数，获取用户足迹（浏览）列表

### **输入参数**

| 字段名 | 中文名 | 说明 | 数据类型 |
| :--- | :--- | :--- | :--- |
| pageIndex | 当前请求页数 | 请求页数不大于总页数 | int |
| pageSize | 请求条数 |  | int |

#### **示例**

```javascript
 {
     "head": {
        "user_uuid": ""
    },
    "body":{
        "pageIndex": 1,
        "pageSize": 20
     }
}
```

### **输出参数**

| 字段名 | 中文名 | 说明 | 字段类型 |
| :--- | :--- | :--- | :--- |
| result | 结果 | 成功返回'0'，失败返回'1' | int |
| description | 描述 | 结果返回'1'时为错误信息 | String |
| total | 总页数 |  | int |
| page | 当前页数 |  | int |
| browseList | 足迹列表 |  |  |
| browseList/id | 足迹id |  | int |
| browseList/carUuid | 车辆uuid |  | String |
| browseList/carBrand | 车辆品牌 |  | String |
| browseList/carNumber | 车牌号 |  | String |
| browseList/price | 租车价格 |  | double |
| browseList/address | 取车地址 |  | String |
| browseList/orderQuantity | 车辆接单量 |  | int |
| browseList/collection | 用户收藏量 |  | int |
| browseList/carImage | 车辆图片地址 |  | String |

#### **示例**

```javascript
{
    "head": {
        "returnCode": "000",
        "returnDescription": "验证通过",
        "sysTime": "2016-06-06 14:56:43"
    },
    "body": {
        "total": 1,
        "page": 1,
        "result": "0",
        "description": "查询成功",
        "browseList": [
            {
                "id":"",
                "carUuid": "",
                "carBrand": "",
                "carNumber": "",
                "price":"",
                "orderQuantity": "",
                "collection": "",
                "carImage": ""
            },
            {
                "id":"",
                "carUuid": "",
                "carBrand": "",
                "carNumber": "",
                "price":"",
                "orderQuantity": "",
                "collection": "",
                "carImage": ""
            }
        ]
    }
}
```



