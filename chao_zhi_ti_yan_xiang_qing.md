# 超值体验详情

### **API名称**

     超值体验详情

### **路径**

 >    premium_experience/detail

***
###  **支持格式**

   json

###  **HTTP请求方式**

   post

###  **是否需要登录**


    true


### **行为描述** 

    通过post方式发送请求，返回超值体验数据


### **输入参数**

|字段名|中文名|说明|数据类型|
|:---|:---|:---|:---|
|articleUuid|超值体验记录uuid||String|
#### **示例**


```javascript
 {
     "head": {
        "user_uuid": ""
    },
    "body":{
        "articleUuid": ""
     }
}
```

### **输出参数**

|字段名|中文名|说明|字段类型|
|:---|:---|:---|
|result|结果|成功返回'0'，失败返回'1'|int|
|description|描述|结果返回'1'时为错误信息|String|

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
        "result": "0"
    }
}
```