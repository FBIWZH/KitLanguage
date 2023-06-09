### 基本结构

如同c++，Kit语言在每句话后都要加分号。不同点在于：`for`，`while`，`if-else`这些结构后**都要加分号**。

以下是一个例子：
```cpp
for i=0,i<5,i=i+1
{
	print(i);
};
```
特别的，在`if-else`结构里，分号要加在`else`的**尾部**象征结束。

以下是一个例子：
```cpp
if 1==2
{
	print(114514);
}
else
{
	print(1919810);
};
```
单行注释:`#`

目前还不支持多行注释(悲
### 引用

引用的方法:
```cpp
include <文件名>
或者是
include fromlib <自带库的名称>
```


### 变量&列表

像`python`一样，`kit`语言的变量不需要定义
可以直接用`=`来赋值。

就像这样:
```cpp
a=114514*1919810;
```

列表用`[]`表示，就像这样:
```python
list=[1,1,4,5,1,4];
```

以下是`Kit`语言变量的表达式的运算符：
```cpp
a+b       //返回a加b
a-b       //返回a减b
a*b       //返回a乘b
a/b       //返回a除b
a//b       //返回a整除b
a**b       //返回a的b次方(b可以是小数)
a%b       //返回a模b
a&b			 //返回a与b
a|b			 //返回a或b
a^b			 //返回a异或b
a>b,a<b,a>=b,a<=b,a==b,a!=b //不用我说了吧
```

以下是`Kit`语言列表的表达式的运算符：
```python
a.append(x)     #在a的末尾添加x
a.size()        #返回a的大小
a.len()         #返回a的大小
a.sort()        #将a从小到大排序
a.read(x)       #覆盖a读入x个元素
a.print(x)      #以x为间隔输出a
a.insert(p,x)   #在第p个位置后插入x
a.replace(p,x)  #将a[p]替换为x
```
### 循环结构

**for**使用方式：
```cpp
for <初始表达式>,<终止表达式>,<每循环一次触发事件>
{
	<内容>
};
```


**while**使用方式：
```cpp
while <终止表达式>
{
	<内容>
};
```

### 分支结构

**if**结构：
```
if <条件表达式>
{
	<内容>
};
```


**if-else**结构：
```
if <条件表达式>
{
	<内容>
}
else
{
	<内容>
};
```

注意分号！
### 函数

有两种函数：有返回值和没有返回值的。

有返函数：
```
function <名称>(<参数>)
{
	<内容>
};
```
**用return 返回值！！！**

无返函数：
```
define <名称>(<参数>)
{
	<内容>
};
```
### 自带函数


基本自带函数:
```python
print(...);  #注意，不支持列表
input()	 	 #注意，不支持列表
```

math库函数:
```python
import fromlib math;  #引用
max(x,y)
min(x,y)
lcm(x,y)
gcd(x,y)
abs(x)
fabs(x)
isprime(x)

import fromlib stdlib;  #引用
srand(x)
rand()
```
