---
title: "Toán tử gán, số học và logic"
date: 2024-12-16
weight: 7
draft: false
---
<p style="font-size: 2em; font-weight: bold; color: black;">1. Toán Tử Gán
<p style="text-indent: 50px;">Toán tử gán trong JavaScript được sử dụng để gán giá trị cho biến. Cách sử dụng phổ biến nhất là toán tử "=". Tuy nhiên, JavaScript cung cấp một số toán tử gán mở rộng để giúp việc gán trở nên dễ dàng hơn.

**Toán tử "=:"** Gán giá trị cho biến.
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">a = <span style="color: red;">10;</span></span> <span style="color: green;">// Gán giá trị 10 cho biến a</span></p>
</div>

**Toán tử +=:** Gán giá trị mới bằng cách cộng thêm một giá trị vào giá trị hiện tại.


<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">b = <span style="color: red;">5;</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">b <span style="color: yellow;">+=</span> <span style="color: red;">3;</span><span style="color: green;"> // b = b + 3 => b = 8</span></p>
</div>

**Toán tử -=:** Gán giá trị mới bằng cách trừ đi một giá trị.

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">c = <span style="color: red;">10;</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">c <span style="color: yellow;">-=</span> <span style="color: red;">4;</span> <span style="color: green;">// c = c - 4 =&gt; c = 6</span></p>
</div>

**Toán tử =:** Gán giá trị mới bằng cách nhân với một giá trị.

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">d = <span style="color: red;">2;</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">d <span style="color: yellow;">*=</span><span style="color: red;"> 5;</span> <span style="color: green;">// d = d * 5 => d = 10</span></p>
</div>

**Toán tử /=:** Gán giá trị mới bằng cách chia cho một giá trị.
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">e = <span style="color: red;">20;</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">e <span style="color: yellow;">/=</span> <span style="color: red;">4;</span><span style="color: green;"> // e = e / 4 => e = 5</span></p>
</div>

**Toán tử %=:** Gán giá trị mới bằng phép chia lấy dư.

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">f = <span style="color: red;">10;</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">f <span style="color: yellow;">%=</span> <span style="color: red;">3;</span><span style="color: green;"> // f = f % 3 => f = 1</span></p>
</div>
<p style="font-size: 2em; font-weight: bold; color: black;">2. Toán Tử Số Học
<p style="text-indent: 50px;">Toán tử số học trong JavaScript được sử dụng để thực hiện các phép toán cơ bản.

**Toán tử +:** Cộng hai giá trị lại.

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">sum = <span style="color: red;">10 <span style="color: yellow;">+</span> 5;</span></span><span style="color: green;"> // sum = 15</span></p>
</div>

**Toán tử -:** Trừ hai giá trị.

<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">difference = <span style="color: red;">10 <span style="color: yellow;">-</span> 5;</span></span><span style="color: green;"> // difference = 5</span></p>
</div>

**Toán tử * :** Nhân hai giá trị.
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">product = <span style="color: red;">10 <span style="color: yellow;">*</span> 5;</span></span><span style="color: green;"> // product = 50</span></p>
</div>

**Toán tử /:** Chia hai giá trị.
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">quotient = <span style="color: red;">10 <span style="color: yellow;">/</span> 2;</span></span><span style="color: green;"> // quotient = 5</span></p>
</div>

**Toán tử %:** Lấy dư của phép chia.
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">remainder = <span style="color: red;">10 <span style="color: yellow;">%</span> 3;</span></span><span style="color: green;"> // remainder = 1</span></p>
</div>
<p style="font-size: 2em; font-weight: bold; color: black;">3. Toán Tử Logic
<p style="text-indent: 50px;">Toán tử logic trong JavaScript được sử dụng để thực hiện các phép toán logic với các giá trị boolean (true hoặc false).

**Toán tử && (AND):** Trả về true nếu cả hai biểu thức đều đúng.
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">a = <span style="color: red;">true;</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">b = <span style="color: red;">false;</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">result = <span style="color: red;">a <span style="color: yellow;">&&</span> b;</span></span><span style="color: green;"> // result = false</span></p>
</div>

**Toán tử || (OR):** Trả về true nếu ít nhất một trong các biểu thức đúng.
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">a = <span style="color: red;">true;</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">b = <span style="color: red;">false;</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">result = <span style="color: red;">a <span style="color: yellow;">||</span> b;</span></span> <span style="color: green;">// result = true</span></p>
</div>

**Toán tử ! (NOT):** Đảo ngược giá trị boolean của biểu thức.
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">a = <span style="color: red;">true;</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">result = <span style="color: red;">!a;</span></span> <span style="color: green;">// result = false</span></p>
</div>

**Toán tử ?? (Nullish Coalescing):** Trả về giá trị bên trái nếu nó khác null hoặc undefined, nếu không thì trả về giá trị bên phải.
<div style="display: flex; flex-direction: column; align-items: flex-start; background-color: black; padding: 10px;">
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">a = <span style="color: red;">null;</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">b = <span style="color: red;">"Hello";</span></span></p>
    <p style="background-color: black; color: violet; display: block; margin: 0; padding: 5px;">let <span style="color: yellow;">result = <span style="color: red;">a <span style="color: yellow;">??</span> b;</span></span><span style="color: green;"> // result = "Hello"</span></p>
</div>
<p style="font-size: 2em; font-weight: bold; color: black;">4. Kết luận
<p style="text-indent: 50px;">Các toán tử trong JavaScript giúp bạn thực hiện các phép toán cơ bản, từ gán giá trị, thực hiện các phép toán số học đến các phép toán logic. Việc hiểu rõ cách sử dụng chúng sẽ giúp bạn viết mã hiệu quả hơn và dễ dàng giải quyết các vấn đề trong lập trình.

<!-- <div style="display: flex; justify-content: space-between; align-items: center; margin: 20px 0;">
  <a href="https://dinhtanplinh03.github.io/posts/posts6/" style="display: inline-block; padding: 10px 20px; background-color: green; color: white; text-decoration: none; border-radius: 5px; font-size: 16px;">Quay lại bài trước</a>
  <a href="https://dinhtanplinh03.github.io/posts/posts8/" style="display: inline-block; padding: 10px 20px; background-color: green; color: white; text-decoration: none; border-radius: 5px; font-size: 16px;">Chuyển sang bài tiếp theo</a>
</div> -->