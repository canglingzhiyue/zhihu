# 知乎API

### 返回code常用状态码说明
|状态码|说明|
|--|--|
|0|仅表示请求成功|
|401004|用户不存在,请先开户|
|401005|用户被锁定|
|401017|次数用完|
|401018|token缺失|
|500001|系统内部异常|
|500002|请求有问题|

|已完成|等待添加|
|--|--|
|搜索推荐|✓|
|搜索结果|✓|
|评论列表|✓|
|二级评论|✓|
|回答列表|✓|
|其他|ㄨ(可定制)|

|全局参数|说明|
|--|--|
|cookie|web端cookie|
|token|访问凭证|

## 1.搜索推荐
```
/zh/searchSuggests
```
### 参数:
|参数名|类型|必选|说明|
|--|:--:|:--:|:--|
|kw|string|是|关键词|


## 2.搜索结果
```
/zh/searchResult
```
### 参数:
|参数名|类型|必选|说明|
|--|:--:|:--:|:--|
|kw|string|是|关键词|
|pageIndex|int|是|页数，默认1|
|nextUrl|string|否|请求链接，从第一页获取的下一页请求链接|


## 3.评论列表
```
/zh/commentsOne
```
### 参数:
|参数名|类型|必选|说明|
|--|:--:|:--:|:--|
|answerId|string|是|回答帖子ID|
|sortType|int|是|排序 1.默认 2.时间|
|pageIndex|int|是|页数，默认1|
|nextUrl|string|否|请求链接，从第一页获取的下一页请求链接,当pageIndex>1时必传|


## 4.二级评论列表
```
/zh/commentsReply
```
### 参数:
|参数名|类型|必选|说明|
|--|:--:|:--:|:--|
|commentId|string|是|评论ID|
|sortType|int|是|排序 1.默认 2.时间|
|pageIndex|int|是|页数，默认1|
|nextUrl|string|否|请求链接，从第一页获取的下一页请求链接,当pageIndex>1时必传|



## 5.问题所有回答Answers
```
/zh/answers
```
### 参数:
|参数名|类型|必选|说明|
|--|:--:|:--:|:--|
|qid|string|是|问题ID|
|sortType|int|是|排序 1.默认 2.时间|
|pageIndex|int|是|页数，默认1|
|nextUrl|string|否|请求链接，从第一页获取的下一页请求链接,当pageIndex>1时必传|



### 联系QQ:45497494
###
<img src="https://qr.api.cli.im/newqr/create?data=https%253A%252F%252Fqm.qq.com%252Fcgi-bin%252Fqm%252Fqr%253Fk%253DgsXU_14bQsI8BdSevrFzHU7vIYnRCnFQ%2526noverify%253D0&level=H&transparent=false&bgcolor=%23FFFFFF&forecolor=%23000000&blockpixel=12&marginblock=1&logourl=&logoshape=no&size=500&kid=cliim&key=211db538a2ba8c28441f5d952fe165db" width="20%">

~~### [小红书](https://github.com/canglingzhiyue/xiaohongshu)~~
~~### [抖音](https://github.com/canglingzhiyue/douyin)~~













