# 发现详情

### **API名称**

```
 发现详情
```

### **路径**

> discover/particulars/{id}

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
通过get方法向服务器发送发现id，请求数据在页面展示发现详情信息。
```

### **输入参数**

| 字段名 | 中文名 | 说明 | 数据类型 |
| :--- | :--- | :--- | :--- |
| id | 文章id |  | int |

#### **示例**

```javascript
 {host}discover/particulars/1
```

### **输出参数**

| 字段名 | 中文名 | 说明 | 字段类型 |
| :--- | :--- | :--- | :--- |
| result | 结果 | 成功返回'0'，失败返回'1' | int |
| description | 描述 | 结果返回'1'时为错误信息 | String |
| title | 标题 |  | String |
| articlePicture | 封面图 |  | String |
| articleContent | 文章内容（正文） |  | String |
|  |  |  |  |

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
        "title":"",
        "articlePicture":"",
        "articleContent":"" 
    }
}
```



