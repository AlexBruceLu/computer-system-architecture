### 用“系统思维”分析问题

    ISO C90标准下，在32位系统上以下C表达式的结果是什么？
```c
-2147483648 < 2147483647
```
***false（与事实不符）！Why?***

    以下关系表达式结果呢？
```c
int i = -2147483648;
i < 2147483647
```
***true！Why?***

   理解以上问题需要知道：编译器如何处理字面量、高级语言中运算规则、高级语言与指令之间的对应、机器指令的执行过程、机器级数据的表示和运算等知识。


```c
sum(int a[ ], unsigned len)
{
int i，sum = 0;
for (i = 0; i <= len–1; i++)
sum += a[i];
return sum;
}
```
以上代码给出一个整形数组，有 **len**个元素，把所有的元素进行累加，所得结果作为返回值。按照预想当参数 **len**为0时，
返回值应该是0，for循环条件是不满足的，因此直接跳出循环，返回值为sum初始值0。但真实结果为出现访问违例的错误提示。

![image](https://raw.githubusercontent.com/wiki/AlexBruceLu/computer-system-architecture/stage1_1.png)
