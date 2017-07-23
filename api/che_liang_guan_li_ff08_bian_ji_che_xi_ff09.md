# 车辆管理（编辑车系）
### **API名称**

     车辆管理编辑车系

### **路径**

 >   carList/detail/edit/car_series

***
###  **支持格式**

   json

###  **HTTP请求方式**

   post

###  **是否需要登录**


    true


### **行为描述** 

    通过post方式发送请求，返回首页数据


### **输入参数**

|字段名|中文名|说明|数据类型|
|:---|:---|:---|:---|

|brand|品牌|String|

#### **示例**


```javascript
 {
     "head": {
        "brand": ""
    },
    "body":{
        "brand": ""
     }
}
```



### **输出参数**

|字段名|中文名|说明|字段类型|
|:---|:---|:---|
|result|结果|成功返回'0'，失败返回'1'|int|
|description|描述|结果返回'1'时为错误信息|String|
|jinkou|进口|ArrayList|
|jinkou/car_series|车系|String|
|guochan|国产|ArrayList|
|guochan/car_series|车系|String|
#### **示例**


```javascript
{
    "head": {
        "returnCode": "000",
        "returnDescription": "验证通过",
        "sysTime": "2016-08-11 09:39:33"
    },
    "body": {
        "description": "查询成功",
        "result": "0",
        "jinkou":[
          {
            "car_series":""
          }
        ],
        "guochan":[
          {
            "car_series":""
          }
        ]
    }
}
