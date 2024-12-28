---
title: "Hàm trong JavaScript"
date: 2024-12-18
weight: 9
draft: false
---
<p style="text-indent: 50px;">Hàm (function) trong JavaScript là một khối mã có thể được gọi và thực thi khi cần thiết. Hàm giúp tổ chức mã nguồn tốt hơn, giảm thiểu sự trùng lặp và dễ dàng tái sử dụng. JavaScript cung cấp nhiều cách để khai báo và sử dụng hàm.
<p style="font-size: 2em; font-weight: bold; color: black;">1. Khai Báo Hàm trong JavaScript
<p style="text-indent: 50px;">Có hai cách phổ biến để khai báo hàm trong JavaScript: khai báo hàm thông thường và khai báo hàm dưới dạng biểu thức hàm.

**a. Hàm Cơ Bản (Function Declaration)**
<p style="text-indent: 50px;">Cách đơn giản nhất để khai báo một hàm trong JavaScript là sử dụng cú pháp function. Hàm được khai báo với từ khóa function, sau đó là tên hàm, danh sách tham số trong dấu ngoặc đơn và phần thân hàm trong dấu ngoặc nhọn.

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">function <span style="color: red;">greet</span>(<span style="color: yellow;">name</span>) {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: violet;">console.log(<span style="color: white;">"Hello, " + name + "!"</span>);</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">}</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">greet(<span style="color: yellow;">"John"</span>); <span style="color: green;">//In ra: Hello, John!</span></p>
</div>

Trong ví dụ trên, hàm greet nhận một tham số name và in ra một thông điệp chào mừng.

**b. Biểu Thức Hàm (Function Expression)**
<p style="text-indent: 50px;">Hàm có thể được khai báo dưới dạng biểu thức hàm và có thể được gán cho một biến. Điều này cho phép bạn tạo các hàm vô danh (anonymous functions), tức là hàm không có tên.
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">sum = <span style="color: red;">function</span>(<span style="color: yellow;">a, b</span>) {</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: yellow;">return a + b;</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">};</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">console.log(<span style="color: yellow;">sum(2, 3)</span>); <span style="color: green;">// In ra: 5</span></p>
</div>

Trong ví dụ trên, hàm không có tên và được gán cho biến sum, sau đó có thể gọi hàm thông qua biến này.

<p style="font-size: 2em; font-weight: bold; color: black;">2. Hàm với Tham Số và Trả Về Giá Trị
<p style="text-indent: 50px;">Hàm có thể nhận một hoặc nhiều tham số và trả về một giá trị. Tham số của hàm là những giá trị được truyền vào hàm khi nó được gọi, còn giá trị trả về có thể được sử dụng trong các phép toán khác.

**a. Tham Số**
<p style="text-indent: 50px;">Tham số là các biến được khai báo trong dấu ngoặc đơn của hàm và được sử dụng trong thân hàm.

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">function <span style="color: red;">multiply</span>(<span style="color: yellow;">x, y</span>) {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: violet;">return</span> <span style="color: yellow;">x</span> <span style="color: yellow;">* y;</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">}</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">console.log(<span style="color: yellow;">multiply(2, 3)</span>); <span style="color: green;">//In ra: 6</span></p>
</div>

Hàm multiply nhận hai tham số x và y, và trả về giá trị của phép nhân chúng.

**b. Giá Trị Trả Về (Return)**
<p style="text-indent: 50px;">Hàm có thể trả về một giá trị sử dụng từ khóa return. Khi một giá trị được trả về, hàm sẽ kết thúc và không thực thi các mã còn lại.

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">function <span style="color: red;">square</span>(<span style="color: yellow;">number</span>) {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: violet;">return</span> <span style="color: yellow;">number</span> * <span style="color: yellow;">number</span>;</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">}</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">result = <span style="color: red;">square</span>(<span style="color: yellow;">4</span>);</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">console.log(<span style="color: yellow;">result</span>); <span style="color: green;">// In ra: 16</span></p>
</div>

<p style="font-size: 2em; font-weight: bold; color: black;">3. Hàm với Tham Số Mặc Định
<p style="text-indent: 50px;">JavaScript cho phép bạn gán giá trị mặc định cho các tham số hàm. Nếu không có giá trị được truyền vào khi gọi hàm, giá trị mặc định sẽ được sử dụng.

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">function <span style="color: red;">greet</span>(<span style="color: yellow;">name = <span style="color: red;">"Guest"</span></span>) {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: violet;">console.log(<span style="color: white;">"Hello, " + name + "!"</span>);</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">}</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">greet(); <span style="color: green;">// In ra: Hello, Guest!</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">greet(<span style="color: yellow;">"Alice"</span>); <span style="color: green;">// In ra: Hello, Alice!</span></p>
</div>

