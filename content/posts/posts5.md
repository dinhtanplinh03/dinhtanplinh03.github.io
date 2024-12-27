---
title: "Biến, kiểu dữ liệu, truyền kiểu và chú thích (Phần 2)"
date: 2024-12-14
weight: 5
draft: false
---
<p style="text-indent: 50px;">JavaScript là một ngôn ngữ linh hoạt và được sử dụng rộng rãi nhờ khả năng làm việc với nhiều kiểu dữ liệu khác nhau. Trong bài viết này, chúng ta sẽ khám phá các kiểu dữ liệu chính trong JavaScript, bao gồm cách chúng hoạt động và khi nào nên sử dụng.
<p style="font-size: 2em; font-weight: bold; color: black;">1. Kiểu Dữ Liệu Nguyên Thủy (Primitive Types)
<p style="text-indent: 50px;">Kiểu dữ liệu nguyên thủy là những kiểu dữ liệu cơ bản nhất trong JavaScript. Mỗi giá trị thuộc kiểu nguyên thủ là một giá trị duy nhất và không thể thay đổi. Các kiểu dữ liệu nguyên thủ bao gồm:
<p style="font-size: 1.5em; font-weight: bold; color: black;">1.1. String
<p style="text-indent: 50px;">Đại diện cho các chuỗi ký tự.
Cách khai báo:
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;"> <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">name = <span style="color: red;">&ldquo;Alice&rdquo;;</span></span></p> <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">greeting = <span style="color: red;">&lsquo;Hello&rsquo;;</span></span></p> </div>
Lưu ý: Chuỗi trong JavaScript có thể được bao bọc bởi dấu nháy đơn (' ') hoặc nháy kép (" ").
<p style="font-size: 1.5em; font-weight: bold; color: black;">1.2. Number
<p style="text-indent: 50px;">Đại diện cho các con số, bao gồm số nguyên và số thực. Cách khai báo:
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">age = <span style="color: red;">25;</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">price = <span style="color: red;">99.99;</span></span></p>
</div>
Lưu ý: JavaScript chỉ có một kiểu số duy nhất, khác với nhiều ngôn ngữ khác.
<p style="font-size: 1.5em; font-weight: bold; color: black;">1.3. Boolean
<p style="text-indent: 50px;">Đại diện cho hai giá trị logic: true và false. Cách khai báo:
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">isLoggedIn = <span style="color: red;">true;</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">hasPermission = <span style="color: red;">false;</span></span></p>
</div>
<p style="font-size: 1.5em; font-weight: bold; color: black;">1.4. Undefined
<p style="text-indent: 50px;">Biểu thị một biến được khai báo nhưng chưa được gán giá trị. Cách khai báo:

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">user = <span style="color: red;">undefined;</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">console.log(<span style="color: yellow;">user</span>); <span style="color: green;">//undefined</span></p>
</div>
<p style="font-size: 1.5em; font-weight: bold; color: black;">1.5. Null
<p style="text-indent: 50px;">Đại diện cho giá trị "trống" hoặc "không tồn tại". Cách khai báo:
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">value = <span style="color: red;">null;</span></span></p>
</div>
<p style="font-size: 1.5em; font-weight: bold; color: black;">1.6. Symbol
<p style="text-indent: 50px;">Được giới thiệu trong ES6, biểu diễn một giá trị duy nhất và không trùng lặp. Cách khai báo:
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">uniqueId = <span style="color: red;">Symbol('id');</span></span></p>
</div>
<p style="font-size: 2em; font-weight: bold; color: black;">2. Kiểu Dữ Liệu Tham Chiếu (Reference Types)
<p style="text-indent: 50px;">Các kiểu dữ liệu tham chiếu bao gồm Object, Array, và Function. Đặc điểm của chúng là giá trị được lưu trữ bằng tham chiếu, không phải trực tiếp.
<p style="font-size: 1.5em; font-weight: bold; color: black;">2.1. Object
<p style="text-indent: 50px;">Là tập hợp các cặp key-value. Cách khai báo:
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">user = <span style="color: red;">{</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: yellow;">name:</span> <span style="color: red;">"Alice"</span>,</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">&nbsp;&nbsp;&nbsp;&nbsp;<span style="color: yellow;">age:</span> <span style="color: red;">25</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">}<span style="color: red;">;</span></p>
</div>
<p style="font-size: 1.5em; font-weight: bold; color: black;">2.2. Array
<p style="text-indent: 50px;">Là danh sách các phần tử. Cách khai báo:
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">colors = <span style="color: red;">["red", "green", "blue"];</span></span></p>
</div>
<p style="font-size: 1.5em; font-weight: bold; color: black;">2.3. Function
<p style="text-indent: 50px;">Là khối mã chứa các tác vụ. Cách khai báo:
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">function <span style="color: yellow;">greet</span>()</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">{</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">    <span style="color: yellow;">console.log</span>(<span style="color: red;">"Hello, World!"</span>);</p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">}</p>
</div>

<div style="display: flex; justify-content: space-between; align-items: center; margin: 20px 0;">
  <a href="http://localhost:1313/dinhtanplinh03/dinhtanplinh03.github.io.git/posts/posts4/" style="display: inline-block; padding: 10px 20px; background-color: green; color: white; text-decoration: none; border-radius: 5px; font-size: 16px;">Quay lại bài trước</a>
  <a href="http://localhost:1313/dinhtanplinh03/dinhtanplinh03.github.io.git/posts/posts6/" style="display: inline-block; padding: 10px 20px; background-color: green; color: white; text-decoration: none; border-radius: 5px; font-size: 16px;">Chuyển sang bài tiếp theo</a>
</div>