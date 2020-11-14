### 背景:

最近编译原理布置作业，进行词法分析，在使用flex工具进行规则处理的时候遇到了需要将16进制字符串转化为10进制字符串的问题。由于很长时间没有接触过c++，很是生疏，而且当初进行学习的时候，并没有学习地很深入，所以在查了一些资料后，我写下这篇文章。

#### 方法：

##### 在这里大致有两种方式，将16进制转为10进制（排除c语言的写法）

- 第一种：

  ```c++
  #include <sstream>
   
  int x;
  stringstream ss;
  ss << std::hex << "1A";  //std::oct（八进制）、std::dec（十进制）
  ss >> x;
  cout << x<<endl;
  输出：26
  ```

- 第二种：

  ```c++
  string out = "1A";
  int x = stoi(out, nullptr, 16);
  cout << x <<endl;
   
  输出：26
  ```

博客内容来源：https://blog.csdn.net/MOU_IT/article/details/89060249，里面很是详细。

#### 其它

另外，由于我对string了解不多，发现其有很多用法。比如std::to_string()的很多用法，以及string和char*的转换，都是很重要的内容，以及string::data()和string::c_str()这些函数的用法，也很重要。

- https://blog.csdn.net/puppylpg/article/details/51260100 ，这篇博客主要讲述利用stringstream进行数据类型转换的方式。
- https://blog.csdn.net/u013066730/article/details/84105567 ，这篇主要讲了整型值和字符串的转换问题，但是只作为参考，比较杂。
- https://www.jianshu.com/p/266fca755967 ，代码很值得参考。