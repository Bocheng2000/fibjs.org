# 对象 HttpCookie
HttpCookie 是 HTTP 协议封装的 cookie 对象，它提供了获取、设置 cookie 的各个属性，同时也支持多个 cookie 的组织与处理，是 [http.Request](../../module/ifs/http.md#Request) 和 [http.Response](../../module/ifs/http.md#Response) 两个对象都支持的一个重要属性

HttpCookie 对象有一些重要的属性，其中最重要的是 name，value 和 expires。其中，name 和 value 属性是必须设定的，name 属性为 cookie 的名称，value 属性为 cookie 的值。

```JavaScript
const http = require('http');

const cookie = new http.Cookie('my_cookie_name', 'my_cookie_value');
console.log(cookie.name, cookie.value); // my_cookie_name my_cookie_value
```

在上述的示例代码中，我们创建了一个名为 "my_cookie_name" 值为 "my_cookie_value" 的 cookie 对象，并使用 [console.log](../../module/ifs/console.md#log) 打印 cookie 对象的 name 和 value 属性的值。

除此之外，HttpCookie 对象还有 expires、domain、[path](../../module/ifs/path.md)、secure、httpOnly 等属性，可以指定 cookie 过期时间、访问路径、可访问域名、安全等级，cookie 仅允许 [http](../../module/ifs/http.md) 请求等等。

```JavaScript
const http = require('http');

const now = new Date();
const date = new Date(
    now.getFullYear(),
    now.getMonth(),
    now.getDate() + 1
);
const options = {
    name: 'my_cookie_name',
    value: 'my_cookie_value',
    expires: date,
    domain: 'localhost',
    path: '/',
    secure: true,
    httpOnly: true
};
const cookie = new http.Cookie(options);
console.log(cookie);
```

在上述示例代码中，我们创建了一个 cookie 对象，并指定了 cookie 的各种属性。我们先实例化了一个 Date 类型的变量 now，然后新建了一个 date 变量，它的值为明天这个时间点。options 是一个 JS 对象，其中包含了很多关键的属性，比如过期时间 expires、cookie 名称和值 name 和 value、cookie 生效域名 domain、cookie 生效路径 [path](../../module/ifs/path.md)，另有 cookie 安全选项 secure 和 [http](../../module/ifs/http.md)-only 两个属性。

在实际开发场景中，我们需要移除一个 cookie，可以将其过期时间设置为一个过去的时间，或者直接从 cookies 属性中删除。如：

```JavaScript
const http = require('http');

const cookie = new http.Cookie('my_cookie_name', 'my_cookie_value');
delete cookie.server; // delete server property
cookie.expires = -1; // set expires to -1
```

在上述示例代码中，我们使用了 delete 语句，移除了 cookie 对象的 server 属性（HTTP only cookie）。次外，为了移除最近添加的 cookie，我们将 expires 属性的值设置为 -1。

## 继承关系
```dot
digraph {
    node [fontname="Helvetica,sans-Serif", fontsize=10, shape="record", style="filled", fillcolor="white"];

    object [tooltip="object", URL="object.md", label="{object|toString()\ltoJSON()\l}"];
    HttpCookie [tooltip="HttpCookie", fillcolor="lightgray", id="me", label="{HttpCookie|new HttpCookie()\l|name\lvalue\ldomain\lpath\lexpires\lhttpOnly\lsecure\l|parse()\lmatch()\l}"];

    object -> HttpCookie [dir=back];
}
```

## 构造函数
        
### HttpCookie
**HttpCookie 构造函数，创建一个新的 HttpCookie 对象**

```JavaScript
new HttpCookie(Object opts = {});
```

调用参数:
* opts: Object, 指定创建的 cookie 的属性

opts 可以设置的选项如下：

```JavaScript
{
    "name": "", // specify the name of the cookie
    "value": "", // specify the value of the cookie
    "expires": Date, // specify the expires time of the cookie
    "domain": "", // specify the domain of the cookie
    "path": "", // specify the path of the cookie
    "secure": false, // specify the secure of the cookie
    "httpOnly": false, // specify the httpOnly of the cookie
}
```

--------------------------
**HttpCookie 构造函数，创建一个新的 HttpCookie 对象**

```JavaScript
new HttpCookie(String name,
    String value,
    Object opts = {});
```

调用参数:
* name: String, 指定创建的 cookie 名称
* value: String, 指定创建的 cookie 值
* opts: Object, 指定创建的 cookie 的其它属性

opts 可以设置的选项如下：

```JavaScript
{
    "expires": Date, // specify the expires time of the cookie
    "domain": "", // specify the domain of the cookie
    "path": "", // specify the path of the cookie
    "secure": false, // specify the secure of the cookie
    "httpOnly": false, // specify the httpOnly of the cookie
}
```

## 成员属性
        
### name
**String, 查询和设置 cookie 名称**

```JavaScript
String HttpCookie.name;
```

--------------------------
### value
**String, 查询和设置 cookie 的值**

```JavaScript
String HttpCookie.value;
```

--------------------------
### domain
**String, 查询和设置 cookie 的域名范围**

```JavaScript
String HttpCookie.domain;
```

--------------------------
### path
**String, 查询和设置 cookie 的路径范围**

```JavaScript
String HttpCookie.path;
```

--------------------------
### expires
**Date, 查询和设置 cookie 的过期时间**

```JavaScript
Date HttpCookie.expires;
```

--------------------------
### httpOnly
**Boolean, 查询和设置 cookie 是否仅允许 [http](../../module/ifs/http.md) 请求，缺省 false**

```JavaScript
Boolean HttpCookie.httpOnly;
```

--------------------------
### secure
**Boolean, 查询和设置 cookie 是否仅通过 https 传递，缺省 false**

```JavaScript
Boolean HttpCookie.secure;
```

## 成员函数
        
### parse
**解析给定的字符串，填充 cookie 对象**

```JavaScript
HttpCookie.parse(String header);
```

调用参数:
* header: String, 指定需要解析的 header 字符串

--------------------------
### match
**检测给定的 [url](../../module/ifs/url.md) 是否匹配当前设置**

```JavaScript
Boolean HttpCookie.match(String url);
```

调用参数:
* url: String, 指定测试的 [url](../../module/ifs/url.md)

返回结果:
* Boolean, 匹配成功返回 true

--------------------------
### toString
**返回对象的字符串表示，一般返回 "[Native Object]"，对象可以根据自己的特性重新实现**

```JavaScript
String HttpCookie.toString();
```

返回结果:
* String, 返回对象的字符串表示

--------------------------
### toJSON
**返回对象的 JSON 格式表示，一般返回对象定义的可读属性集合**

```JavaScript
Value HttpCookie.toJSON(String key = "");
```

调用参数:
* key: String, 未使用

返回结果:
* Value, 返回包含可 JSON 序列化的值

