# 申请添加车型

### **API名称**

     申请添加车型

### **路径**

 >   carList/detail/edit/apply

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
|apply_user_uuid|申请者uuid||String|

#### **示例**


```javascript
 {
     "head": {
        "apply_user_uuid": ""
    },
    "body":{
        "apply_user_uuid": ""
     }
}
```



### **输出参数**

|字段名|中文名|说明|字段类型|
|:---|:---|:---|
|result|结果|成功返回'0'，失败返回'1'|int|
|description|描述|结果返回'1'时为错误信息|String|
|brand_model|行驶证品牌型号|String|
|brand|品牌|String|
|car_series|车系|String|
|model_year|年款|String|
|transmission_case|变速箱|String|
|displacement|排量|String|
|car_model|车型|String|
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
        "brand_model":"",
        "brand":"",
        "car_series":"",
        "model_year":"",
        "transmission_case":"",
        "displacement":"",
        "car_model":"",
        
    }
}