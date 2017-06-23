# 对象 Handler
消息处理器接口

## 继承关系
<div class="inherits"><svg width="442pt" height="514pt" viewBox="0.00 0.00 442.00 514.00" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
<g id="graph0" class="graph" transform="scale(1 1) rotate(0) translate(4 510)">
<title>%0</title>
<polygon fill="#ffffff" stroke="transparent" points="-4,4 -4,-510 438,-510 438,4 -4,4"/>
<!-- object -->
<g id="node1" class="node">
<title>object</title>
<g id="a_node1"><a xlink:href="object.md" xlink:title="object">
<polygon fill="#ffffff" stroke="transparent" points="165,-414 165,-506 222,-506 222,-414 165,-414"/>
<polygon fill="none" stroke="#000000" points="165.5,-484 165.5,-506 222.5,-506 222.5,-484 165.5,-484"/>
<text text-anchor="start" x="180.6625" y="-492" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">object</text>
<polygon fill="none" stroke="#000000" points="165.5,-414 165.5,-484 222.5,-484 222.5,-414 165.5,-414"/>
<text text-anchor="start" x="170.5" y="-470" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> dispose()</text>
<text text-anchor="start" x="170.5" y="-458" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> equals()</text>
<text text-anchor="start" x="170.5" y="-446" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> toString()</text>
<text text-anchor="start" x="170.5" y="-434" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> toJSON()</text>
<text text-anchor="start" x="170.5" y="-422" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> valueOf()</text>
</a>
</g>
</g>
<!-- Handler -->
<g id="node2" class="node">
<title>Handler</title>
<g id="a_node2"><a xlink:title="Handler">
<polygon fill="#d3d3d3" stroke="transparent" points="153,-312 153,-378 234,-378 234,-312 153,-312"/>
<polygon fill="none" stroke="#000000" points="153.5,-356 153.5,-378 234.5,-378 234.5,-356 153.5,-356"/>
<text text-anchor="start" x="176.4985" y="-364" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">Handler</text>
<polygon fill="none" stroke="#000000" points="153.5,-334 153.5,-356 234.5,-356 234.5,-334 153.5,-334"/>
<text text-anchor="start" x="158.5" y="-342" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">  new Handler()</text>
<polygon fill="none" stroke="#000000" points="153.5,-312 153.5,-334 234.5,-334 234.5,-312 153.5,-312"/>
<text text-anchor="start" x="158.5" y="-320" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> invoke()</text>
</a>
</g>
</g>
<!-- object&#45;&gt;Handler -->
<g id="edge1" class="edge">
<title>object-&gt;Handler</title>
<path fill="none" stroke="#000000" d="M193.5,-403.6502C193.5,-394.8735 193.5,-386.0612 193.5,-378.0314"/>
<polygon fill="#000000" stroke="#000000" points="190.0001,-403.8877 193.5,-413.8877 197.0001,-403.8878 190.0001,-403.8877"/>
</g>
<!-- AsyncWait -->
<g id="node3" class="node">
<title>AsyncWait</title>
<g id="a_node3"><a xlink:href="AsyncWait.md" xlink:title="AsyncWait">
<polygon fill="#ffffff" stroke="transparent" points="0,-185 0,-229 57,-229 57,-185 0,-185"/>
<polygon fill="none" stroke="#000000" points=".5,-207 .5,-229 57.5,-229 57.5,-207 .5,-207"/>
<text text-anchor="start" x="5.388" y="-215" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">AsyncWait</text>
<polygon fill="none" stroke="#000000" points=".5,-185 .5,-207 57.5,-207 57.5,-185 .5,-185"/>
<text text-anchor="start" x="5.5" y="-193" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> end()</text>
</a>
</g>
</g>
<!-- Handler&#45;&gt;AsyncWait -->
<g id="edge2" class="edge">
<title>Handler-&gt;AsyncWait</title>
<path fill="none" stroke="#000000" d="M143.3345,-325.7962C118.0319,-314.2465 88.1948,-297.5713 66.5,-276 53.2141,-262.7898 43.2654,-243.9575 36.887,-229.3039"/>
<polygon fill="#000000" stroke="#000000" points="142.222,-329.1311 152.7835,-329.9713 145.0512,-322.7282 142.222,-329.1311"/>
</g>
<!-- Chain -->
<g id="node4" class="node">
<title>Chain</title>
<g id="a_node4"><a xlink:href="Chain.md" xlink:title="Chain">
<polygon fill="#ffffff" stroke="transparent" points="75.5,-174 75.5,-240 147.5,-240 147.5,-174 75.5,-174"/>
<polygon fill="none" stroke="#000000" points="75.5,-218 75.5,-240 147.5,-240 147.5,-218 75.5,-218"/>
<text text-anchor="start" x="98.4425" y="-226" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">Chain</text>
<polygon fill="none" stroke="#000000" points="75.5,-196 75.5,-218 147.5,-218 147.5,-196 75.5,-196"/>
<text text-anchor="start" x="80.5" y="-204" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">  new Chain()</text>
<polygon fill="none" stroke="#000000" points="75.5,-174 75.5,-196 147.5,-196 147.5,-174 75.5,-174"/>
<text text-anchor="start" x="80.5" y="-182" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> append()</text>
</a>
</g>
</g>
<!-- Handler&#45;&gt;Chain -->
<g id="edge3" class="edge">
<title>Handler-&gt;Chain</title>
<path fill="none" stroke="#000000" d="M168.697,-303.2584C156.7062,-283.0787 142.513,-259.1926 131.265,-240.263"/>
<polygon fill="#000000" stroke="#000000" points="165.7417,-305.1366 173.859,-311.9456 171.7595,-301.5608 165.7417,-305.1366"/>
</g>
<!-- HandlerEx -->
<g id="node5" class="node">
<title>HandlerEx</title>
<g id="a_node5"><a xlink:href="HandlerEx.md" xlink:title="HandlerEx">
<polygon fill="#ffffff" stroke="transparent" points="165.5,-168 165.5,-246 221.5,-246 221.5,-168 165.5,-168"/>
<polygon fill="none" stroke="#000000" points="165.5,-224 165.5,-246 221.5,-246 221.5,-224 165.5,-224"/>
<text text-anchor="start" x="170.164" y="-232" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">HandlerEx</text>
<polygon fill="none" stroke="#000000" points="165.5,-190 165.5,-224 221.5,-224 221.5,-190 165.5,-190"/>
<text text-anchor="start" x="170.5" y="-210" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> handler</text>
<text text-anchor="start" x="170.5" y="-198" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> stats</text>
<polygon fill="none" stroke="#000000" points="165.5,-168 165.5,-190 221.5,-190 221.5,-168 165.5,-168"/>
<text text-anchor="start" x="170.5" y="-176" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> onerror()</text>
</a>
</g>
</g>
<!-- Handler&#45;&gt;HandlerEx -->
<g id="edge4" class="edge">
<title>Handler-&gt;HandlerEx</title>
<path fill="none" stroke="#000000" d="M193.5,-301.8151C193.5,-284.0088 193.5,-263.5224 193.5,-246.1589"/>
<polygon fill="#000000" stroke="#000000" points="190.0001,-301.9455 193.5,-311.9456 197.0001,-301.9456 190.0001,-301.9455"/>
</g>
<!-- Routing -->
<g id="node8" class="node">
<title>Routing</title>
<g id="a_node8"><a xlink:href="Routing.md" xlink:title="Routing">
<polygon fill="#ffffff" stroke="transparent" points="240,-138 240,-276 321,-276 321,-138 240,-138"/>
<polygon fill="none" stroke="#000000" points="240.5,-254 240.5,-276 321.5,-276 321.5,-254 240.5,-254"/>
<text text-anchor="start" x="263.7735" y="-262" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">Routing</text>
<polygon fill="none" stroke="#000000" points="240.5,-232 240.5,-254 321.5,-254 321.5,-232 240.5,-232"/>
<text text-anchor="start" x="245.5" y="-240" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">  new Routing()</text>
<polygon fill="none" stroke="#000000" points="240.5,-138 240.5,-232 321.5,-232 321.5,-138 240.5,-138"/>
<text text-anchor="start" x="245.5" y="-218" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> append()</text>
<text text-anchor="start" x="245.5" y="-206" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> all()</text>
<text text-anchor="start" x="245.5" y="-194" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> get()</text>
<text text-anchor="start" x="245.5" y="-182" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> post()</text>
<text text-anchor="start" x="245.5" y="-170" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> del()</text>
<text text-anchor="start" x="245.5" y="-158" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> put()</text>
<text text-anchor="start" x="245.5" y="-146" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> patch()</text>
</a>
</g>
</g>
<!-- Handler&#45;&gt;Routing -->
<g id="edge7" class="edge">
<title>Handler-&gt;Routing</title>
<path fill="none" stroke="#000000" d="M219.7512,-303.3602C226.1011,-293.2879 233.0362,-282.2874 239.876,-271.438"/>
<polygon fill="#000000" stroke="#000000" points="216.711,-301.6197 214.3387,-311.9456 222.6325,-305.3529 216.711,-301.6197"/>
</g>
<!-- SslHandler -->
<g id="node9" class="node">
<title>SslHandler</title>
<g id="a_node9"><a xlink:href="SslHandler.md" xlink:title="SslHandler">
<polygon fill="#ffffff" stroke="transparent" points="339,-162 339,-252 434,-252 434,-162 339,-162"/>
<polygon fill="none" stroke="#000000" points="339.5,-230 339.5,-252 434.5,-252 434.5,-230 339.5,-230"/>
<text text-anchor="start" x="362.5545" y="-238" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">SslHandler</text>
<polygon fill="none" stroke="#000000" points="339.5,-208 339.5,-230 434.5,-230 434.5,-208 339.5,-208"/>
<text text-anchor="start" x="344.5" y="-216" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">  new SslHandler()</text>
<polygon fill="none" stroke="#000000" points="339.5,-162 339.5,-208 434.5,-208 434.5,-162 339.5,-162"/>
<text text-anchor="start" x="344.5" y="-194" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> verification</text>
<text text-anchor="start" x="344.5" y="-182" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> ca</text>
<text text-anchor="start" x="344.5" y="-170" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> handler</text>
</a>
</g>
</g>
<!-- Handler&#45;&gt;SslHandler -->
<g id="edge8" class="edge">
<title>Handler-&gt;SslHandler</title>
<path fill="none" stroke="#000000" d="M243.5921,-325.8795C270.9352,-313.9994 304.428,-296.9885 330.5,-276 339.0326,-269.1311 347.1398,-260.7648 354.4011,-252.2601"/>
<polygon fill="#000000" stroke="#000000" points="242.0372,-322.7372 234.1992,-329.8658 244.7719,-329.1809 242.0372,-322.7372"/>
</g>
<!-- HttpHandler -->
<g id="node6" class="node">
<title>HttpHandler</title>
<g id="a_node6"><a xlink:href="HttpHandler.md" xlink:title="HttpHandler">
<polygon fill="#ffffff" stroke="transparent" points="76.5,0 76.5,-102 176.5,-102 176.5,0 76.5,0"/>
<polygon fill="none" stroke="#000000" points="76.5,-80 76.5,-102 176.5,-102 176.5,-80 76.5,-80"/>
<text text-anchor="start" x="99.8305" y="-88" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">HttpHandler</text>
<polygon fill="none" stroke="#000000" points="76.5,-58 76.5,-80 176.5,-80 176.5,-58 76.5,-58"/>
<text text-anchor="start" x="81.5" y="-66" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">  new HttpHandler()</text>
<polygon fill="none" stroke="#000000" points="76.5,0 76.5,-58 176.5,-58 176.5,0 76.5,0"/>
<text text-anchor="start" x="81.5" y="-44" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> crossDomain</text>
<text text-anchor="start" x="81.5" y="-32" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> forceGZIP</text>
<text text-anchor="start" x="81.5" y="-20" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> maxHeadersCount</text>
<text text-anchor="start" x="81.5" y="-8" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> maxUploadSize</text>
</a>
</g>
</g>
<!-- HandlerEx&#45;&gt;HttpHandler -->
<g id="edge5" class="edge">
<title>HandlerEx-&gt;HttpHandler</title>
<path fill="none" stroke="#000000" d="M172.467,-158.0277C164.8314,-140.2492 156.1878,-120.1239 148.4731,-102.1612"/>
<polygon fill="#000000" stroke="#000000" points="169.4308,-159.8274 176.5931,-167.6346 175.8627,-157.065 169.4308,-159.8274"/>
</g>
<!-- WebSocketHandler -->
<g id="node7" class="node">
<title>WebSocketHandler</title>
<g id="a_node7"><a xlink:href="WebSocketHandler.md" xlink:title="WebSocketHandler">
<polygon fill="#ffffff" stroke="transparent" points="194.5,-18 194.5,-84 326.5,-84 326.5,-18 194.5,-18"/>
<polygon fill="none" stroke="#000000" points="194.5,-62 194.5,-84 326.5,-84 326.5,-62 194.5,-62"/>
<text text-anchor="start" x="217.437" y="-70" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">WebSocketHandler</text>
<polygon fill="none" stroke="#000000" points="194.5,-40 194.5,-62 326.5,-62 326.5,-40 194.5,-40"/>
<text text-anchor="start" x="199.5" y="-48" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">  new WebSocketHandler()</text>
<polygon fill="none" stroke="#000000" points="194.5,-18 194.5,-40 326.5,-40 326.5,-18 194.5,-18"/>
<text text-anchor="start" x="199.5" y="-26" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> maxSize</text>
</a>
</g>
</g>
<!-- HandlerEx&#45;&gt;WebSocketHandler -->
<g id="edge6" class="edge">
<title>HandlerEx-&gt;WebSocketHandler</title>
<path fill="none" stroke="#000000" d="M214.427,-158.2745C224.8001,-134.1221 237.0546,-105.5893 246.3166,-84.024"/>
<polygon fill="#000000" stroke="#000000" points="211.1373,-157.065 210.4069,-167.6346 217.5692,-159.8274 211.1373,-157.065"/>
</g>
</g>
</svg></div>

