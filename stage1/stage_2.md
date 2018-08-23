### 用高级语言开发程序

随着技术的发展，出现了许多高级编程语言它们与具体机器结构无关， 面向算法描述，比机器级语言描述能力强得多
高级语言中一条语句对应几条、几十条甚至几百条指令。有“面向过程”和“面向对象”的语言之分。

**处理逻辑分为三种结构： 顺序结构、选择结构、循环结构**
**有两种转换方式：“编译”和“解释”
• 编译程序(Complier)：将高级语言源程序转换为机器级目标程序，执行时只要启动目标程序即可
• 解释程序(Interpreter )：将高级语言语句逐条翻译成机器指令并立即执行，不生成目标文件**

### 一个典型程序的转换处理过程

```c
//hello.c
#include <stdio.h>
int main()
{
printf("hello, world\n");
}
```

计算机是直接不能执行hello.c的，而是先用ASCII文本表示hello.c。

![image](https://raw.githubusercontent.com/wiki/AlexBruceLu/computer-system-architecture/stage1_5.png)

Hello程序的数据流动过程

![image](https://raw.githubusercontent.com/wiki/AlexBruceLu/computer-system-architecture/stage1_6.png)
![image](https://raw.githubusercontent.com/wiki/AlexBruceLu/computer-system-architecture/stage1_7.png)

