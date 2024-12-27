---
title: "Điều kiện và vòng lăp trong JavaScript"
date: 2024-12-17
weight: 8
draft: false
---
<p style="font-size: 2em; font-weight: bold; color: black;">1. Điều Kiện trong JavaScript
<p style="text-indent: 50px;">Điều kiện trong JavaScript giúp chúng ta kiểm tra các biểu thức và thực hiện các hành động khác nhau dựa trên kết quả của việc kiểm tra. JavaScript cung cấp các cấu trúc điều kiện như if, else, else if, và switch để xử lý các tình huống khác nhau.

**a. Câu Lệnh if**
<p style="text-indent: 50px;">Câu lệnh if cho phép bạn kiểm tra một điều kiện và thực hiện một hành động nếu điều kiện đó đúng (true).
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">age = 18</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;"><span style="color: red;">if</span>  (<span style="color: yellow;">age >= 18</span>) {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: yellow;">console.log</span>(<span style="color: white;">"Bạn đã đủ tuổi để lái xe."</span>); </p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">}</p>
</div>


**b. Câu Lệnh else**
<p style="text-indent: 50px;">Câu lệnh else được sử dụng sau câu lệnh if để thực hiện một hành động nếu điều kiện trong if không đúng (false).
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">age = 16;</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;"><span style="color: red;">if</span> (<span style="color: yellow;">age >= 18</span>) {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: violet;">console.log(<span style="color: white;">"Bạn đã đủ tuổi để lái xe.</span>");</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">}<span style="color: red;"> else </span>{</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: violet;">console.log(<span style="color: white;">"Bạn chưa đủ tuổi để lái xe."</span>);</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">}</p>
</div>

**c. Câu Lệnh else if**
<p style="text-indent: 50px;">Khi bạn cần kiểm tra nhiều điều kiện, bạn có thể sử dụng else if để kiểm tra các điều kiện bổ sung.

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">age =20;</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;"><span style="color: red;">if</span> (<span style="color: yellow;">age < 18</span>) {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: violet;">console.log(<span style="color: white;">"Bạn là thiếu niên."</span>);</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">} <span style="color: red;">else if</span> (<span style="color: yellow;">age >= 18 && age <= 60</span>) {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: violet;">console.log(<span style="color: white;">"Bạn là người trưởng thành."</span>);</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">} <span style="color: red;">else</span> {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: violet;">console.log(<span style="color: white;">"Bạn là người cao tuổi."</span>);</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">}</p>
</div>

**d. Câu Lệnh switch**
<p style="text-indent: 50px;">Câu lệnh switch là một cách khác để kiểm tra nhiều điều kiện, nhưng với cú pháp ngắn gọn hơn so với chuỗi các câu lệnh if-else.

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">day = <span style="color: red;">2;</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">dayName;</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;"><span style="color: red;">switch</span> (<span style="color: yellow;">day</span>) {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: red;">case</span> <span style="color: yellow;">1:</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">    dayName = <span style="color: white;">"Thứ Hai";</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">    <span style="color: red;">break;</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: red;">case</span> <span style="color: yellow;">2:</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">    dayName = <span style="color: white;">"Thứ Ba";</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">    <span style="color: red;">break;</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: red;">case</span> <span style="color: yellow;">3:</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">    dayName = <span style="color: white;">"Thứ Tư";</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">    <span style="color: red;">break;</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: red;">default</span>:</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">    dayName = <span style="color: white;">"Ngày không hợp lệ";</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">}</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">console.log(<span style="color: yellow;">dayName</span>); // <span style="color: white;">In ra "Thứ Ba"</span></p>
</div>

<p style="font-size: 2em; font-weight: bold; color: black;">2. Vòng Lặp trong JavaScript
<p style="text-indent: 50px;">Vòng lặp là một cấu trúc điều khiển giúp bạn thực hiện một đoạn mã nhiều lần. JavaScript hỗ trợ nhiều loại vòng lặp khác nhau, bao gồm for, while, do...while, và vòng lặp for...in và for...of.

