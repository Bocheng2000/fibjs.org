# 对象 Stream
流操作对象，用于二进制数据流读写

Stream 为基础对象，用于为流处理定义标准借口，不能独立创建

## 继承关系
<div class="inherits"><svg width="436pt" height="646pt" viewBox="0.00 0.00 435.50 646.00" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
<g id="graph0" class="graph" transform="scale(1 1) rotate(0) translate(4 642)">
<title>%0</title>
<polygon fill="#ffffff" stroke="transparent" points="-4,4 -4,-642 431.5,-642 431.5,4 -4,4"/>
<!-- object -->
<g id="node1" class="node">
<title>object</title>
<g id="a_node1"><a xlink:href="object.md" xlink:title="object">
<polygon fill="#ffffff" stroke="transparent" points="197.5,-546 197.5,-638 254.5,-638 254.5,-546 197.5,-546"/>
<polygon fill="none" stroke="#000000" points="198,-616 198,-638 255,-638 255,-616 198,-616"/>
<text text-anchor="start" x="213.1625" y="-624" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">object</text>
<polygon fill="none" stroke="#000000" points="198,-546 198,-616 255,-616 255,-546 198,-546"/>
<text text-anchor="start" x="203" y="-602" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> dispose()</text>
<text text-anchor="start" x="203" y="-590" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> equals()</text>
<text text-anchor="start" x="203" y="-578" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> toString()</text>
<text text-anchor="start" x="203" y="-566" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> toJSON()</text>
<text text-anchor="start" x="203" y="-554" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> valueOf()</text>
</a>
</g>
</g>
<!-- Stream -->
<g id="node2" class="node">
<title>Stream</title>
<g id="a_node2"><a xlink:title="Stream">
<polygon fill="#d3d3d3" stroke="transparent" points="198.5,-430 198.5,-510 253.5,-510 253.5,-430 198.5,-430"/>
<polygon fill="none" stroke="#000000" points="199,-488 199,-510 254,-510 254,-488 199,-488"/>
<text text-anchor="start" x="210.388" y="-496" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">Stream</text>
<polygon fill="none" stroke="#000000" points="199,-430 199,-488 254,-488 254,-430 199,-430"/>
<text text-anchor="start" x="204" y="-474" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> read()</text>
<text text-anchor="start" x="204" y="-462" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> write()</text>
<text text-anchor="start" x="204" y="-450" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> close()</text>
<text text-anchor="start" x="204" y="-438" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> copyTo()</text>
</a>
</g>
</g>
<!-- object&#45;&gt;Stream -->
<g id="edge1" class="edge">
<title>object-&gt;Stream</title>
<path fill="none" stroke="#000000" d="M226,-535.8267C226,-527.1786 226,-518.4003 226,-510.193"/>
<polygon fill="#000000" stroke="#000000" points="222.5001,-535.877 226,-545.877 229.5001,-535.8771 222.5001,-535.877"/>
</g>
<!-- BufferedStream -->
<g id="node3" class="node">
<title>BufferedStream</title>
<g id="a_node3"><a xlink:href="BufferedStream.md" xlink:title="BufferedStream">
<polygon fill="#ffffff" stroke="transparent" points="0,-186 0,-358 116,-358 116,-186 0,-186"/>
<polygon fill="none" stroke="#000000" points="0,-336 0,-358 116,-358 116,-336 0,-336"/>
<text text-anchor="start" x="22.992" y="-344" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">BufferedStream</text>
<polygon fill="none" stroke="#000000" points="0,-314 0,-336 116,-336 116,-314 0,-314"/>
<text text-anchor="start" x="5" y="-322" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">  new BufferedStream()</text>
<polygon fill="none" stroke="#000000" points="0,-268 0,-314 116,-314 116,-268 0,-268"/>
<text text-anchor="start" x="5" y="-300" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> stream</text>
<text text-anchor="start" x="5" y="-288" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> charset</text>
<text text-anchor="start" x="5" y="-276" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> EOL</text>
<polygon fill="none" stroke="#000000" points="0,-186 0,-268 116,-268 116,-186 0,-186"/>
<text text-anchor="start" x="5" y="-254" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> readText()</text>
<text text-anchor="start" x="5" y="-242" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> readLine()</text>
<text text-anchor="start" x="5" y="-230" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> readLines()</text>
<text text-anchor="start" x="5" y="-218" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> readUntil()</text>
<text text-anchor="start" x="5" y="-206" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> writeText()</text>
<text text-anchor="start" x="5" y="-194" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> writeLine()</text>
</a>
</g>
</g>
<!-- Stream&#45;&gt;BufferedStream -->
<g id="edge2" class="edge">
<title>Stream-&gt;BufferedStream</title>
<path fill="none" stroke="#000000" d="M189.5974,-448.1218C168.8903,-434.4143 143.4834,-415.3325 125,-394 115.5849,-383.1336 106.927,-370.728 99.183,-358.0856"/>
<polygon fill="#000000" stroke="#000000" points="187.8536,-451.1623 198.1502,-453.6583 191.6575,-445.286 187.8536,-451.1623"/>
</g>
<!-- SeekableStream -->
<g id="node5" class="node">
<title>SeekableStream</title>
<g id="a_node5"><a xlink:href="SeekableStream.md" xlink:title="SeekableStream">
<polygon fill="#ffffff" stroke="transparent" points="134.5,-202 134.5,-342 217.5,-342 217.5,-202 134.5,-202"/>
<polygon fill="none" stroke="#000000" points="135,-320 135,-342 218,-342 218,-320 135,-320"/>
<text text-anchor="start" x="139.5465" y="-328" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">SeekableStream</text>
<polygon fill="none" stroke="#000000" points="135,-202 135,-320 218,-320 218,-202 135,-202"/>
<text text-anchor="start" x="140" y="-306" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> seek()</text>
<text text-anchor="start" x="140" y="-294" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> tell()</text>
<text text-anchor="start" x="140" y="-282" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> rewind()</text>
<text text-anchor="start" x="140" y="-270" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> size()</text>
<text text-anchor="start" x="140" y="-258" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> readAll()</text>
<text text-anchor="start" x="140" y="-246" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> truncate()</text>
<text text-anchor="start" x="140" y="-234" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> eof()</text>
<text text-anchor="start" x="140" y="-222" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> flush()</text>
<text text-anchor="start" x="140" y="-210" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> stat()</text>
</a>
</g>
</g>
<!-- Stream&#45;&gt;SeekableStream -->
<g id="edge4" class="edge">
<title>Stream-&gt;SeekableStream</title>
<path fill="none" stroke="#000000" d="M213.4065,-420.1296C207.4367,-396.4892 200.2025,-367.842 193.693,-342.0643"/>
<polygon fill="#000000" stroke="#000000" points="210.0398,-421.0931 215.8818,-429.9317 216.8268,-419.3791 210.0398,-421.0931"/>
</g>
<!-- Socket -->
<g id="node8" class="node">
<title>Socket</title>
<g id="a_node8"><a xlink:href="Socket.md" xlink:title="Socket">
<polygon fill="#ffffff" stroke="transparent" points="235.5,-150 235.5,-394 318.5,-394 318.5,-150 235.5,-150"/>
<polygon fill="none" stroke="#000000" points="236,-372 236,-394 319,-394 319,-372 236,-372"/>
<text text-anchor="start" x="262.217" y="-380" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">Socket</text>
<polygon fill="none" stroke="#000000" points="236,-350 236,-372 319,-372 319,-350 236,-350"/>
<text text-anchor="start" x="241" y="-358" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">  new Socket()</text>
<polygon fill="none" stroke="#000000" points="236,-256 236,-350 319,-350 319,-256 236,-256"/>
<text text-anchor="start" x="241" y="-336" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> family</text>
<text text-anchor="start" x="241" y="-324" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> type</text>
<text text-anchor="start" x="241" y="-312" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> remoteAddress</text>
<text text-anchor="start" x="241" y="-300" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> remotePort</text>
<text text-anchor="start" x="241" y="-288" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> localAddress</text>
<text text-anchor="start" x="241" y="-276" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> localPort</text>
<text text-anchor="start" x="241" y="-264" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> timeout</text>
<polygon fill="none" stroke="#000000" points="236,-150 236,-256 319,-256 319,-150 236,-150"/>
<text text-anchor="start" x="241" y="-242" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> connect()</text>
<text text-anchor="start" x="241" y="-230" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> bind()</text>
<text text-anchor="start" x="241" y="-218" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> listen()</text>
<text text-anchor="start" x="241" y="-206" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> accept()</text>
<text text-anchor="start" x="241" y="-194" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> recv()</text>
<text text-anchor="start" x="241" y="-182" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> recvfrom()</text>
<text text-anchor="start" x="241" y="-170" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> send()</text>
<text text-anchor="start" x="241" y="-158" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> sendto()</text>
</a>
</g>
</g>
<!-- Stream&#45;&gt;Socket -->
<g id="edge7" class="edge">
<title>Stream-&gt;Socket</title>
<path fill="none" stroke="#000000" d="M238.8761,-420.0103C240.9621,-411.9118 243.1988,-403.228 245.5049,-394.2751"/>
<polygon fill="#000000" stroke="#000000" points="235.4257,-419.3748 236.3206,-429.9317 242.2044,-421.1209 235.4257,-419.3748"/>
</g>
<!-- SslSocket -->
<g id="node9" class="node">
<title>SslSocket</title>
<g id="a_node9"><a xlink:href="SslSocket.md" xlink:title="SslSocket">
<polygon fill="#ffffff" stroke="transparent" points="336.5,-204 336.5,-340 427.5,-340 427.5,-204 336.5,-204"/>
<polygon fill="none" stroke="#000000" points="337,-318 337,-340 428,-340 428,-318 337,-318"/>
<text text-anchor="start" x="360.273" y="-326" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">SslSocket</text>
<polygon fill="none" stroke="#000000" points="337,-296 337,-318 428,-318 428,-296 337,-296"/>
<text text-anchor="start" x="342" y="-304" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">  new SslSocket()</text>
<polygon fill="none" stroke="#000000" points="337,-238 337,-296 428,-296 428,-238 337,-238"/>
<text text-anchor="start" x="342" y="-282" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> verification</text>
<text text-anchor="start" x="342" y="-270" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> ca</text>
<text text-anchor="start" x="342" y="-258" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> peerCert</text>
<text text-anchor="start" x="342" y="-246" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> stream</text>
<polygon fill="none" stroke="#000000" points="337,-204 337,-238 428,-238 428,-204 337,-204"/>
<text text-anchor="start" x="342" y="-224" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> connect()</text>
<text text-anchor="start" x="342" y="-212" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> accept()</text>
</a>
</g>
</g>
<!-- Stream&#45;&gt;SslSocket -->
<g id="edge8" class="edge">
<title>Stream-&gt;SslSocket</title>
<path fill="none" stroke="#000000" d="M262.3212,-449.4951C283.6853,-435.9695 309.9604,-416.6037 328,-394 340.7146,-378.0686 351.0688,-358.674 359.1829,-340.0797"/>
<polygon fill="#000000" stroke="#000000" points="260.4798,-446.5186 253.8048,-454.7463 264.1537,-452.477 260.4798,-446.5186"/>
</g>
<!-- SubProcess -->
<g id="node4" class="node">
<title>SubProcess</title>
<g id="a_node4"><a xlink:href="SubProcess.md" xlink:title="SubProcess">
<polygon fill="#ffffff" stroke="transparent" points="21,0 21,-114 95,-114 95,0 21,0"/>
<polygon fill="none" stroke="#000000" points="21,-92 21,-114 95,-114 95,-92 21,-92"/>
<text text-anchor="start" x="31.0485" y="-100" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">SubProcess</text>
<polygon fill="none" stroke="#000000" points="21,-46 21,-92 95,-92 95,-46 21,-46"/>
<text text-anchor="start" x="26" y="-78" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> pid</text>
<text text-anchor="start" x="26" y="-66" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> stdin</text>
<text text-anchor="start" x="26" y="-54" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> stdout</text>
<polygon fill="none" stroke="#000000" points="21,0 21,-46 95,-46 95,0 21,0"/>
<text text-anchor="start" x="26" y="-32" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> kill()</text>
<text text-anchor="start" x="26" y="-20" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> wait()</text>
<text text-anchor="start" x="26" y="-8" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> findWindow()</text>
</a>
</g>
</g>
<!-- BufferedStream&#45;&gt;SubProcess -->
<g id="edge3" class="edge">
<title>BufferedStream-&gt;SubProcess</title>
<path fill="none" stroke="#000000" d="M58,-175.5634C58,-154.6097 58,-133.0893 58,-114.2322"/>
<polygon fill="#000000" stroke="#000000" points="54.5001,-175.7901 58,-185.7901 61.5001,-175.7901 54.5001,-175.7901"/>
</g>
<!-- File -->
<g id="node6" class="node">
<title>File</title>
<g id="a_node6"><a xlink:href="File.md" xlink:title="File">
<polygon fill="#ffffff" stroke="transparent" points="132,-18 132,-96 184,-96 184,-18 132,-18"/>
<polygon fill="none" stroke="#000000" points="132,-74 132,-96 184,-96 184,-74 132,-74"/>
<text text-anchor="start" x="149.947" y="-82" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">File</text>
<polygon fill="none" stroke="#000000" points="132,-40 132,-74 184,-74 184,-40 132,-40"/>
<text text-anchor="start" x="137" y="-60" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> name</text>
<text text-anchor="start" x="137" y="-48" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> fd</text>
<polygon fill="none" stroke="#000000" points="132,-18 132,-40 184,-40 184,-18 132,-18"/>
<text text-anchor="start" x="137" y="-26" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> chmod()</text>
</a>
</g>
</g>
<!-- SeekableStream&#45;&gt;File -->
<g id="edge5" class="edge">
<title>SeekableStream-&gt;File</title>
<path fill="none" stroke="#000000" d="M169.2937,-191.8964C166.5602,-159.2468 163.5243,-122.9846 161.2891,-96.2868"/>
<polygon fill="#000000" stroke="#000000" points="165.8089,-192.2254 170.131,-201.8985 172.7844,-191.6413 165.8089,-192.2254"/>
</g>
<!-- MemoryStream -->
<g id="node7" class="node">
<title>MemoryStream</title>
<g id="a_node7"><a xlink:href="MemoryStream.md" xlink:title="MemoryStream">
<polygon fill="#ffffff" stroke="transparent" points="203,-12 203,-102 317,-102 317,-12 203,-12"/>
<polygon fill="none" stroke="#000000" points="203,-80 203,-102 317,-102 317,-80 203,-80"/>
<text text-anchor="start" x="225.8355" y="-88" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">MemoryStream</text>
<polygon fill="none" stroke="#000000" points="203,-58 203,-80 317,-80 317,-58 203,-58"/>
<text text-anchor="start" x="208" y="-66" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000">  new MemoryStream()</text>
<polygon fill="none" stroke="#000000" points="203,-12 203,-58 317,-58 317,-12 203,-12"/>
<text text-anchor="start" x="208" y="-44" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> setTime()</text>
<text text-anchor="start" x="208" y="-32" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> clone()</text>
<text text-anchor="start" x="208" y="-20" font-family="Helvetica,sans-Serif" font-size="10.00" fill="#000000"> clear()</text>
</a>
</g>
</g>
<!-- SeekableStream&#45;&gt;MemoryStream -->
<g id="edge6" class="edge">
<title>SeekableStream-&gt;MemoryStream</title>
<path fill="none" stroke="#000000" d="M207.0335,-192.569C218.9239,-162.1353 232.0752,-128.4743 242.2986,-102.3071"/>
<polygon fill="#000000" stroke="#000000" points="203.7676,-191.3104 203.3885,-201.8985 210.2877,-193.8578 203.7676,-191.3104"/>
</g>
</g>
</svg></div>

