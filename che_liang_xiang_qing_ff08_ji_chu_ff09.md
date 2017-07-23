# 车辆详情（基础）

### **API名称**

     车辆详情

### **路径**

 >    carList/detail

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
|city|城市||String|
#### **示例**


```javascript
 {
     "head": {
        "user_uuid": ""
    },
    "body":{
        "user_uuid": "",
        "city":""
     }
}
```



### **输出参数**

|字段名|中文名|说明|字段类型|
|:---|:---|:---|
|result|结果|成功返回'0'，失败返回'1'|int|
|description|描述|结果返回'1'时为错误信息|String|
|car_status|车量状态|1：审核中；2：审核成功；3：审核未通过|int|
|license_plate_number|车牌号|String|
|car_name|车名|String|
||||
|car_owner_name|车主姓名|String|
|register_time|车辆注册时间|date|
|driving_license_photo|行驶证照片|String|
|man_car_photo|人车合影||String|
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
        "car_status": "车量状态",
        "license_plate_number": "车牌号",
        "car_name":"车名",
        "car_owner_name":"车主姓名",
        "register_time":"车辆注册时间",
        "driving_license_photo":"行驶证照片",
        "man_car_photo":"人车合影"
           
    }
}
```