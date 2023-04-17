| 优先级 | 运算符 | 描述 | 结合性 |
|:-:|------|:------|--------|
| 1      | ::     | 作用域解析 | 左到右 |
| 2      | a++&emsp;a-- <br> type(  )&emsp;type{  } <br> a(  ) <br> a[  ] <br> <strong>.&emsp;-></strong> | 后缀自增与自减 <br> 函数风格转型 <br> 函数调用 <br> 下标 <br> 成员访问 | 左到右 |
| 3      | ++a&emsp;--a <br> +a&emsp;-a <br>!&emsp;~ <br> *(type)* <br> *a <br> &a <br> sizeof <br> co_await <br> new&emsp;new[ ]	<br>delete&emsp;delete[ ]	| 前缀自增与自减 <br> 一元加与减 <br> 逻辑非和逐位非 <br> C 风格转型 <br> 间接（解引用） <br> 取址 <br> 取大小 <br> await 表达式 (C++20)<br> 动态内存分配<br> 动态内存分配|**<font color =red>右到左</font>**|
| 4      | <strong>.* &emsp;->*</strong> | 成员指针 | 左到右 |
| 5      | *&emsp;/&emsp;% | 乘法、除法与余数 | 左到右 |
| 6      | +&emsp;- | 加法与减法 | 左到右 |
| 7      | <<&emsp;>> | 逐位左移与右移 | 左到右 |
| 8      | <=> | 三路比较运算符(C++20 起) | 左到右 |
| 9      | <&emsp;≤ <br> >&emsp;≥ |分别为 < 与 ≤ 的关系运算符<br>分别为 > 与 ≥ 的关系运算符| 左到右 |
| 10     | ==&emsp;!= | 分别为 = 与 ≠ 的相等性运算符 | 左到右 |
| 11     | & | 逐位与 | 左到右 |
| 12     | ^ | 逐位异或（互斥或） | 左到右 |
| 13     | \| | 逐位或（可兼或） | 左到右 |
| 14     | && | 逻辑与 | 左到右 |
| 15     | \|\| | 逻辑或 | 左到右 |
| 16     |a?b:c<br>throw<br>co_yield<br>=<br>+=&emsp;-=<br>*=&emsp;/=&emsp;%=<br><<=&emsp;>>=<br>&=&emsp;^=&emsp;\|=|三元条件<br>throw运算符<br>yield 表达式 (C++20)<br>直接赋值（C++ 类默认提供）<br>以和及差复合赋值<br> 以积、商及余数复合赋值<br> 以逐位左移及右移复合赋值<br>以逐位与、异或及或复合赋值 |**<font color =red>右到左</font>**|
| 17     | , | 逗号 | 左到右 |
	