Trong ví dụ trên, nếu không truyền tham số name, giá trị mặc định là "Guest" sẽ được sử dụng.

<p style="font-size: 2em; font-weight: bold; color: black;">4. Hàm Nhanh (Arrow Function)
<p style="text-indent: 50px;">Trong ES6, JavaScript giới thiệu một cách khai báo hàm mới gọi là arrow function. Cú pháp của arrow function ngắn gọn hơn và không có từ khóa function, thay vào đó sử dụng dấu =>.

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">add = (<span style="color: white;">a, b</span>) => <span style="color: red;">a + b;</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">console.log(<span style="color: yellow;">add(2, 3)</span>); <span style="color: green;">// In ra: 5</span></p>
</div>

Arrow function rất hữu ích khi bạn muốn viết hàm ngắn gọn, nhưng cũng có những điểm khác biệt như không có this và không thể sử dụng làm hàm khởi tạo.

<p style="font-size: 2em; font-weight: bold; color: black;">5. Hàm Tự Gọi (IIFE - Immediately Invoked Function Expression)
<p style="text-indent: 50px;">IIFE là một biểu thức hàm được gọi ngay sau khi được khai báo. Cú pháp của IIFE là hàm được bao trong dấu ngoặc đơn, và sau đó được gọi ngay lập tức.

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">(<span style="color: red;">function</span>() {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: violet;">console.log(<span style="color: white;">"This is an IIFE!"</span>);</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">})();</p>
</div>

IIFE thường được sử dụng để tạo ra một phạm vi (scope) riêng biệt cho các biến trong hàm mà không làm ảnh hưởng đến phạm vi toàn cục.

<p style="font-size: 2em; font-weight: bold; color: black;">6. Hàm Tham Chiếu và Hàm Gọi Lại (Callback Functions)
<p style="text-indent: 50px;">Hàm trong JavaScript có thể được truyền như một tham số cho một hàm khác. Hàm nhận tham số này gọi là callback function.

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">function <span style="color: red;">processData</span>(<span style="color: yellow;">data, callback</span>) {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: violet;">console.log(<span style="color: white;">"Processing: " + data</span>);</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: violet;">callback();</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">}</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">function <span style="color: red;">showResult</span>() {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: violet;">console.log(<span style="color: white;">"Processing Complete!"</span>);</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">}</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">processData(<span style="color: yellow;">"File 1"</span>, <span style="color: yellow;">showResult</span>);</p>
</div>

Trong ví dụ trên, hàm showResult là một hàm callback được truyền vào hàm processData và được gọi sau khi quá trình xử lý dữ liệu hoàn tất.

<p style="font-size: 2em; font-weight: bold; color: black;">7. Hàm Đệ Quy (Recursive Functions)
<p style="text-indent: 50px;">Hàm đệ quy là hàm gọi chính nó trong quá trình thực thi. Hàm đệ quy rất mạnh mẽ và hữu ích trong việc giải quyết các bài toán phức tạp như tính toán giai thừa, tìm kiếm trong cây,…

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;"><span style="color: red;">function</span> <span style="color: yellow;">factorial</span>(<span style="color: yellow;">n</span>) {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: red;">if</span> (<span style="color: yellow;">n === 0</span>) {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">    <span style="color: yellow;">return</span> <span style="color: red;">1;</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  }</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: yellow;">return</span> <span style="color: yellow;">n</span> <span style="color: red;">*</span> <span style="color: yellow;">factorial(n - 1);</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">}</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">console.log(<span style="color: yellow;">factorial(5)</span>); // In ra: <span style="color: red;">120</span></p>
</div>

Trong ví dụ trên, hàm factorial tính giai thừa của một số thông qua việc gọi chính nó.

<p style="font-size: 2em; font-weight: bold; color: black;">8. Kết luận
<p style="text-indent: 50px;">Hàm là một phần quan trọng trong JavaScript, giúp bạn tổ chức và tái sử dụng mã dễ dàng. Từ việc khai báo các hàm cơ bản, đến việc sử dụng hàm dưới dạng biểu thức, arrow function, hàm đệ quy và callback function, JavaScript cung cấp nhiều công cụ mạnh mẽ để xử lý các tác vụ phức tạp.

<div style="display: flex; justify-content: space-between; align-items: center; margin: 20px 0;">
  <a href="https://dinhtanplinh03.github.io/posts/posts9/" style="display: inline-block; padding: 10px 20px; background-color: green; color: white; text-decoration: none; border-radius: 5px; font-size: 16px;">Quay lại bài trước</a>
</div>