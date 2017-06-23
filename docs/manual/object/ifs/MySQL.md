# 对象 MySQL
mysql 数据库连接对象

使用 [db](../../module/ifs/db.md).open 或 [db](../../module/ifs/db.md).openMySQL 创建，创建方式：

```JavaScript
var msql = db.openMySQL("mysql://user:pass@host/db");
```

## 继承关系
<div class="inherits"><svg width="81pt" height="376pt" viewBox="0.00 0.00 81.00 376.00" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
<g id="graph0" class="graph" transform="scale(1 1) rotate(0) translate(4 372)">
<title>%0</title>
<polygon fill="#ffffff" stroke="transparent" points="-4,4 -4,-372 77,-372 77,4 -4,4"/>
<!-- object -->
<g id="node1" class="node">
<title>object</title>
<g id="a_node1"><a xlink:href="object.md" xlink:title="object">
<polygon fill="#ffffff" stroke="transparent" points="8,-276 8,-368 65,-368 65,-276 8,-276"/>
<polygon fill="none" stroke="#000000" points="8.5,-346 8.5,-368 65.5,-368 65.5,-346 8.5,-346"/>
<text text-anchor="start" x="23.6625" y="-354" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">object</text>
<polygon fill="none" stroke="#000000" points="8.5,-276 8.5,-346 65.5,-346 65.5,-276 8.5,-276"/>
<text text-anchor="start" x="13.5" y="-332" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> dispose()</text>
<text text-anchor="start" x="13.5" y="-320" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> equals()</text>
<text text-anchor="start" x="13.5" y="-308" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> toString()</text>
<text text-anchor="start" x="13.5" y="-296" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> toJSON()</text>
<text text-anchor="start" x="13.5" y="-284" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> valueOf()</text>
</a>
</g>
</g>
<!-- DbConnection -->
<g id="node2" class="node">
<title>DbConnection</title>
<g id="a_node2"><a xlink:href="DbConnection.md" xlink:title="DbConnection">
<polygon fill="#ffffff" stroke="transparent" points="0,-114 0,-240 73,-240 73,-114 0,-114"/>
<polygon fill="none" stroke="#000000" points=".5,-218 .5,-240 73.5,-240 73.5,-218 .5,-218"/>
<text text-anchor="start" x="5.3255" y="-226" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">DbConnection</text>
<polygon fill="none" stroke="#000000" points=".5,-196 .5,-218 73.5,-218 73.5,-196 .5,-196"/>
<text text-anchor="start" x="5.5" y="-204" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> type</text>
<polygon fill="none" stroke="#000000" points=".5,-114 .5,-196 73.5,-196 73.5,-114 .5,-114"/>
<text text-anchor="start" x="5.5" y="-182" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> close()</text>
<text text-anchor="start" x="5.5" y="-170" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> begin()</text>
<text text-anchor="start" x="5.5" y="-158" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> commit()</text>
<text text-anchor="start" x="5.5" y="-146" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> rollback()</text>
<text text-anchor="start" x="5.5" y="-134" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> execute()</text>
<text text-anchor="start" x="5.5" y="-122" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> format()</text>
</a>
</g>
</g>
<!-- object&#45;&gt;DbConnection -->
<g id="edge1" class="edge">
<title>object-&gt;DbConnection</title>
<path fill="none" stroke="#000000" d="M36.5,-265.6596C36.5,-257.2593 36.5,-248.554 36.5,-240.0266"/>
<polygon fill="#000000" stroke="#000000" points="33.0001,-265.7224 36.5,-275.7224 40.0001,-265.7225 33.0001,-265.7224"/>
</g>
<!-- MySQL -->
<g id="node3" class="node">
<title>MySQL</title>
<g id="a_node3"><a xlink:title="MySQL">
<polygon fill="#d3d3d3" stroke="transparent" points="1.5,0 1.5,-78 71.5,-78 71.5,0 1.5,0"/>
<polygon fill="none" stroke="#000000" points="1.5,-56 1.5,-78 71.5,-78 71.5,-56 1.5,-56"/>
<text text-anchor="start" x="19.832" y="-64" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">MySQL</text>
<polygon fill="none" stroke="#000000" points="1.5,-22 1.5,-56 71.5,-56 71.5,-22 1.5,-22"/>
<text text-anchor="start" x="6.5" y="-42" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> rxBufferSize</text>
<text text-anchor="start" x="6.5" y="-30" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> txBufferSize</text>
<polygon fill="none" stroke="#000000" points="1.5,0 1.5,-22 71.5,-22 71.5,0 1.5,0"/>
<text text-anchor="start" x="6.5" y="-8" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> use()</text>
</a>
</g>
</g>
<!-- DbConnection&#45;&gt;MySQL -->
<g id="edge2" class="edge">
<title>DbConnection-&gt;MySQL</title>
<path fill="none" stroke="#000000" d="M36.5,-103.4693C36.5,-94.8023 36.5,-86.2311 36.5,-78.3058"/>
<polygon fill="#000000" stroke="#000000" points="33.0001,-103.6545 36.5,-113.6545 40.0001,-103.6545 33.0001,-103.6545"/>
</g>
</g>
</svg></div>

