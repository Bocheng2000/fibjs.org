# 对象 EventEmitter
事件触发对象，可用于建立观察者模式，支持事件触发的对象均继承于此，同一事件的同一函数只会产生一次回调

[Event](Event.md) 对象可独立创建，以用于组建自定义的事件系统：

```JavaScript
var EventEmitter = require('events');

var e = new EventEmitter();
```

## 继承关系
<div class="inherits"><svg width="403pt" height="624pt" viewBox="0.00 0.00 402.50 624.00" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
<g id="graph0" class="graph" transform="scale(1 1) rotate(0) translate(4 620)">
<title>%0</title>
<polygon fill="#ffffff" stroke="transparent" points="-4,4 -4,-620 398.5,-620 398.5,4 -4,4"/>
<!-- object -->
<g id="node1" class="node">
<title>object</title>
<g id="a_node1"><a xlink:href="object.md" xlink:title="object">
<polygon fill="#ffffff" stroke="transparent" points="171,-524 171,-616 228,-616 228,-524 171,-524"/>
<polygon fill="none" stroke="#000000" points="171.5,-594 171.5,-616 228.5,-616 228.5,-594 171.5,-594"/>
<text text-anchor="start" x="186.6625" y="-602" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">object</text>
<polygon fill="none" stroke="#000000" points="171.5,-524 171.5,-594 228.5,-594 228.5,-524 171.5,-524"/>
<text text-anchor="start" x="176.5" y="-580" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> dispose()</text>
<text text-anchor="start" x="176.5" y="-568" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> equals()</text>
<text text-anchor="start" x="176.5" y="-556" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> toString()</text>
<text text-anchor="start" x="176.5" y="-544" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> toJSON()</text>
<text text-anchor="start" x="176.5" y="-532" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> valueOf()</text>
</a>
</g>
</g>
<!-- EventEmitter -->
<g id="node2" class="node">
<title>EventEmitter</title>
<g id="a_node2"><a xlink:title="EventEmitter">
<polygon fill="#d3d3d3" stroke="transparent" points="140.5,-244 140.5,-488 258.5,-488 258.5,-244 140.5,-244"/>
<polygon fill="none" stroke="#000000" points="140.5,-466 140.5,-488 258.5,-488 258.5,-466 140.5,-466"/>
<text text-anchor="start" x="170.8855" y="-474" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">EventEmitter</text>
<polygon fill="none" stroke="#000000" points="140.5,-444 140.5,-466 258.5,-466 258.5,-444 140.5,-444"/>
<text text-anchor="start" x="145.5" y="-452" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">  new EventEmitter()</text>
<polygon fill="none" stroke="#000000" points="140.5,-422 140.5,-444 258.5,-444 258.5,-422 140.5,-422"/>
<text text-anchor="start" x="145.5" y="-430" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> defaultMaxListeners</text>
<polygon fill="none" stroke="#000000" points="140.5,-244 140.5,-422 258.5,-422 258.5,-244 140.5,-244"/>
<text text-anchor="start" x="145.5" y="-408" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> on()</text>
<text text-anchor="start" x="145.5" y="-396" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> addListener()</text>
<text text-anchor="start" x="145.5" y="-384" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> prependListener()</text>
<text text-anchor="start" x="145.5" y="-372" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> once()</text>
<text text-anchor="start" x="145.5" y="-360" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> prependOnceListener()</text>
<text text-anchor="start" x="145.5" y="-348" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> off()</text>
<text text-anchor="start" x="145.5" y="-336" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> removeListener()</text>
<text text-anchor="start" x="145.5" y="-324" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> removeAllListeners()</text>
<text text-anchor="start" x="145.5" y="-312" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> setMaxListeners()</text>
<text text-anchor="start" x="145.5" y="-300" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> getMaxListeners()</text>
<text text-anchor="start" x="145.5" y="-288" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> listeners()</text>
<text text-anchor="start" x="145.5" y="-276" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> listenerCount()</text>
<text text-anchor="start" x="145.5" y="-264" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> eventNames()</text>
<text text-anchor="start" x="145.5" y="-252" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> emit()</text>
</a>
</g>
</g>
<!-- object&#45;&gt;EventEmitter -->
<g id="edge1" class="edge">
<title>object-&gt;EventEmitter</title>
<path fill="none" stroke="#000000" d="M199.5,-513.9235C199.5,-505.7711 199.5,-497.1241 199.5,-488.2645"/>
<polygon fill="#000000" stroke="#000000" points="196.0001,-513.964 199.5,-523.9641 203.0001,-513.9641 196.0001,-513.964"/>
</g>
<!-- Service -->
<g id="node3" class="node">
<title>Service</title>
<g id="a_node3"><a xlink:href="Service.md" xlink:title="Service">
<polygon fill="#ffffff" stroke="transparent" points="0,0 0,-208 79,-208 79,0 0,0"/>
<polygon fill="none" stroke="#000000" points=".5,-186 .5,-208 79.5,-208 79.5,-186 .5,-186"/>
<text text-anchor="start" x="23.3325" y="-194" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">Service</text>
<polygon fill="none" stroke="#000000" points=".5,-164 .5,-186 79.5,-186 79.5,-164 .5,-164"/>
<text text-anchor="start" x="5.5" y="-172" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">  new Service()</text>
<polygon fill="none" stroke="#000000" points=".5,-106 .5,-164 79.5,-164 79.5,-106 .5,-106"/>
<text text-anchor="start" x="5.5" y="-150" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> name</text>
<text text-anchor="start" x="5.5" y="-138" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> onstop</text>
<text text-anchor="start" x="5.5" y="-126" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> onpause</text>
<text text-anchor="start" x="5.5" y="-114" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> oncontinue</text>
<polygon fill="none" stroke="#000000" points=".5,0 .5,-106 79.5,-106 79.5,0 .5,0"/>
<text text-anchor="start" x="5.5" y="-92" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> install()</text>
<text text-anchor="start" x="5.5" y="-80" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> remove()</text>
<text text-anchor="start" x="5.5" y="-68" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> start()</text>
<text text-anchor="start" x="5.5" y="-56" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> stop()</text>
<text text-anchor="start" x="5.5" y="-44" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> restart()</text>
<text text-anchor="start" x="5.5" y="-32" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> run()</text>
<text text-anchor="start" x="5.5" y="-20" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> isInstalled()</text>
<text text-anchor="start" x="5.5" y="-8" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> isRunning()</text>
</a>
</g>
</g>
<!-- EventEmitter&#45;&gt;Service -->
<g id="edge2" class="edge">
<title>EventEmitter-&gt;Service</title>
<path fill="none" stroke="#000000" d="M134.493,-280.3763C118.2727,-257.4216 101.5221,-232.235 87.5,-208 84.6617,-203.0945 81.8605,-197.9922 79.1232,-192.7978"/>
<polygon fill="#000000" stroke="#000000" points="131.7874,-282.6107 140.4389,-288.7265 137.4895,-278.5504 131.7874,-282.6107"/>
</g>
<!-- WebSocket -->
<g id="node4" class="node">
<title>WebSocket</title>
<g id="a_node4"><a xlink:href="WebSocket.md" xlink:title="WebSocket">
<polygon fill="#ffffff" stroke="transparent" points="97,-12 97,-196 194,-196 194,-12 97,-12"/>
<polygon fill="none" stroke="#000000" points="97.5,-174 97.5,-196 194.5,-196 194.5,-174 97.5,-174"/>
<text text-anchor="start" x="120.4385" y="-182" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">WebSocket</text>
<polygon fill="none" stroke="#000000" points="97.5,-152 97.5,-174 194.5,-174 194.5,-152 97.5,-152"/>
<text text-anchor="start" x="102.5" y="-160" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">  new WebSocket()</text>
<polygon fill="none" stroke="#000000" points="97.5,-46 97.5,-152 194.5,-152 194.5,-46 97.5,-46"/>
<text text-anchor="start" x="102.5" y="-138" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> url</text>
<text text-anchor="start" x="102.5" y="-126" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> protocol</text>
<text text-anchor="start" x="102.5" y="-114" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> origin</text>
<text text-anchor="start" x="102.5" y="-102" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> readyState</text>
<text text-anchor="start" x="102.5" y="-90" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> onopen</text>
<text text-anchor="start" x="102.5" y="-78" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> onmessage</text>
<text text-anchor="start" x="102.5" y="-66" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> onclose</text>
<text text-anchor="start" x="102.5" y="-54" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> onerror</text>
<polygon fill="none" stroke="#000000" points="97.5,-12 97.5,-46 194.5,-46 194.5,-12 97.5,-12"/>
<text text-anchor="start" x="102.5" y="-32" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> close()</text>
<text text-anchor="start" x="102.5" y="-20" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> send()</text>
</a>
</g>
</g>
<!-- EventEmitter&#45;&gt;WebSocket -->
<g id="edge3" class="edge">
<title>EventEmitter-&gt;WebSocket</title>
<path fill="none" stroke="#000000" d="M172.2271,-233.6761C169.6185,-221.0192 167.0132,-208.3787 164.5087,-196.2275"/>
<polygon fill="#000000" stroke="#000000" points="168.8714,-234.7336 174.3181,-243.8212 175.7273,-233.3205 168.8714,-234.7336"/>
</g>
<!-- WebView -->
<g id="node5" class="node">
<title>WebView</title>
<g id="a_node5"><a xlink:href="WebView.md" xlink:title="WebView">
<polygon fill="#ffffff" stroke="transparent" points="212.5,-17 212.5,-191 294.5,-191 294.5,-17 212.5,-17"/>
<polygon fill="none" stroke="#000000" points="212.5,-169 212.5,-191 294.5,-191 294.5,-169 212.5,-169"/>
<text text-anchor="start" x="232.3885" y="-177" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">WebView</text>
<polygon fill="none" stroke="#000000" points="212.5,-87 212.5,-169 294.5,-169 294.5,-87 212.5,-87"/>
<text text-anchor="start" x="217.5" y="-155" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> visible</text>
<text text-anchor="start" x="217.5" y="-143" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> onload</text>
<text text-anchor="start" x="217.5" y="-131" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> onmove</text>
<text text-anchor="start" x="217.5" y="-119" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> onresize</text>
<text text-anchor="start" x="217.5" y="-107" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> onclose</text>
<text text-anchor="start" x="217.5" y="-95" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> onmessage</text>
<polygon fill="none" stroke="#000000" points="212.5,-17 212.5,-87 294.5,-87 294.5,-17 212.5,-17"/>
<text text-anchor="start" x="217.5" y="-73" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> setHtml()</text>
<text text-anchor="start" x="217.5" y="-61" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> print()</text>
<text text-anchor="start" x="217.5" y="-49" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> close()</text>
<text text-anchor="start" x="217.5" y="-37" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> wait()</text>
<text text-anchor="start" x="217.5" y="-25" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> postMessage()</text>
</a>
</g>
</g>
<!-- EventEmitter&#45;&gt;WebView -->
<g id="edge4" class="edge">
<title>EventEmitter-&gt;WebView</title>
<path fill="none" stroke="#000000" d="M226.7419,-233.8265C229.7191,-219.3816 232.6923,-204.9557 235.5169,-191.2515"/>
<polygon fill="#000000" stroke="#000000" points="223.2727,-233.3205 224.6819,-243.8212 230.1286,-234.7336 223.2727,-233.3205"/>
</g>
<!-- Worker -->
<g id="node6" class="node">
<title>Worker</title>
<g id="a_node6"><a xlink:href="Worker.md" xlink:title="Worker">
<polygon fill="#ffffff" stroke="transparent" points="312.5,-60 312.5,-148 394.5,-148 394.5,-60 312.5,-60"/>
<polygon fill="none" stroke="#000000" points="312.5,-126 312.5,-148 394.5,-148 394.5,-126 312.5,-126"/>
<text text-anchor="start" x="337.3925" y="-134" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">Worker</text>
<polygon fill="none" stroke="#000000" points="312.5,-104 312.5,-126 394.5,-126 394.5,-104 312.5,-104"/>
<text text-anchor="start" x="317.5" y="-112" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">  new Worker()</text>
<polygon fill="none" stroke="#000000" points="312.5,-82 312.5,-104 394.5,-104 394.5,-82 312.5,-82"/>
<text text-anchor="start" x="317.5" y="-90" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> onmessage</text>
<polygon fill="none" stroke="#000000" points="312.5,-60 312.5,-82 394.5,-82 394.5,-60 312.5,-60"/>
<text text-anchor="start" x="317.5" y="-68" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> postMessage()</text>
</a>
</g>
</g>
<!-- EventEmitter&#45;&gt;Worker -->
<g id="edge5" class="edge">
<title>EventEmitter-&gt;Worker</title>
<path fill="none" stroke="#000000" d="M264.1543,-272.2648C277.6877,-251.4312 291.4845,-229.224 303.5,-208 314.3568,-188.8227 325.1151,-166.9242 333.8551,-148.1838"/>
<polygon fill="#000000" stroke="#000000" points="261.1225,-270.5062 258.5809,-280.7917 266.9819,-274.3361 261.1225,-270.5062"/>
</g>
</g>
</svg></div>

