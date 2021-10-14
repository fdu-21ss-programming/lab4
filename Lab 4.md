# Lab 4

> 本次lab目标：
>
> 1. 预习if语句
> 2. 预习switch语句
> 3. 预习三元表达式
> 4. 在头歌平台使用编程解决实际问题
> 5. Project发布



## 获取及提交lab

**获取**：通过 `https://github.com/fdu-21ss-programming/lab4`或者`微信群`获取。

**提交**：本次lab附带的练习题将于2021年10月14日15:25发布于头歌平台

**截止时间**：2021年10月17日 23:59:59



## 1. 预习if语句

1. 下面代码中的表达式或者变量b返回的是一个布尔值。从语义上看，表示: 如果b返回true（非0）,那么做事件A ; 如果b返回false（值为0）,那么做事件B

```c
// 注意缩进
if (b) {
	//do A
} else {
	//do B
}
```

1. 判断布尔值b是true还是false时，采用

```c
if (b==0){}
```

或者

```c
if (!b){}
```

的写法都是可以的，但是推荐用第二种

3. 注意if的书写格式，if(b) 后面的代码用 {} 封闭是很好的习惯，注意 if(b) 后面没有分号，如果在if(b)后直接加上分号，编译器会认为，若b为true，执行空语句。

```c
if (b);
```

4. if-else if-else if-....可以不断进行判断

```c
if (a) {
	//do A
} else if (b) {
	//do B
} else if (c) {
	//do C
} else {
	//do D
}
```

## 2. 预习switch语句

一个 **switch** 语句允许测试一个变量等于多个值时的情况。每个值称为一个 case，且被测试的变量会对每个 **switch case** 进行检查。

C 语言中 **switch** 语句的语法：

```c
switch(expression){
    case constant-expression  :
       statement(s);
       break; /* 可选的 */
    case constant-expression  :
       statement(s);
       break; /* 可选的 */
  
    /* 可以有任意数量的 case 语句 */
    default : /* 可选的 */
       statement(s);
}
```

- 当被测试的变量等于 case 中的常量时，case 后跟的语句将被执行，直到遇到 **break** 语句为止。
- 当遇到 **break** 语句时，switch 终止，控制流将跳转到 switch 语句后的下一行。
- 不是每一个 case 都需要包含 **break**。如果 case 语句不包含 **break**，控制流将会**继续**后续的 case，直到遇到 break 为止。
- 一个 **switch** 语句可以有一个可选的 **default** case，出现在 switch 的结尾。default case 可用于在上面所有 case 都不为真时执行一个任务。default case 中的 **break** 语句不是必需的。

## 3. 预习三元表达式

三元表达式实际上是运算符`?:`组成的表达式，示例如下：

```c
b = (a == 1) ? 20 : 30;
```

该表达式可看作一个if-else语句的简写，即

```c
if (a == 1){
    b = 20;
} else{
    b = 30;
}
```

## 4. Project发布

### Project获取及提交

**获取**：本次Project文档通过[本次lab](https://github.com/fdu-21ss-programming/lab4)以及`微信群`获取。

**提交物**：将你的源代码与设计文档进行打包，命名为学号_ 姓名（如20302010000_王明），作为提交物。

**提交**：提交至超星学习通对应的作业中。

**截止时间**：暂定北京时间12月23号23:59，面试时间待定



### Project内容

见[项目需求文档](https://github.com/fdu-21ss-programming/lab4/blob/main/2021%20%E7%A8%8B%E5%BA%8F%E8%AE%BE%E8%AE%A1Project%E6%96%87%E6%A1%A3.md)。



### Project参考

+ [2048游戏网页版](https://2048game.com/)
+ [C语言项目结构](https://stackoverflow.com/questions/2360734/whats-a-good-directory-structure-for-larger-c-projects-using-makefile)

