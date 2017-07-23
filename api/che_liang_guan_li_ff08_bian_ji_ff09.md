# 车辆管理（编辑）

### **API名称**

     车辆管理

### **路径**

 >   carList/detail/edit

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
|car_uuid|车辆uuid||String|

#### **示例**


```javascript
 {
     "head": {
        "car_uuid": ""
    },
    "body":{
        "car_uuid": ""
     }
}
```



### **输出参数**

|字段名|中文名|说明|字段类型|
|:---|:---|:---|
|result|结果|成功返回'0'，失败返回'1'|int|
|description|描述|结果返回'1'时为错误信息|String|
|car_owner_name|车主姓名|String|
|license_plate_number|车牌号|String|
|vehicle_identification_number|车架号|String|
|engine_number|发动机号|String|
|color|颜色|String|
|brand|品牌（车型）|String
|transmission_case|变速箱|String|
|register_time|车辆注册时间|date|
|city|城市|String|
|model_character|车型（类型）（SUV、轿跑等）|String|
|seat_number|座位数|int|
|displacement|排量|String|
|model_year|年款|
|model|款式（舒适型、时尚型等）|string|
|driving_license_photo|行驶证照片|String|
|man_car_photo|人车合影||String|
|car_uuid|车辆uuid|String|

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
        "car_owner_name":"",
        "license_plate_number":"",
        "vehicle_identification_number":"",
        "engine_number":"",
        "color":"",
        "brand":"",
        "transmission_case":"",
        "register_time":"",
        "city":"",
        "model_character":"",
        "seat_number":"",
        "displacement":"",
        "model_year":""
        "model":"",
        "driving_license_photo":"",
        "man_car_photo":"",
        "car_uuid":""
    }
}