## 构造函数
        
### Handler
** 构造一个消息处理器链处理对象 **

```JavaScript
new Handler(Array hdlrs);
```

调用参数:
* hdlrs: Array, 处理器数组

--------------------------
** 创建一个消息处理器路由对象 **

```JavaScript
new Handler(Object map);
```

调用参数:
* map: Object, 初始化路由参数

--------------------------
** 创建一个 JavaSvript 消息处理器 **

```JavaScript
new Handler(Function hdlr);
```

调用参数:
* hdlr: Function, JavaScript 处理器函数

## 成员函数
        
### invoke
** 处理一个消息或对象 **

```JavaScript
Handler Handler.invoke(object v) async;
```

调用参数:
* v: [object](object.md), 指定处理的消息或对象

返回结果:
* Handler, 返回下一步的处理器

--------------------------
### dispose
** 强制回收对象，调用此方法后，对象资源将立即释放 **

```JavaScript
Handler.dispose();
```

--------------------------
### equals
** 比较当前对象与给定的对象是否相等 **

```JavaScript
Boolean Handler.equals(object expected);
```

调用参数:
* expected: object, 制定比较的目标对象

返回结果:
* Boolean, 返回对象比较的结果

--------------------------
### toString
** 返回对象的字符串表示，一般返回 "[Native Object]"，对象可以根据自己的特性重新实现 **

```JavaScript
String Handler.toString();
```

返回结果:
* String, 返回对象的字符串表示

--------------------------
### toJSON
** 返回对象的 JSON 格式表示，一般返回对象定义的可读属性集合 **

```JavaScript
Value Handler.toJSON(String key = "");
```

调用参数:
* key: String, 未使用

返回结果:
* Value, 返回包含可 JSON 序列化的值

--------------------------
### valueOf
** 返回对象本身的数值 **

```JavaScript
Value Handler.valueOf();
```

返回结果:
* Value, 返回对象本身的数值