## 构造函数
        
### EventEmitter
** 构造函数 **

```JavaScript
new EventEmitter();
```

## 静态属性
        
### defaultMaxListeners
** Integer, 默认全局最大监听器数 **

```JavaScript
static Integer EventEmitter.defaultMaxListeners;
```

## 成员函数
        
### on
** 绑定一个事件处理函数到对象 **

```JavaScript
Object EventEmitter.on(String ev,
    Function func);
```

调用参数:
* ev: String, 指定事件的名称
* func: Function, 指定事件处理函数

返回结果:
* Object, 返回成功绑定的数量，如果函数已绑定则返回 0

--------------------------
** 绑定一个事件处理函数到对象 **

```JavaScript
Object EventEmitter.on(Object map);
```

调用参数:
* map: Object, 指定事件映射关系，对象属性名称将作为事件名称，属性的值将作为事件处理函数

返回结果:
* Object, 返回事件对象本身，便于链式调用

--------------------------
### addListener
** 绑定一个事件处理函数到对象 **

```JavaScript
Object EventEmitter.addListener(String ev,
    Function func);
```

调用参数:
* ev: String, 指定事件的名称
* func: Function, 指定事件处理函数

返回结果:
* Object, 返回事件对象本身，便于链式调用

--------------------------
** 绑定一个事件处理函数到对象 **

