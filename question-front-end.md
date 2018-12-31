# question-front-end
some questions and codes for front-end.

#### 1. XMLHttpRequest有哪些通用属性和方法？
readystate：表示请求状态的整数<br>
&emsp;UNSET(0)：对象已创建；<br>
&emsp;OPENED(1)：open()成功调用，在这个状态下可以为xhr设置请求头，或者使用send()发送请求；<br>
&emsp;HEADERS_RECEIVED(2)：所有重定向已自动完成访问，并且最终响应的HTTP头已经收到；<br>
&emsp;LOADING(3)：响应体正在接收；<br>
&emsp;DONE(4)：数据传输完成或者传输发生错误。<br>
onreadystatechange：readystate改变时调用的函数<br>
Status：服务器返回的HTTP状态码，如200、404<br>
statusText：服务器返回的HTTP状态信息，如OK、No Content<br>
responseText：来自服务器的字符串形式的完整响应<br>
responseXML：Document对象，表示服务器的响应解析成的XML文档<br>
abort()：取消异步HTTP请求<br>
getAllResponseHesders()：返回一个字符串，包含响应中服务器发送的所有HTTP报头，每个报头都是用冒号分割的键值对，用换行符分割报头行<br>
open(method, url, asynchronous [, user, passwod])：初始化准备发送到服务器上的请求，asynchronous表示请求是否异步<br>
setRequestHeader(name, value)：设置HTTP报头<br>
send(body)：对服务器请求进行初始化。参数body包含请求的主体部分，对于POST请求为键值对字符串，对于GET请求为null<br>

#### 2. sessionStorage、localStorage和cookie的区别？
(1) 都会在浏览器保存，有大小限制，同源限制<br>
(2) cookie在请求时发送到服务器，作为会话的标志，服务器可修改cookie；storage不会发送到服务器<br>
(3) cookie有path概念，子路径可以访问父路径cookie，父路径不能访问子路径cookie<br>
(4) 有效期：cookie在设置的有效期内有效，默认为浏览器关闭，可以通过max-age设置有效期；sessionStorage在窗口关闭前有效，localStorage长期有效，直到用户删除<br>
(5) 共享：sessionStorage不能共享，localStorage在同源文档间共享，cookie在同源且符合path规则的文档间共享<br>
(6) localStorage的修改会触发其他窗口的update事件<br>
(7) cookie有secure属性要求HTTPS传输<br>
(8) 浏览器不能保存超过300个cookie，单个服务器不能超过20个，每个cookie不能超过4K；storage大小能达到5M

#### 3. JavaScript的数据类型？
六种基本数据类型：undefined、null、boolean、number、string、symbol(ES6)<br>
一种引用类型：Object

#### 4. 什么是闭包？有什么用？
闭包是在某个作用域内定义的函数，它可以访问这个作用域内的所有变量。<br>
闭包作用域链通常包括三个部分：<br>
(1) 函数本身作用域<br>
(2) 闭包定义时的作用域<br>
(3) 全局作用域<br>

闭包常见用途：<br>
(1) 创建特权方法用于访问控制<br>
(2) 事件处理程序及回调

#### 5. JavaScript定义函数的方法？
(1) 函数声明表达式<br>
(2) function操作符<br>
(3) Function构造函数<br>
(4) ES6：arrow function
































#### 100
