---
layout: default
title: C++ Primer 中文版(第4版)
---

{{ page.title }}
================

## Chapter 1

### 1.1
主函数

<pre>
int main()
{
    return 0; # Means success
} # this is curly brace
</pre>

函数必须指定4个元素：返回类型, 函数名, 形参表, 函数体。  

Linux下编译：

{% highlight ruby linenos %}
g++ hello.cc –o hello
./hello # Execute
echo $? # see the return value from main
{% endhighlight %}


### 1.2
Preprocessor directive: include尖括号中是头文件。标准库用`<>`括起来。自定义库用`""`。  

iostream
* istream：cin。输入值与存入的变量类型不符合时, 或读入`ctrl+D`时, 返回的值为假, 可用于while的中。  
* ostream：cout,  cerror, clog。  
* iostream库能所有处理内置类型的输出。  
```

#include <iosteam>
int main()
{
    std::cout << "Enter two numbers: " << std::endl; # std::endl is one of manipulators
    int v1, v2; 
    std::cin >> v1 >> v2; 
    std::cout << "Sum :" << v1 + v2 << std::endl; 
}
```

`<<`操作符：每次接受两个操作数, 左边为ostream对象, 右边为内容。该表达式执行完后, 返回void*的ostream对象。  
Manipulator操作符：`endl`, 换行并刷新缓冲区(buff)。  

调用前需有`std::`是使用命名空间(namespace)std内的函数或操作符避免定义变量时冲突。  
作用域(Scope)操作符：取namespace中的对象。  

对于出错的情况：
```
    std::cerr << "Error" << std::endl;