```JavaScript
Object EventEmitter.addListener(Object map);
```

调用参数:
* map: Object, 指定事件映射关系，对象属性名称将作为事件名称，属性的值将作为事件处理函数

返回结果:
* Object, 返回事件对象本身，便于链式调用

--------------------------
### prependListener
** 绑定一个事件处理函数到对象起始 **

```JavaScript
Object EventEmitter.prependListener(String ev,
    Function func);
```

调用参数:
* ev: String, 指定事件的名称
* func: Function, 指定事件处理函数

返回结果:
* Object, 返回成功绑定的数量，如果函数已绑定则返回 0

--------------------------
** 绑定一个事件处理函数到对象起始 **

```JavaScript
Object EventEmitter.prependListener(Object map);
```

调用参数:
* map: Object, 指定事件映射关系，对象属性名称将作为事件名称，属性的值将作为事件处理函数

返回结果:
* Object, 返回成功绑定的数量，如果函数已绑定则返回 0

--------------------------
### once
** 绑定一个一次性事件处理函数到对象，一次性处理函数只会触发一次 **

```JavaScript
Object EventEmitter.once(String ev,
    Function func);
```

调用参数:
* ev: String, 指定事件的名称
* func: Function, 指定事件处理函数

返回结果:
* Object, 返回事件对象本身，便于链式调用

