# 用户信息API文档


<a name="overview"></a>
## Overview
这里除了查看接口功能外，还提供了调试测试功能


### Version information
*Version* : 1.0


### Contact information
*Contact* : 王延飞


### URI scheme
*Host* : localhost:8080  
*BasePath* : /


### Tags

* UserApi : 用户基本信息操作API




<a name="paths"></a>
## Resources

<a name="userapi_resource"></a>
### UserApi
用户基本信息操作API


<a name="adduserusingpost"></a>
#### /addUser
```
POST /user/addUser
```


##### Description
添加一个用户


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**user**  <br>*required*|user|[User](#user)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[User](#user)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `application/json`


<a name="getuserusingget"></a>
#### /getUser
```
GET /user/getUser
```


##### Description
根据姓名查询用户信息


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Query**|**name**  <br>*required*|name|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[User](#user)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `application/json`




<a name="definitions"></a>
## Definitions

<a name="user"></a>
### User
用户信息描述


|Name|Description|Schema|
|---|---|---|
|**address**  <br>*optional*|家庭住址|string|
|**age**  <br>*optional*|年龄|integer (int32)|
|**id**  <br>*optional*|证件号|integer (int32)|
|**name**  <br>*optional*|姓名|string|
|**sex**  <br>*optional*|性别|string|