## 成员函数
        
### read
** 从流内读取指定大小的数据 **

```JavaScript
Buffer Stream.read(Integer bytes = -1) async;
```

调用参数:
* bytes: Integer, 指定要读取的数据量，缺省为读取随机大小的数据块，读出的数据尺寸取决于设备

返回结果:
* [Buffer](Buffer.md), 返回从流内读取的数据，若无数据可读，或者连接中断，则返回 null

--------------------------
### write
** 将给定的数据写入流 **

```JavaScript
Stream.write(Buffer data) async;
```

调用参数:
* data: [Buffer](Buffer.md), 给定要写入的数据

--------------------------
### close
** 关闭当前流对象 **

```JavaScript
Stream.close() async;
```

--------------------------
### copyTo
** 复制流数据到目标流中 **

```JavaScript
Long Stream.copyTo(Stream stm,
    Long bytes = -1) async;
```

调用参数:
* stm: Stream, 目标流对象
* bytes: Long, 复制的字节数

返回结果:
* Long, 返回复制的字节数

--------------------------
### dispose
** 强制回收对象，调用此方法后，对象资源将立即释放 **

```JavaScript
Stream.dispose();
```

--------------------------
### equals
** 比较当前对象与给定的对象是否相等 **

```JavaScript
Boolean Stream.equals(object expected);
```

调用参数:
* expected: object, 制定比较的目标对象

返回结果:
* Boolean, 返回对象比较的结果

--------------------------
### toString
** 返回对象的字符串表示，一般返回 "[Native Object]"，对象可以根据自己的特性重新实现 **

```JavaScript
String Stream.toString();
```

返回结果:
* String, 返回对象的字符串表示

--------------------------
### toJSON
** 返回对象的 JSON 格式表示，一般返回对象定义的可读属性集合 **

```JavaScript
Value Stream.toJSON(String key = "");
```

调用参数:
* key: String, 未使用

返回结果:
* Value, 返回包含可 JSON 序列化的值

--------------------------
### valueOf
** 返回对象本身的数值 **

```JavaScript
Value Stream.valueOf();
```

返回结果:
* Value, 返回对象本身的数值