--------------------------
** 绑定一个一次性事件处理函数到对象，一次性处理函数只会触发一次 **

```JavaScript
Object EventEmitter.once(Object map);
```

调用参数:
* map: Object, 指定事件映射关系，对象属性名称将作为事件名称，属性的值将作为事件处理函数

返回结果:
* Object, 返回事件对象本身，便于链式调用

--------------------------
### prependOnceListener
** 绑定一个事件处理函数到对象起始 **

```JavaScript
Object EventEmitter.prependOnceListener(String ev,
    Function func);
```

调用参数:
* ev: String, 指定事件的名称
* func: Function, 指定事件处理函数

返回结果:
* Object, 返回成功绑定的数量，如果函数已绑定则返回 0

--------------------------
** 绑定一个事件处理函数到对象起始 **

```JavaScript
Object EventEmitter.prependOnceListener(Object map);
```

调用参数:
* map: Object, 指定事件映射关系，对象属性名称将作为事件名称，属性的值将作为事件处理函数

返回结果:
* Object, 返回成功绑定的数量，如果函数已绑定则返回 0

--------------------------
### off
** 从对象处理队列中取消指定函数 **

```JavaScript
Object EventEmitter.off(String ev,
    Function func);
```

调用参数:
* ev: String, 指定事件的名称
* func: Function, 指定事件处理函数

返回结果:
* Object, 返回事件对象本身，便于链式调用

--------------------------
** 取消对象处理队列中的全部函数 **

