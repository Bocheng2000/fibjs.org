# 模块 base32
base32 编码与解码模块

`base32`模块是一个用于 base32 编码和解码的模块。Base32 是一种用于将二进制数据编码为 ASCII 字符串的算法，用于将二进制数据在邮件、DNS 等网络协议中传输。

该模块提供了两个方法：`encode` 和 `decode`。其中 `encode` 方法用于将二进制数据编码为 Base32 字符串，`decode` 方法用于将 Base32 字符串解码为二进制数据。下面是使用示例：

```JavaScript
const base32 = require('base32');
const data = new Uint8Array([0x4e, 0x4f, 0x44, 0x45]); // 'NODE'
const encoded = base32.encode(data); // 'KRUGKIDROV======'
const decoded = base32.decode(encoded); // [0x4e, 0x4f, 0x44, 0x45]
console.log(encoded, decoded); // KRUGKIDROV====== [78, 79, 68, 69]
```

可以看到，`encode` 方法将二进制数据编码为了 `KRUGKIDROV======`，而 `decode` 方法将其解码为了 `[0x4e, 0x4f, 0x44, 0x45]`。

需要注意的是，Base32 编码的结果字符串长度是原二进制数据长度的约 8/5 倍，因此不适合用于对大量数据的编码。如果需要对大量数据进行编码，建议使用 Base64 编码。

## 静态函数
        
### encode
**以 base32 方式编码数据**

```JavaScript
static String base32.encode(Buffer data);
```

调用参数:
* data: [Buffer](../../object/ifs/Buffer.md), 要编码的数据

返回结果:
* String, 返回编码的字符串

--------------------------
### decode
**以 base32 方式解码字符串为二进制数据**

```JavaScript
static Buffer base32.decode(String data);
```

调用参数:
* data: String, 要解码的字符串

返回结果:
* [Buffer](../../object/ifs/Buffer.md), 返回解码的二进制数据