## 成员属性
        
### rxBufferSize
** Integer, 数据库连接接收缓存尺寸 **

```JavaScript
Integer MySQL.rxBufferSize;
```

--------------------------
### txBufferSize
** Integer, 数据库连接发送缓存尺寸 **

```JavaScript
Integer MySQL.txBufferSize;
```

--------------------------
### type
** String, 查询当前连接数据库类型 **

```JavaScript
readonly String MySQL.type;
```

## 成员函数
        
### use
** 选择当前数据库连接的缺省数据库 **

```JavaScript
MySQL.use(String dbName) async;
```

调用参数:
* dbName: String, 指定数据库名

--------------------------
### close
** 关闭当前数据库连接 **

```JavaScript
MySQL.close() async;
```

--------------------------
### begin
** 在当前数据库连接上启动一个事务 **

```JavaScript
MySQL.begin() async;
```

--------------------------
### commit
** 提交当前数据库连接上的事务 **

```JavaScript
MySQL.commit() async;
```

--------------------------
### rollback
** 回滚当前数据库连接上的事务 **

```JavaScript
MySQL.rollback() async;
```

--------------------------
### execute
** 执行一个 sql 命令，并返回执行结果 **

```JavaScript
DBResult MySQL.execute(String sql) async;
```

调用参数:
* sql: String, 格式化字符串，可选参数用 ? 指定。例如：'SELECT FROM TEST WHERE [id]=?'

返回结果:
* [DBResult](DBResult.md), 返回 sql 命令执行结果

--------------------------
** 执行一个 sql 命令，并返回执行结果，可根据参数格式化字符串 **

```JavaScript
DBResult MySQL.execute(String sql,
    ...);
```

调用参数:
* sql: String, 格式化字符串，可选参数用 ? 指定。例如：'SELECT FROM TEST WHERE [id]=?'
* ...: 可选参数列表

返回结果:
* [DBResult](DBResult.md), 返回 sql 命令执行结果

--------------------------
### format
** 格式化一个 sql 命令，并返回格式化结果 **

```JavaScript
String MySQL.format(String sql,
    ...);
```

调用参数:
* sql: String, 格式化字符串，可选参数用 ? 指定。例如：'SELECT FROM TEST WHERE [id]=?'
* ...: 可选参数列表

返回结果:
* String, 返回格式化之后的 sql 命令

--------------------------
### dispose
** 强制回收对象，调用此方法后，对象资源将立即释放 **

```JavaScript
MySQL.dispose();
```

--------------------------
### equals
** 比较当前对象与给定的对象是否相等 **

```JavaScript
Boolean MySQL.equals(object expected);
```

调用参数:
* expected: object, 制定比较的目标对象

返回结果:
* Boolean, 返回对象比较的结果

--------------------------
### toString
** 返回对象的字符串表示，一般返回 "[Native Object]"，对象可以根据自己的特性重新实现 **

```JavaScript
String MySQL.toString();
```

返回结果:
* String, 返回对象的字符串表示

--------------------------
### toJSON
** 返回对象的 JSON 格式表示，一般返回对象定义的可读属性集合 **

```JavaScript
Value MySQL.toJSON(String key = "");
```

调用参数:
* key: String, 未使用

返回结果:
* Value, 返回包含可 JSON 序列化的值

--------------------------
### valueOf
** 返回对象本身的数值 **

```JavaScript
Value MySQL.valueOf();
```

返回结果:
* Value, 返回对象本身的数值
