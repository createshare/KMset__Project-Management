# MISRA C 2012 编程规范

- MISRA C 是由汽车产业软件可靠性协会（MISRA）提出的C语言开发标准。其目的是在增进嵌入式系统的安全性及可移植性。

- 针对 C++ 语言也有对应的标准 MISRA C++。

- MISRA C 一开始主要是针对汽车产业，不过其他产业也逐渐开始使用 MISRA C：包括航天、电信、国防、医疗设备、铁路等领域中都已有厂商使用 MISRA C。

- 2012 年发布第三版，为当前最新有效的C语言规范版本，称为 MISRAC:2012。 

-  Misra C 不能 100% 保证程序不出问题，但是能尽可能的预防.
- 总结一下，基本上使用Misra C具有以下五个维度的优势：
  - 提升可靠性
  - 提升可读性
  - 提升可移植性
  - 提升可维护性
  - 提升安全性
    

# MISRA C 2012 强制项列表

| MISRA  C：2012/AMD2  强制项 | 内容                                                         | 翻译                                                         |
| --------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| R.9.1                       | The value of an object with  automatic storage duration shall not be read before it has been set | 具有自动存储持续时间的对象(临时变量)的值在设置前不得读取     |
| R.12.5                      | The sizeof operator shall not have an operand which is a function paramter  declared as "array of type" | sizeof  运算符的操作数不得包含任何被声明为数组类型的函数参数 |
| R.13.6                      | The operand of the sizeof operator shall not contain  any expression which has potential side effects | sizeof 运算符的操作数不得包含任何可能产生副作用的表达式      |
| R.17.3                      | A function shall not be declared  implicitly                 | 禁止隐式声明函数                                             |
| R.17.4                      | ALL exit paths from a function  with non-void return type shall have an explicit  return statement with an expression | 具有非void  返回类型的函数的所有退出路径都应为具有带有表达式的显式     return 语句 |
| R.17.6                      | The declaration of an array  parameter shall not contain the static keyword between the [] | 数组形参的声明不得在[]之间包含static 关键字                  |
| R.19.1                      | An object shall not be assigned  or copied to an overlapping object | 不得将对象赋值或复制给重叠的对象                             |
| R.21.13                     | Any value passed to a function  in <ctype.h> shall be representable as an unsigned char or be the value  EOF | 任何被传给<ctype.h>中函数的值都应是unsigned  char类型或EOF   |
| R.21.17                     | Use of the string handling  functions from <string.h> shall not result in accesses beyond the  bounds of the objects referenced by their pointer parameters | 使用<string.h>中的字符串处理函数不应导致超出指针参数所引用对象范围的访问 |
| R.21.18                     | The size_t argument passed to  any function in <string.h> shall have an appropriate value | 将size_t参数传递给<string.h>中任意函数，应有适当的值         |
| R.21.19                     | The pointers returned by the  Standard Library functions localeconv，getenv,setlocale or strerror shall only be used as if they have pointer to const-qualified  type | 标准库函数localeconv、getenv、setlocale或strerror返回的指针只能作为具有const限定类型的指针使用 |
| R.21.20                     | The pointers returned by the  Standard Library functions asctime,ctime,gmtime,localtime,localeconv,getenv,setlocale  or strerror shall not be used following a subsequent call to the same  function | 由标准库函数asctime,ctime,gmtime,localtime,localeconv,getenv,setlocale或strerror返回的指针不能在后续调用同一个函数之后使用 |
| R.22.2                      | A block of memory shall only be  freed if it was allocated by means of a Standard Library function | 只有通过标准库函数分配的内存块才能释放                       |
| R.22.4                      | There shall be no attempt to  write to a stream which has been opened as read-only | 禁止尝试对以只读方式打开的流执行写操作                       |
| R.22.5                      | A pointer to a FILE object shall  not be dereferenced        | 禁止反引用指向FILE 对象的指针                                |
| R.22.6                      | The value of a pointer to a FILE  shall not be used after the associated stream has been closed | 关联的流关闭后，禁止再使用指向FILE 的指针                    |





![XXX](figures/XXX.jpg)



