# 超值体验

### **API名称**

     超值体验

### **路径**

 >    premium_experience

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
|pageIndex|当前请求页数|请求页数不大于总页数|int|
|pageSize|请求条数||int|
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

|字段名|中文名|说明|字段类型|
|:---|:---|:---|
|result|结果|成功返回'0'，失败返回'1'|int|
|description|描述|结果返回'1'时为错误信息|String|
|total|总页数||int|
|page|当前页数||int|
|premiumExperience/carName|名称||String|
|premiumExperience/price|价格||String|
|premiumExperience/imgUrl|图片||String|
|premiumExperience/linkUrl|链接||String|


#### **示例**


```javascript
{
    "head": {
        "returnCode": "000",
        "returnDescription": "验证通过",
        "sysTime": "2016-08-11 09:39:33"
    },
    "body": {
        "total": 1,
        "page": 1,
        "description": "查询成功",
        "result": "0",
        "premiumExperience": [
            {
                "carName": "",
                "price": "",
                "imgUrl": "图片",
                "linkUrl": "http://fastask.oss-cn-hangzhou.aliyuncs.com/410ae0ffb34fb59dd132732b657434f2.jpg"
            },
            {
                "carName": "",
                "price": "",
                "imgUrl": "图片",
                "linkUrl": "http://fastask.oss-cn-hangzhou.aliyuncs.com/789d6a91afc099cc9e6953f8d50a8c01.jpg"
            }
        ]
    }
}
```
