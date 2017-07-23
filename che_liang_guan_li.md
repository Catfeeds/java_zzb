# 车辆管理

### **API名称**

     车辆管理

### **路径**

 >    carList

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
|user_uuid|用户uuid||String|

#### **示例**


```javascript
 {
     "head": {
        "user_uuid": ""
    },
    "body":{
        "user_uuid": ""
     }
}
```



### **输出参数**

|字段名|中文名|说明|字段类型|
|:---|:---|:---|
|result|结果|成功返回'0'，失败返回'1'|int|
|description|描述|结果返回'1'时为错误信息|String|
|man_car_photo|图片||String|
|brand|品牌|String
|license_plate_number|车牌号|String|
|car_status|车量状态|1：审核中；2：审核成功；3：审核未通过|int|
|car_uuid|车辆uuid|String|
|banner|轮播图|String|
|car_name|车名|String|
|car_type|1：出租；2：日常',|int|
|car_series|车系|String|
|model_character|车型（类型）（SUV、轿跑等）|String|
|model|款式（舒适型、时尚型等）|string|
|displacement|排量|String|
|manual_or_automatic|手/自动挡|1：自动；2：手动；3：手自一体'|int|
mileage|里程|int|
|address_map|取车坐标|String|
|address|取车地址|String|
|car_dsp|车辆描述|String|
|order_quantity|车辆接单量'|int|
|collection|用户收藏量|int|
|working_day_price|工作日价格|float|
|vehicle_age|车龄'|int|
|is_navigation|是否能外接mp3|1：能；2：不能'|int|
|vehicle_identification_number|车架号|String|
|weekend_price|周末价格|float|
|shelves_start_time|上架时间|date|
|engine_number|发动机号|String|
|seat_number|座位数|int|
|color|颜色|Sting|
|register_time|车辆注册时间|date|
|city|城市|String|
|driving_license_photo|行驶证照片|String|
|vehicle_delivery_mode|交付方式|int|
|car_owner_name|车主姓名|String|
|shelves_end_time|下架时间|date|
|lease_time|不可用时间列表|String|
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
        "carList": [
            {
                "man_car_photo": "图片",
                "brand": "品牌",
                "license_plate_number":"车牌号",
                "car_status":"车辆状态",
                "car_uuid":"车辆uuid",
                "banner":"轮播图",
                "car_name":"车名",
                "car_type":"",
                "car_series":"",
                .
                .
                .
            }
        ]
    }
}
```