**a. Vòng Lặp for**
<p style="text-indent: 50px;">Vòng lặp for được sử dụng khi bạn biết trước số lần lặp. Cú pháp cơ bản của vòng lặp for gồm ba phần: khởi tạo, điều kiện và bước nhảy.

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">for (<span style="color: yellow;">let i = 0; i < 5; i++</span>) {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: violet;">console.log(<span style="color: white;">i</span>);</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">}</p>
</div>
Trong ví dụ trên, vòng lặp sẽ in ra các số từ 0 đến 4.

**b. Vòng Lặp while**
<p style="text-indent: 50px;">Vòng lặp while sẽ tiếp tục thực hiện một khối mã cho đến khi điều kiện kiểm tra trở thành false. Điều này có nghĩa là nếu điều kiện không được thỏa mãn ngay từ đầu, vòng lặp có thể không thực thi một lần nào.
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">i = <span style="color: red;">0;</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;"><span style="color: red;">while</span> (<span style="color: yellow;">i < 5</span>) {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: violet;">console.log(<span style="color: white;">i</span>);</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: yellow;">i++;</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">}</p>
</div>
Vòng lặp trên sẽ cho kết quả giống như vòng lặp for, nhưng cú pháp khác.

**c. Vòng Lặp do...while**
<p style="text-indent: 50px;">Vòng lặp do...while tương tự như vòng lặp while, nhưng nó đảm bảo rằng khối mã sẽ được thực thi ít nhất một lần, vì điều kiện được kiểm tra sau khi khối mã thực thi.
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">i = <span style="color: red;">0;</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;"><span style="color: red;">do</span> {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: violet;">console.log(<span style="color: white;">i</span>);</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: yellow;">i++;</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">} <span style="color: red;">while</span> (<span style="color: yellow;">i &lt; 5</span>);</p>
</div>

**d. Vòng Lặp for...in**
<p style="text-indent: 50px;">Vòng lặp for...in được sử dụng để lặp qua các thuộc tính của một đối tượng.

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">person = <span style="color: red;">{ name: "John", age: 30, city: "New York" };</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;"><span style="color: red;">for</span> (<span style="color: yellow;">let key</span> <span style="color: red;">in</span> <span style="color: yellow;">person</span>) {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: violet;">console.log(<span style="color: white;">key + ": " + person[key]</span>);</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">}</p>
</div>

Kết quả sẽ là:
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">name: <span style="color: yellow;">John</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">age: <span style="color: yellow;">30</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">city: <span style="color: yellow;">New York</span></p>
</div>

**e. Vòng Lặp for...of**
<p style="text-indent: 50px;">Vòng lặp for...of được sử dụng để lặp qua các phần tử của một mảng hoặc các đối tượng có thể lặp khác như chuỗi (string).

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">numbers = <span style="color: red;">[1, 2, 3, 4, 5];</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;"><span style="color: red;">for</span> (<span style="color: yellow;">let number of numbers</span>) {</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">  <span style="color: violet;">console.log(<span style="color: white;">number</span>);</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">}</p>
</div>
Kết quả sẽ là:
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">1</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">2</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">3</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">4</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">5</p>
</div>

<p style="font-size: 2em; font-weight: bold; color: black;">3. Kết luận
<p style="text-indent: 50px;">Điều kiện và vòng lặp là những công cụ quan trọng trong JavaScript giúp bạn kiểm tra các giá trị và lặp lại các thao tác một cách linh hoạt. Việc hiểu và sử dụng thành thạo các cấu trúc này giúp bạn viết mã hiệu quả và dễ dàng quản lý luồng chương trình.

<div style="display: flex; justify-content: space-between; align-items: center; margin: 20px 0;">
  <a href="http://localhost:1313/dinhtanplinh03/dinhtanplinh03.github.io.git/posts/posts7/" style="display: inline-block; padding: 10px 20px; background-color: green; color: white; text-decoration: none; border-radius: 5px; font-size: 16px;">Quay lại bài trước</a>
  <a href="http://localhost:1313/dinhtanplinh03/dinhtanplinh03.github.io.git/posts/posts9/" style="display: inline-block; padding: 10px 20px; background-color: green; color: white; text-decoration: none; border-radius: 5px; font-size: 16px;">Chuyển sang bài tiếp theo</a>
</div>