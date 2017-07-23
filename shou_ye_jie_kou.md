# 首页

### **API名称**

     首页

### **路径**

 >    home_page

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
|banners/imgUrl|图片|轮播图|String|
|banners/linkUrl|链接url|轮播图|String|
|premiumExperience/carName|车名|超值体验|String|
|premiumExperience/price|价格|超值体验|String|
|premiumExperience/imgUrl|图片|超值体验|String|
|premiumExperience/linkUrl|链接|超值体验|String|
|newCarModel/carName|车名|新鲜车型|String|
|newCarModel/price|价格|新鲜车型|String|
|newCarModel/linkUrl|链接|新鲜车型|String|
|newCarModel/imgUrl|图片|新鲜车型|String|
|carModel/tittle|标题|车型专区|String|
|carModel/imgUrl|图片|车型专区|String|
|carModel/linkUrl|链接|车型专区|String|
|guessLike/carName|车名|猜你喜欢|String|
|guessLike/price|价格|猜你喜欢|String|
|guessLike/linkUrl|链接|猜你喜欢|String|
|guessLike/imgUrl|图片|猜你喜欢|String|
|recentBrowse/carName|车名|最近浏览|String|
|recentBrowse/price|价格|最近浏览|String|
|recentBrowse/linkUrl|链接|最近浏览|String|
|recentBrowse/imgUrl|图片|最近浏览|String|

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
        "banners": [
            {
                "imgUrl": "图片",
                "linkUrl": "http://fastask.oss-cn-hangzhou.aliyuncs.com/410ae0ffb34fb59dd132732b657434f2.jpg"
            },
            {
                "imgUrl": "图片",
                "linkUrl": "http://fastask.oss-cn-hangzhou.aliyuncs.com/789d6a91afc099cc9e6953f8d50a8c01.jpg"
            }
        ],
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
        ],
        "newCarModel": [
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
        ],
        "carModel": [
            {
                "tittle": "",
                "imgUrl": "图片",
                "linkUrl": "http://fastask.oss-cn-hangzhou.aliyuncs.com/410ae0ffb34fb59dd132732b657434f2.jpg"
            },
            {
                "tittle": "图片",
                "imgUrl": "图片",
                "linkUrl": "http://fastask.oss-cn-hangzhou.aliyuncs.com/789d6a91afc099cc9e6953f8d50a8c01.jpg"
            }
        ],
        "guessLike": [
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
        ],
        "recentBrowse": [
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