```JavaScript
Object EventEmitter.off(String ev);
```

调用参数:
* ev: String, 指定事件的名称

返回结果:
* Object, 返回事件对象本身，便于链式调用

--------------------------
** 从对象处理队列中取消指定函数 **

```JavaScript
Object EventEmitter.off(Object map);
```

调用参数:
* map: Object, 指定事件映射关系，对象属性名称作为事件名称，属性的值作为事件处理函数

返回结果:
* Object, 返回事件对象本身，便于链式调用

--------------------------
### removeListener
** 从对象处理队列中取消指定函数 **

```JavaScript
Object EventEmitter.removeListener(String ev,
    Function func);
```

调用参数:
* ev: String, 指定事件的名称
* func: Function, 指定事件处理函数

返回结果:
* Object, 返回事件对象本身，便于链式调用

--------------------------
** 取消对象处理队列中的全部函数 **

```JavaScript
Object EventEmitter.removeListener(String ev);
```

调用参数:
* ev: String, 指定事件的名称

返回结果:
* Object, 返回事件对象本身，便于链式调用

--------------------------
** 从对象处理队列中取消指定函数 **

```JavaScript
Object EventEmitter.removeListener(Object map);
```

调用参数:
* map: Object, 指定事件映射关系，对象属性名称作为事件名称，属性的值作为事件处理函数

返回结果:
* Object, 返回事件对象本身，便于链式调用

--------------------------
### removeAllListeners
** 从对象处理队列中取消所有事件的所有监听器， 如果指定事件，则移除指定事件的所有监听器。 **

```JavaScript
Object EventEmitter.removeAllListeners(Array evs = []);
```

调用参数:
* evs: Array, 指定事件的名称

返回结果:
* Object, 返回事件对象本身，便于链式调用

--------------------------
### setMaxListeners
** 监听器的默认限制的数量，仅用于兼容 **

```JavaScript
EventEmitter.setMaxListeners(Integer n);
```

调用参数:
* n: Integer, 指定事件的数量

--------------------------
### getMaxListeners
** 获取监听器的默认限制的数量，仅用于兼容 **

```JavaScript
Integer EventEmitter.getMaxListeners();
```

返回结果:
* Integer, 返回默认限制数量

--------------------------
### listeners
** 查询对象指定事件的监听器数组 **

```JavaScript
Array EventEmitter.listeners(String ev);
```

调用参数:
* ev: String, 指定事件的名称

返回结果:
* Array, 返回指定事件的监听器数组

--------------------------
### listenerCount
** 查询对象指定事件的监听器数量 **

```JavaScript
Integer EventEmitter.listenerCount(String ev);
```

调用参数:
* ev: String, 指定事件的名称

返回结果:
* Integer, 返回指定事件的监听器数量

--------------------------
### eventNames
** 查询监听器事件名称 **

```JavaScript
Array EventEmitter.eventNames();
```

返回结果:
* Array, 返回事件名称数组

--------------------------
### emit
** 主动触发一个事件 **

```JavaScript
Boolean EventEmitter.emit(String ev,
    ...);
```

调用参数:
* ev: String, 事件名称
* ...: 事件参数，将会传递给事件处理函数

返回结果:
* Boolean, 返回事件触发状态，有响应事件返回 true，否则返回 false

--------------------------
### dispose
** 强制回收对象，调用此方法后，对象资源将立即释放 **

```JavaScript
EventEmitter.dispose();
```

--------------------------
### equals
** 比较当前对象与给定的对象是否相等 **

```JavaScript
Boolean EventEmitter.equals(object expected);
```

调用参数:
* expected: object, 制定比较的目标对象

返回结果:
* Boolean, 返回对象比较的结果

--------------------------
### toString
** 返回对象的字符串表示，一般返回 "[Native Object]"，对象可以根据自己的特性重新实现 **

```JavaScript
String EventEmitter.toString();
```

返回结果:
* String, 返回对象的字符串表示

--------------------------
### toJSON
** 返回对象的 JSON 格式表示，一般返回对象定义的可读属性集合 **

```JavaScript
Value EventEmitter.toJSON(String key = "");
```

调用参数:
* key: String, 未使用

返回结果:
* Value, 返回包含可 JSON 序列化的值

--------------------------
### valueOf
** 返回对象本身的数值 **

```JavaScript
Value EventEmitter.valueOf();
```

返回结果:
* Value, 返回对象本身的数值
