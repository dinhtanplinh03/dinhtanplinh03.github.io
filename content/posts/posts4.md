---
title: "Biến, kiểu dữ liệu, truyền kiểu và chú thích (Phần 1)"
date: 2024-12-13
weight: 4
draft: false
---
<p style="text-indent: 50px;">Để sử dụng JavaScriptJavaScript một cách hiệu quả, việc hiểu rõ các khái niệm cơ bản như biến, kiểu dữ liệu, truyền kiểu và chú thích là rất quan trọng. Trong bài viết này, chúng ta sẽ cùng tìm hiểu các khái niệm này một cách chi tiết.
<p style="text-indent: 50px;">Vì bài viết này tìm hiểu khá nhiều khái niệm nên tôi sẽ chia nó làm nhiều phần.
<p style="font-size: 2em; font-weight: bold; color: black;">1. Biến là gì?
<p style="text-indent: 50px;">Bạn hãy tưởng tượng rằng dòng chữ Hello World mà chúng ta in ra trong bài trước chính là một món hàng. Nhưng để có thể sử dụng món hàng đó bất cứ khi nào, chúng ta cần một chiếc hộp để đựng nó. Chiếc hộp đó chính là biến trong lập trình. Một chiếc hộp (biến) trong JavaScript có thể chứa bất kỳ thứ gì bạn muốn: một con số, một đoạn chữ, hay thậm chí là một mệnh lệnh. Khi bạn đặt món hàng vào chiếc hộp, bạn có thể dán nhãn cho nó để dễ nhớ. Nhãn đó chính là tên biến.
<p style="font-size: 2em; font-weight: bold; color: black;">2. Cách khai báo biến trong JavaScript
<p style="text-indent: 50px;">Để tạo ra chiếc hộp này, chúng ta sử dụng các từ khóa "let", "const", hoặc "var". Hãy hình dung rằng những từ khóa này giống như các loại hộp khác nhau, mỗi loại có đặc điểm riêng.

<p style="text-indent: 50px; font-weight: bold;">Khai báo một chiếc hộp (biến)
<div style="display: flex; justify-content: center; align-items: center; height: auto; background-color:white">
    <p style="background-color: black; color: blue; display: inline;">let <span style="color: yellow;">message = <span style="color: red;">Hello, World!";</span></span></p>
</div>
"let" là cách bạn nói với JavaScript: "Hãy tạo một chiếc hộp có thể thay đổi, và tôi đặt tên cho nó là message.". Nội dung bên trong hộp là "Hello, World!".
<p style="text-indent: 50px;">Giờ bạn có thể dùng chiếc hộp này bất kỳ lúc nào. Chỉ cần gọi tên "message", JavaScript sẽ lấy dữ liệu bên trong hộp ra cho bạn.

<p style="text-indent: 50px; font-weight: bold;">Thay đổi nội dung hộp (biến)
<div style="display: flex; justify-content: center; align-items: center; height: auto; background-color:white">
    <p style="background-color: black; color: blue; display: inline;"><span style="color: yellow;">message = <span style="color: red;">Hello, JavaScript!";</span></span></p>
</div>
Chiếc hộp vẫn giữ nguyên tên, nhưng bạn có thể thay đổi món hàng bên trong.
<p style="text-indent: 50px; font-weight: bold;">Khai báo một hộp (biến) không đổi
<div style="display: flex; justify-content: center; align-items: center; height: auto; background-color:white">
    <p style="background-color: black; color: violet; display: inline;">const <span style="color: yellow;">pi = <span style="color: red;">3,14;</span></span></p>
</div>
Với "const", bạn tạo ra một chiếc hộp mà nội dung bên trong không thể thay đổi. Một khi bạn đã đặt 3.14 vào, bạn không thể thay thế nó bằng một giá trị khác.
<p style="font-size: 2em; font-weight: bold; color: black;">3. Biến giúp ích gì?
<p style="text-indent: 50px;">Bạn có thể nghĩ rằng "Tại sao không dùng trực tiếp nội dung như "Hello, World!" mà cần biến?" Câu trả lời là: biến giúp bạn tái sử dụng và tổ chức dữ liệu dễ dàng hơn.

