# Client-pc 接口文档

baseUrl: http://localhost:8005

## 目录：

[1、用户登录](#1用户登录)<br/>
[2、个人资料](#2个人资料)<br/>

## 接口列表：

### 1、用户登录

#### 请求URL:  
```
http://localhost:8005/login
```

#### 示例：
 [http://localhost:8005/login](http://localhost:8005/login)

#### 请求方式: 
```
POST
```

#### 参数类型：query

|参数|是否必选|类型|说明|
|:-----|:-------:|:-----|:-----|
|mobile|Y        |string|      |
|password|Y        |string|      |

#### 返回示例：

```javascript
{
	"code": 0,
	"msg": "登陆成功",
	"data": {
		"token": "token"
	}
}
```
### 2、个人资料

#### 请求URL:  
```
http://localhost:8005/user/profile
```

#### 示例：
 [http://localhost:8005/user/profile](http://localhost:8005/user/profile)

#### 请求方式: 
```
POST
```

#### 参数类型：无

#### 返回示例：

```javascript
{
	"code": 0,
	"msg": "获取成功",
	"data": {
		"id": 2,
		"name": "zendevon",
		"mobile": "19911111111",
		"password": "e10adc3949ba59abbe56e057f20f883e",
		"photo": "http://localhost:8005/user/avatar/2",
		"gender": 1,
		"birthday": "2000-11-08T16:00:00.000Z",
		"real_name": "阿文",
		"intro": "234"
	}
}
```