# C++ Primer ���İ�
## Chapter 1
### 1.1
������
```
int main()
{
    return 0; # Means success
} # this is curly brace
```
��������ָ��4��Ԫ�أ���������, ������, �βα�, �����塣  

Linux�±��룺
```
g++ hello.cc �Co hello
./hello # Execute
echo $? # see the return value from main
```

### 1.2
Preprocessor directive: include����������ͷ�ļ�����׼����`<>`���������Զ������`""`��  

iostream
* istream��cin������ֵ�����ı������Ͳ�����ʱ, �����`ctrl+D`ʱ, ���ص�ֵΪ��, ������while���С�  
* ostream��cout,  cerror, clog��  
* iostream�������д����������͵������  
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

`<<`��������ÿ�ν�������������, ���Ϊostream����, �ұ�Ϊ���ݡ��ñ��ʽִ�����, ����void*��ostream����  
Manipulator��������`endl`, ���в�ˢ�»�����(buff)��  

����ǰ����`std::`��ʹ�������ռ�(namespace)std�ڵĺ�������������ⶨ�����ʱ��ͻ��  
������(Scope)��������ȡnamespace�еĶ���  

���ڳ���������
```
    std::cerr << "Error" << std::endl;
    return -1;
```

�������ͣ���int����ö�����ֵ��  

### 1.3
����ע�ͣ�
```
/*
 *
 */
```

### 1.4
���ƽṹ:  
����while������������ʽ���ط�0ʱִ�С�  
```
int sum = 0, val;
while(std::cin >> val) 
    sum += val;
```

��ѭ������for��ѭ��������ѭ�������ͷ�, �������á�  
```
int sum=0;
for(int val = 1; val <= 10; ++val)
	sum += val;
```

����ִ��if��    
```
if(����)
	ִ��;
else
	ִ��;
```

### 1.5
��(class):  
�Զ����������͡�istreamҲ�ǡ�  
��Ҫ�أ����֡������򡢿�ִ�в�����  
������һ����������ͬ�Һ�׺Ϊ`.h`�ļ��С�  
ʵ������
```
Sales_item item; 
```
Sales_item����, item�Ƕ���

��Ա������`item.same_isbn(item2)`�Ǻ�����  
���Ը�д��������  

�������.�������������Ķ���, �Ҳ������ǳ�Ա��  
���ò�����()����סʵ�Ρ�  

### 1.6

### С��
Argument: ʵ��; Parameter: �βΡ�Statement: ��䡣  

Routine: һϵ�в�����ɡ����Զ��庯�����������͡�  
Statically typed: C�Ƕ�smalltalk���ǡ�  

## Chapter 2
### 2.1
��������(arithmetic type)��
* bool,  true, false������Ϊ�κ��������͡�
* char(8 bit, 1 byte), wchar_t���������(16λ)��ÿ���ַ�����ֵΪliteral constant��
* short(16λ), int(16λ), long(32λ),  ����ʱǰ�ɼ� unsigned��C++��-1��unsigned���͵�4294967295(��������й�)��unsigned �������������±ꡣԽ��ᱻwrap around��
* float (32 bit) 6λ��Ч����, double (32 bit) 10λ��Ч����, long double (96 ��128 bit)10λ��Ч���֡�double ������Ч�ʿ��ܱ�float ���ߡ�
Void type.  

�ڴ����: ��Ϊ���д洢, ��chunk ������, 32 bitΪһ��word��ÿ��byte ��һ����ַ��

### 2.2
20��ͬ��20 (decimal), 024 (octal), 0x14 (hexadecimal)��  
20UL�õ�long��unsigned���͡�  
�����ȸ���: 3.14159F = 3.14159E0f 0. = 0e0, 1E-3F = .001f  
wchar_t����: L'a'��  
ת���ַ�(Escape characters)��`\n`, `\t`, `\v` �����Ʊ��, `\b`�˸����, `\r`, `\12` �س���, `\f` ��ֽ��, `\a` ������, `\0` ���ַ�, `\40` �ո����`\xxx` (�˽�����) = (char)0xxx��  
�ַ�����`cout<<"a" "b""c"`�����ÿո񡢻س���tab����������ĩβ�Զ���ӿ��ַ���'A' ��һ���ַ�����"A" ��'A', '\12' �����ַ���

escape `\`: ���ԶϿ����������С�������֮���пո��ע�͡���һ�еĵ�һ���ַ�, �����ǿո��tab�������, ���Բ�������������  

nonportable: ����δ������Ϊ���, �罫char string ��long string ���� `"apple" L"banana"`��  

### 2.3
��ֵ(lvalue): ���������ɳ����ڸ�ֵ���������ҡ���ֵ(rvalue): ��������ֻ�����ҡ�  

����: �ڴ��о������͵�����  

C���Դ�Сд���С��ҹؼ��ʺ������������Ϊ������(identifier)��������������`_`����ĸ��ͷ��  

�ؼ��ʱ�

|  1  |  2  |  3  |  4  |  5  |  6  |  7  |  8  |  9  |  0  |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|asm|do|if|return|try|auto|double|inline|short|typedef| 
|bool|dynamic_cast|int|signed|typeid|break|else|long|sizeof|typename|
|case|enum|mutable|static|union|catch|explicit|namespace|staitc_cast|unsigned|
|char|export|new|struct|using|class|extern|operator|switch|virtual|
|const|false|private|template|void|const_cast|float|protected|this|volatile|
|continue|for|public|throw|wchar_t|default|friend|register|true|while|
|delete|goto|reinterpret_cast|


����������������

| 1 | 2 | 3 | 4 | 5 | 6 |
|:-:|:-:|:-:|:-:|:-:|:-:|
|and|bitand|compl|not_eq|or_eq|xor_eq|
|and_eq|bitor|not|or|xor|


������ֻ�������֡���ĸ���»�����ɡ�һ��ΪСд������������»��߷ֿ�����ڶ��������Ժ��ÿ����������ĸ��д��  

��ʼ�����Ǹ�ֵ����ֵ�ǽ�����ǰֵ����ֵ���档ֱ�Ӹ�ֵ(Direct-initialization)��`int ival (1024);` ��class object ��˵, ��copy-initialization Ч�ʸ�����   
�����: ��constructor ��ʼ�����������κι��캯����ʹ��default constructor����Ĭ�Ϲ��캯����������ڳ�ʼ��ʱ���ṩ��ʼֵ����Ȼ�޷���ʼ����  
```
#include <string>
std::string titleA = "Hello World"; 
std::string titleB("Hello World"); 
std::string all_nines(3, '9'); // 999
```

�������ͣ���������ĳ�ʼ���Զ�Ϊ0���������ڲ��Զ���ʼ����
```
#include <iostream>
#include <string>
int global_var; 

int main()
{
    int local_var; 
    std::string local_str; 
    std::cout<< global_var << std::endl; // it is 0. 
    std::cout << local_var << std::endl; // ��
    std::cout << local_str << std::endl; // ""
}
```