<p style="text-indent: 50px;">Ví dụ: Tái sử dụng dữ liệu. Thay vì viết đi viết lại "Hello, World!" mỗi lần cần in, bạn chỉ cần dùng biến:
<div style="display: flex; flex-direction: column; align-items: flex-start; justify-content: center; height: auto; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 5px; padding: 5px;">let <span style="color: yellow;">message = <span style="color: red;">"Hello World!";</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 5px; padding: 5px;">console.<span style="color: yellow;">log(<span style="color: red;">message);</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 5px; padding: 5px;">console.<span style="color: yellow;">log(<span style="color: red;">message);</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 5px; padding: 5px;">console.<span style="color: yellow;">log(<span style="color: red;">message);</span></span></p>
</div>
<p style="text-indent: 50px;">Ví dụ: Thay đổi dữ liệu linh hoạt. Nếu bạn cần thay đổi nội dung, chỉ cần cập nhật biến:
<div style="display: flex; flex-direction: column; align-items: flex-start; justify-content: center; height: auto; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 5px; padding: 5px;">let <span style="color: yellow;">message</span> = <span style="color: red;">"Hello, World!";</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 5px; padding: 5px;">console.<span style="color: yellow;">log</span>(<span style="color: red;">message</span>);</p>
    <p style="background-color: black; color: violet; display: block; margin: 5px; padding: 5px;">message = <span style="color: red;">"Hello, JavaScript!";</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 5px; padding: 5px;">console.<span style="color: yellow;">log</span>(<span style="color: red;">message</span>);</p>
</div>
<p style="text-indent: 50px;">Bạn không cần sửa tất cả các chỗ dùng "Hello, World!" trong mã nguồn, giúp bạn tiết kiệm thời gian.
<p style="font-size: 2em; font-weight: bold; color: black;">4. Tên biến - Ghi nhớ và hiểu
<p style="text-indent: 50px;">Tên biến giống như nhãn trên hộp. Nếu bạn đặt tên biến rõ ràng, bạn sẽ dễ dàng hiểu được vai trò của biến đó. Một số quy tắc và gợi ý:

- **Tên biến phải bắt đầu bằng chữ cái, _, hoặc $.**

- **Không được chứa khoảng trắng, các từ khóa hoặc ký tự đặc biệt.**

<p style="text-indent: 50px;">Hãy chọn tên gợi nhớ ý nghĩa, ví dụ:

<div style="display: flex; flex-direction: column; align-items: flex-start; justify-content: center; height: auto; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 5px; padding: 5px;">let <span style="color: yellow;">userName</span> = <span style="color: red;">"Alice";</span></p>
    <p style="background-color: black; color: violet; display: block; margin: 5px; padding: 5px;">let <span style="color: yellow;">age</span> = <span style="color: red;">25;</span></p>
</div>
<p style="font-size: 2em; font-weight: bold; color: black;">5. Kết luận
<p style="text-indent: 50px;">Biến là một khái niệm cốt lõi trong JavaScript. Hãy nghĩ về nó như những chiếc hộp giúp bạn lưu trữ và tổ chức dữ liệu một cách hiệu quả. Khi bạn hiểu cách sử dụng biến, bạn đã bước thêm một bước gần hơn đến việc làm chủ JavaScript!

<div style="display: flex; justify-content: space-between; align-items: center; margin: 20px 0;">
  <a href="http://localhost:1313/dinhtanplinh03/dinhtanplinh03.github.io.git/posts/posts3/" style="display: inline-block; padding: 10px 20px; background-color: green; color: white; text-decoration: none; border-radius: 5px; font-size: 16px;">Quay lại bài trước</a>
  <a href="http://localhost:1313/dinhtanplinh03/dinhtanplinh03.github.io.git/posts/posts5/" style="display: inline-block; padding: 10px 20px; background-color: green; color: white; text-decoration: none; border-radius: 5px; font-size: 16px;">Chuyển sang bài tiếp theo</a>
</div>