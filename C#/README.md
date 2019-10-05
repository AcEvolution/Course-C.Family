# C#

笔者学习 `C#` 参照书籍《Head.First.C#.第3版》[Andrew.Stellman等编写]

![](https://ipic-1259722072.cos.ap-beijing.myqcloud.com/1cynt.jpg)

# 简介

C# 是一个现代的、通用的、面向对象的编程语言，它是由微软（Microsoft）开发的，由 Ecma 和 ISO 核准认可的。

C# 是由 Anders Hejlsberg 和他的团队在 .Net 框架开发期间开发的。

C# 是专为公共语言基础结构（CLI）设计的。CLI 由可执行代码和运行时环境组成，允许在不同的计算机平台和体系结构上使用各种高级语言。

下面列出了 C# 成为一种广泛应用的专业语言的原因：

* 现代的、通用的编程语言。
* 面向对象。
* 面向组件。
* 容易学习。
* 结构化语言。
* 它产生高效率的程序。
* 它可以在多种计算机平台上编译。
* .Net 框架的一部分。

## 教程网站

[C# 教程](https://www.runoob.com/csharp/csharp-tutorial.html)

## C# 有用的资源

* C# Programming Guide - 介绍了有关关键的 C# 语言特征以及如何通过 .NET 框架访问 C# 的详细信息。
* Visual Studio - 下载作为 C# 集成开发环境的 Visual Studio 的最新版本。
* Go Mono - Mono 是一个允许开发人员简单地创建跨平台应用程序的软件平台。
* C Sharp (programming language) - 维基百科解释 C#（编程语言）。

## C# 强大的编程功能

虽然 C# 的构想十分接近于传统高级语言 C 和 C++，是一门面向对象的编程语言，但是它与 Java 非常相似，有许多强大的编程功能，因此得到广大程序员的青睐。

下面列出 C# 一些重要的功能：

* 布尔条件（Boolean Conditions）
* 自动垃圾回收（Automatic Garbage Collection）
* 标准库（Standard Library）
* 组件版本（Assembly Versioning）
* 属性（Properties）和事件（Events）
* 委托（Delegates）和事件管理（Events Management）
* 易于使用的泛型（Generics）
* 索引器（Indexers）
* 条件编译（Conditional Compilation）
* 简单的多线程（Multithreading）
* LINQ 和 Lambda 表达式
* 集成 Windows

## C# 环境

### .Net 框架（.Net Framework）

.Net 框架是一个创新的平台，能帮您编写出下面类型的应用程序：

* Windows 应用程序
* Web 应用程序
* Web 服务

.Net 框架应用程序是多平台的应用程序。框架的设计方式使它适用于下列各种语言：C#、C++、Visual Basic、Jscript、COBOL 等等。所有这些语言可以访问框架，彼此之间也可以互相交互。

.Net 框架由一个巨大的代码库组成，用于 C# 等客户端语言。下面列出一些 .Net 框架的组件：

* 公共语言运行库（Common Language Runtime - CLR）
* .Net 框架类库（.Net Framework Class Library）
* 公共语言规范（Common Language Specification）
* 通用类型系统（Common Type System）
* 元数据（Metadata）和组件（Assemblies）
* Windows 窗体（Windows Forms）
* ASP.Net 和 ASP.Net AJAX
* ADO.Net
* Windows 工作流基础（Windows Workflow Foundation - WF）
* Windows 显示基础（Windows Presentation Foundation）
* Windows 通信基础（Windows Communication Foundation - WCF）
* LINQ

如需了解每个组件的详细信息，请参阅微软（Microsoft）的文档。

### C# 的集成开发环境（Integrated Development Environment - IDE）

微软（Microsoft）提供了下列用于 C# 编程的开发工具：

* Visual Studio 2019

Community版本是免费使用的，可从微软官方网址下载。使用这些工具，您可以编写各种 C# 程序，从简单的命令行应用程序到更复杂的应用程序。您也可以使用基本的文本编辑器（比如 Notepad）编写 C# 源代码文件，并使用命令行编译器（.NET 框架的一部分）编译代码为组件。

您可以从 Microsoft Visual Studio 上进行下载。它会自动安装在您的机器上。请注意，您需要一个可用的网络连接来完成速成版的安装。

### 在 Linux 或 Mac OS 上编写 C# 程序

虽然 .NET 框架是运行在 Windows 操作系统上，但是也有一些运行于其它操作系统上的版本可供选择。

Mono 是 .NET 框架的一个开源版本，它包含了一个 C# 编译器，且可运行于多种操作系统上，比如各种版本的 Linux 和 Mac OS。如需了解更多详情，请访问 Go Mono。

Mono 的目的不仅仅是跨平台地运行微软 .NET 应用程序，而且也为 Linux 开发者提供了更好的开发工具。

Mono 可运行在多种操作系统上，包括 Android、BSD、iOS、Linux、OS X、Windows、Solaris 和 UNIX。

在 Windows、 Linux 和 Mac OS 上可以运行 Rider IDE 来编写 C# 程序

在 Mac OS 上还可以使用 Visual Studio 2019 for macOS 编写 C# 程序

# C# 程序结构

一个 C# 程序主要包括以下部分：

* 命名空间声明（Namespace declaration）
* 一个 class
* Class 方法
* Class 属性
* 一个 Main 方法
* 语句（Statements）& 表达式（Expressions）
* 注释

一个简单的代码示例：
```C#
using System;

namespace LearnCSharp
{
    class Program
    {
        static void Main(string[] args)
        {
            /* 我的第一个 C# 程序*/
            Console.WriteLine("Hello World!");
            Console.ReadKey();
        }
    }
}

```

让我们看一下上面程序的各个部分：

* 程序的第一行 `using System;` - `using` 关键字用于在程序中包含 `System` 命名空间。 一个程序一般有多个 `using` 语句。
* 下一行是 `namespace` 声明。一个 `namespace` 里包含了一系列的类。`LearnCSharp` 命名空间包含了类 `Program`。
* 下一行是 `class` 声明。类 `Program` 包含了程序使用的数据和方法声明。类一般包含多个方法。方法定义了类的行为。在这里，`Program` 类只有一个 `Main` 方法。
* 下一行定义了 `Main` 方法，是所有 `C#` 程序的入口点。`Main` 方法说明当执行时，类将做什么动作。
* 下一行 `/*...*/` 将会被编译器忽略，且它会在程序中添加额外的注释。
* `Main` 方法通过语句 `Console.WriteLine("Hello World");` 指定了它的行为。
* `WriteLine` 是一个定义在 `System` 命名空间中的 `Console` 类的一个方法。该语句会在屏幕上显示消息 "Hello, World!"。
* 最后一行 `Console.ReadKey();` 是针对 VS.NET 用户的。这使得程序会等待一个按键的动作，防止程序从 Visual Studio .NET 启动时屏幕会快速运行并关闭。

以下几点值得注意：

* C# 是大小写敏感的。
* 所有的语句和表达式必须以分号（;）结尾。
* 程序的执行从 Main 方法开始。
* 与 Java 不同的是，文件名可以不同于类的名称。

# C# 基本语法

C# 是一种面向对象的编程语言。在面向对象的程序设计方法中，程序由各种相互交互的对象组成。相同种类的对象通常具有相同的类型，或者说，是在相同的 class 中。

例如，以 Rectangle（矩形）对象为例。它具有 length 和 width 属性。根据设计，它可能需要接受这些属性值、计算面积和显示细节。

让我们来看看一个 Rectangle（矩形）类的实现，并借此讨论 C# 的基本语法：
```C#
using System;
namespace RectangleApplication
{
    class Rectangle
    {
        // 成员变量
        double length;
        double width;
        public void Acceptdetails()
        {
            length = 4.5;
            width = 3.5;
        }
        public double GetArea()
        {
            return length * width;
        }
        public void Display()
        {
            Console.WriteLine("Length: {0}", length);
            Console.WriteLine("Width: {0}", width);
            Console.WriteLine("Area: {0}", GetArea());
        }
    }

    class ExecuteRectangle
    {
        static void Main(string[] args)
        {
            Rectangle r = new Rectangle();
            r.Acceptdetails();
            r.Display();
            Console.ReadLine();
        }
    }
}
```

## using 关键字
在任何 C# 程序中的第一条语句都是：
```C#
using System;
```
`using` 关键字用于在程序中包含命名空间。一个程序可以包含多个 `using` 语句。

## class 关键字
class 关键字用于声明一个类。

## C# 中的注释
注释是用于解释代码。编译器会忽略注释的条目。在 C# 程序中，多行注释以 `/*` 开始，并以字符 `*/` 终止，如下所示：
```
/* This program demonstrates
The basic syntax of C# programming 
Language */
```
单行注释是用 `//` 符号表示。例如：
```
//end class Rectangle    
```

## 成员变量
变量是类的属性或数据成员，用于存储数据。在上面的程序中，Rectangle 类有两个成员变量，名为 length 和 width。

## 成员函数
函数是一系列执行指定任务的语句。类的成员函数是在类内声明的。我们举例的类 Rectangle 包含了三个成员函数： AcceptDetails、GetArea 和 Display。

## 实例化一个类
在上面的程序中，类 ExecuteRectangle 是一个包含 Main() 方法和实例化 Rectangle 类的类。

## 标识符
标识符是用来识别类、变量、函数或任何其它用户定义的项目。在 C# 中，类的命名必须遵循如下基本规则：

* 标识符必须以字母、下划线或 @ 开头，后面可以跟一系列的字母、数字（ 0 - 9 ）、下划线（ _ ）、@。
* 标识符中的第一个字符不能是数字。
* 标识符必须不包含任何嵌入的空格或符号，比如 ? - +! # % ^ & * ( ) [ ] { } . ; : " ' / \。
* 标识符不能是 C# 关键字。除非它们有一个 @ 前缀。 例如，@if 是有效的标识符，但 if 不是，因为 if 是关键字。
* 标识符必须区分大小写。大写字母和小写字母被认为是不同的字母。
* 不能与C#的类库名称相同。

## C# 关键字
关键字是 C# 编译器预定义的保留字。这些关键字不能用作标识符，但是，如果您想使用这些关键字作为标识符，可以在关键字前面加上 @ 字符作为前缀。

在 C# 中，有些关键字在代码的上下文中有特殊的意义，如 get 和 set，这些被称为上下文关键字（contextual keywords）。

下表列出了 C# 中的保留关键字（Reserved Keywords）和上下文关键字（Contextual Keywords）：

**保留关键字**

abstract
as
base
bool
break
byte
case

catch
char
checked
class
const
continue
decimal

default
delegate
do
double
else
enum
event

explicit
extern
false
finally
fixed
float
for

foreach
goto
if
implicit
in
in (generic modifier)
int

interface
internal
is
lock
long
namespace
new

null
object
operator
out
out (generic modifier)
override
params

private
protected
public
readonly
ref
return
sbyte

sealed
short
sizeof
stackalloc
static
string
struct

switch
this
throw
true
try
typeof
uint

ulong
unchecked
unsafe
ushort
using
virtual
void

volatile
while

**上下文关键字**

add
alias
ascending
descending
dynamic
from
get

global
group
into
join
let
orderby
partial (type)

partial (method)
remove
select
set

# C# 数据类型

## 值类型（Value types）

值类型变量可以直接分配给一个值。它们是从类 **System.ValueType** 中派生的。

值类型直接包含数据。比如 **int、char、float**，它们分别存储数字、字符、浮点数。当您声明一个 **int** 类型时，系统分配内存来存储值。

下表列出了 C# 2010 中可用的值类型：

| 类型      | 描述                       | 范围                                                      | 默认值   |
|---------|--------------------------|---------------------------------------------------------|-------|
| bool    | 布尔值                      | True 或 False                                            | False |
| byte    | 8 位无符号整数                 | 0 到 255                                                 | 0     |
| char    | 16 位 Unicode 字符          | U \+0000 到 U \+ffff                                     | '\\0' |
| decimal | 128 位精确的十进制值，28\-29 有效位数 | \(\-7\.9 x 1028 到 7\.9 x 1028\) / 100 到 28              | 0\.0M |
| double  | 64 位双精度浮点型               | \(\+/\-\)5\.0 x 10\-324 到 \(\+/\-\)1\.7 x 10308         | 0\.0D |
| float   | 32 位单精度浮点型               | \-3\.4 x 1038 到 \+ 3\.4 x 1038                          | 0\.0F |
| int     | 32 位有符号整数类型              | \-2,147,483,648 到 2,147,483,647                         | 0     |
| long    | 64 位有符号整数类型              | \-9,223,372,036,854,775,808 到 9,223,372,036,854,775,807 | 0L    |
| sbyte   | 8 位有符号整数类型               | \-128 到 127                                             | 0     |
| short   | 16 位有符号整数类型              | \-32,768 到 32,767                                       | 0     |
| uint    | 32 位无符号整数类型              | 0 到 4,294,967,295                                       | 0     |
| ulong   | 64 位无符号整数类型              | 0 到 18,446,744,073,709,551,615                          | 0     |
| ushort  | 16 位无符号整数类型              | 0 到 65,535                                              | 0     |

如需得到一个类型或一个变量在特定平台上的准确尺寸，可以使用 **sizeof** 方法。表达式 _sizeof(type)_ 产生以字节为单位存储对象或类型的存储尺寸。下面举例获取任何机器上 _int_ 类型的存储尺寸：

```C#
using System;

namespace DataTypeApplication
{
   class Program
   {
      static void Main(string[] args)
      {
         Console.WriteLine("Size of int: {0}", sizeof(int));
         Console.ReadLine();
      }
   }
}
```
  
## 引用类型（Reference types）

引用类型不包含存储在变量中的实际数据，但它们包含对变量的引用。

换句话说，它们指的是一个内存位置。使用多个变量时，引用类型可以指向一个内存位置。如果内存位置的数据是由一个变量改变的，其他变量会自动反映这种值的变化。**内置的** 引用类型有：**object**、**dynamic** 和 **string**。

### 对象（Object）类型

**对象（Object）类型** 是 C# 通用类型系统（Common Type System - CTS）中所有数据类型的终极基类。Object 是 System.Object 类的别名。所以对象（Object）类型可以被分配任何其他类型（值类型、引用类型、预定义类型或用户自定义类型）的值。但是，在分配值之前，需要先进行类型转换。

当一个值类型转换为对象类型时，则被称为 **装箱**；另一方面，当一个对象类型转换为值类型时，则被称为 **拆箱**。
    
```
object obj; 
obj = 100; // 这是装箱
```

### 动态（Dynamic）类型

您可以存储任何类型的值在动态数据类型变量中。这些变量的类型检查是在运行时发生的。

声明动态类型的语法：

```
dynamic <variable_name> = value;
```

例如：

```
dynamic d = 20;
```

动态类型与对象类型相似，但是对象类型变量的类型检查是在编译时发生的，而动态类型变量的类型检查是在运行时发生的。

### 字符串（String）类型

**字符串（String）类型** 允许您给变量分配任何字符串值。字符串（String）类型是 System.String 类的别名。它是从对象（Object）类型派生的。字符串（String）类型的值可以通过两种形式进行分配：引号和 @引号。

例如：
 
```
String str = "runoob.com";
```

一个 @引号字符串：

```
@"runoob.com";
```

C# string 字符串的前面可以加 @（称作"逐字字符串"）将转义字符（\）当作普通字符对待，比如：

```
string str = @"C:\Windows";
```

等价于：

```
string str = "C:\Windows";
```

@ 字符串中可以任意换行，换行符及缩进空格都计算在字符串长度之内。

```
string str = @"<script type=""text/javascript"">
    <!--
    -->
</script>";
```

用户自定义引用类型有：class、interface 或 delegate。我们将在以后的章节中讨论这些类型。

## 指针类型（Pointer types）

指针类型变量存储另一种类型的内存地址。C# 中的指针与 C 或 C++ 中的指针有相同的功能。

声明指针类型的语法：

```
type* identifier;
```

例如：

```
char* cptr; int* iptr;
```

我们将在章节"不安全的代码"中讨论指针类型。

# C# 类型转换

类型转换从根本上说是类型铸造，或者说是把数据从一种类型转换为另一种类型。在 C# 中，类型铸造有两种形式：

  * **隐式类型转换** - 这些转换是 C# 默认的以安全方式进行的转换, 不会导致数据丢失。例如，从小的整数类型转换为大的整数类型，从派生类转换为基类。
  * **显式类型转换** - 显式类型转换，即强制类型转换。显式转换需要强制转换运算符，而且强制转换会造成数据丢失。

下面的实例显示了一个显式的类型转换：
```C#
namespace TypeConversionApplication
{
    class ExplicitConversion
    {
        static void Main(string[] args)
        {
            double d = 5673.74;
            int i;

            // 强制转换 double 为 int
            i = (int)d;
            Console.WriteLine(i);
            Console.ReadKey();
            
        }
    }
}
```

## C# 类型转换方法

C# 提供了下列内置的类型转换方法：

| 序号 | 方法          | 描述                            |
|----|-------------|-------------------------------|
| 1  | ToBoolean   | 如果可能的话，把类型转换为布尔型。             |
| 2  | ToByte      | 把类型转换为字节类型。                   |
| 3  | ToChar      | 如果可能的话，把类型转换为单个 Unicode 字符类型。 |
| 4  | ToDateTime  | 把类型（整数或字符串类型）转换为 日期\-时间 结构。   |
| 5  | ToDecimal   | 把浮点型或整数类型转换为十进制类型。            |
| 6  | ToDouble    | 把类型转换为双精度浮点型。                 |
| 7  | ToInt16     | 把类型转换为 16 位整数类型。              |
| 8  | ToInt32     | 把类型转换为 32 位整数类型。              |
| 9  | ToInt64     | 把类型转换为 64 位整数类型。              |
| 10 | ToSbyte     | 把类型转换为有符号字节类型。                |
| 11 | ToSingle    | 把类型转换为小浮点数类型。                 |
| 12 | ToString    | 把类型转换为字符串类型。                  |
| 13 | ToType      | 把类型转换为指定类型。                   |
| 14 | ToUInt16    | 把类型转换为 16 位无符号整数类型。           |
| 15 | ToUInt32    | 把类型转换为 32 位无符号整数类型。           |
| 16 | ToUInt64    | 把类型转换为 64 位无符号整数类型。           |

下面的实例把不同值的类型转换为字符串类型：

```C#
namespace TypeConversionApplication
{
    class StringConversion
    {
        static void Main(string[] args)
        {
            int i = 75;
            float f = 53.005f;
            double d = 2345.7652;
            bool b = true;

            Console.WriteLine(i.ToString());
            Console.WriteLine(f.ToString());
            Console.WriteLine(d.ToString());
            Console.WriteLine(b.ToString());
            Console.ReadKey();
            
        }
    }
}
```

# C# 变量

一个变量只不过是一个供程序操作的存储区的名字。在 C# 中，每个变量都有一个特定的类型，类型决定了变量的内存大小和布局。范围内的值可以存储在内存中，可以对变量进行一系列操作。

我们已经讨论了各种数据类型。C# 中提供的基本的值类型大致可以分为以下几类：

| 类型    | 举例                                                 |
|-------|----------------------------------------------------|
| 整数类型  | sbyte、byte、short、ushort、int、uint、long、ulong 和 char |
| 浮点型   | float 和 double                                     |
| 十进制类型 | decimal                                            |
| 布尔类型  | true 或 false 值，指定的值                                |
| 空类型   | 可为空值的数据类型                                          |

C# 允许定义其他值类型的变量，比如 **enum**，也允许定义引用类型变量，比如 **class**。这些我们将在以后的章节中进行讨论。在本章节中，我们只研究基本变量类型。

## C# 中的变量定义

C# 中变量定义的语法：

```
<data_type> <variable_list>;
```

在这里，data_type 必须是一个有效的 C# 数据类型，可以是 char、int、float、double 或其他用户自定义的数据类型。variable_list 可以由一个或多个用逗号分隔的标识符名称组成。

一些有效的变量定义如下所示：

```
int i, j, k; 
char c, ch; 
float f, salary; 
double d;
```

您可以在变量定义时进行初始化：

```
int i = 100;
```

## C# 中的变量初始化

变量通过在等号后跟一个常量表达式进行初始化（赋值）。初始化的一般形式为：

```
variable_name = value;
```

变量可以在声明时被初始化（指定一个初始值）。初始化由一个等号后跟一个常量表达式组成，如下所示：

```
<data_type> <variable_name> = value;
```

一些实例：

```
int d = 3, f = 5; /* 初始化 d 和 f. */ 
byte z = 22; /* 初始化 z. */ 
double pi = 3.14159; /* 声明 pi 的近似值 */ 
char x = 'x'; /* 变量 x 的值为 'x' */
```

正确地初始化变量是一个良好的编程习惯，否则有时程序会产生意想不到的结果。

请看下面的实例，使用了各种类型的变量：

```C#
namespace VariableDefinition  
{  
    class Program  
    {  
        static void Main(string[] args)  
        {  
            short a;  
            int b ;  
            double c;  
  
            /* 实际初始化 */  
            a = 10;  
            b = 20;  
            c = a + b;  
            Console.WriteLine("a = {0}, b = {1}, c = {2}", a, b, c);  
            Console.ReadLine();  
        }  
    }  
}  
```


## 接受来自用户的值

**System** 命名空间中的 **Console** 类提供了一个函数 **ReadLine()**，用于接收来自用户的输入，并把它存储到一个变量中。

例如：

```
int num; 
num = Convert.ToInt32(Console.ReadLine());
```

函数 **Convert.ToInt32()** 把用户输入的数据转换为 int 数据类型，因为 **Console.ReadLine()** 只接受字符串格式的数据。

## C# 中的 Lvalues 和 Rvalues

C# 中的两种表达式：

  1. **lvalue**：lvalue 表达式可以出现在赋值语句的左边或右边。
  2. **rvalue**：rvalue 表达式可以出现在赋值语句的右边，不能出现在赋值语句的左边。

变量是 lvalue 的，所以可以出现在赋值语句的左边。数值是 rvalue 的，因此不能被赋值，不能出现在赋值语句的左边。下面是一个有效的语句：

```
int g = 20;
```

下面是一个无效的语句，会产生编译时错误：

```
10 = 20;
```

# C# 常量

常量是固定值，程序执行期间不会改变。常量可以是任何基本数据类型，比如整数常量、浮点常量、字符常量或者字符串常量，还有枚举常量。

常量可以被当作常规的变量，只是它们的值在定义后不能被修改。

## 整数常量

整数常量可以是十进制、八进制或十六进制的常量。前缀指定基数：0x 或 0X 表示十六进制，没有前缀则表示十进制。

整数常量也可以有后缀，可以是 U 和 L 的组合，其中，U 和 L 分别表示 unsigned 和 long。后缀可以是大写或者小写，多个后缀以任意顺序进行组合。

这里有一些整数常量的实例：

```
212 /* 合法 */ 
215u /* 合法 */ 
0xFeeL /* 合法 */ 
032UU /* 非法：不能重复后缀 */
```

以下是各种类型的整数常量的实例：

```
85 /* 十进制 */ 
0x4b /* 十六进制 */ 
30 /* int */ 
30u /* 无符号 int */ 
30l /* long */ 
30ul /* 无符号 long */
```

## 浮点常量

一个浮点常量是由整数部分、小数点、小数部分和指数部分组成。您可以使用小数形式或者指数形式来表示浮点常量。

这里有一些浮点常量的实例：

```
3.14159 /* 合法 */ 
314159E-5L /* 合法 */ 
510E /* 非法：不完全指数 */ 
210f /* 非法：没有小数或指数 */ 
.e55 /* 非法：缺少整数或小数 */
```

使用小数形式表示时，必须包含小数点、指数或同时包含两者。使用指数形式表示时，必须包含整数部分、小数部分或同时包含两者。有符号的指数是用 e 或 E 表示的。

## 字符常量

字符常量是括在单引号里，例如，'x'，且可存储在一个简单的字符类型变量中。一个字符常量可以是一个普通字符（例如 'x'）、一个转义序列（例如 '\t'）或者一个通用字符（例如 '\u02C0'）。

在 C# 中有一些特定的字符，当它们的前面带有反斜杠时有特殊的意义，可用于表示换行符（\n）或制表符 tab（\t）。在这里，列出一些转义序列码：

| 转义序列           | 含义             |
|----------------|----------------|
| \\\\           | \\ 字符          |
| \\'            | ' 字符           |
| \\"            | " 字符           |
| \\?            | ? 字符           |
| \\a            | Alert 或 bell   |
| \\b            | 退格键（Backspace） |
| \\f            | 换页符（Form feed） |
| \\n            | 换行符（Newline）   |
| \\r            | 回车             |
| \\t            | 水平制表符 tab      |
| \\v            | 垂直制表符 tab      |
| \\ooo          | 一到三位的八进制数      |
| \\xhh \. \. \. | 一个或多个数字的十六进制数  |

以下是一些转义序列字符的实例：

```C#
namespace EscapeChar
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello\tWorld\n\n");
            Console.ReadLine();
        }
    }
}
```

## 字符串常量

字符串常量是括在双引号 "" 里，或者是括在 @"" 里。字符串常量包含的字符与字符常量相似，可以是：普通字符、转义序列和通用字符
使用字符串常量时，可以把一个很长的行拆成多个行，可以使用空格分隔各个部分。
这里是一些字符串常量的实例。下面所列的各种形式表示相同的字符串。

```
string a = "hello, world";                  // hello, world
string b = @"hello, world";               // hello, world
string c = "hello \t world";               // hello     world
string d = @"hello \t world";               // hello \t world
string e = "Joe said \"Hello\" to me";      // Joe said "Hello" to me
string f = @"Joe said ""Hello"" to me";   // Joe said "Hello" to me
string g = "\\\\server\\share\\file.txt";   // \\server\share\file.txt
string h = @"\\server\share\file.txt";      // \\server\share\file.txt
string i = "one\r\ntwo\r\nthree";
string j = @"one
two
three";
```

## 定义常量

常量是使用 const 关键字来定义的 。定义一个常量的语法如下：

```
const <data_type> <constant_name> = value;
```

下面的代码演示了如何在程序中定义和使用常量：

```C#
using System;

public class ConstTest 
{
    class SampleClass
    {
        public int x;
        public int y;
        public const int c1 = 5;
        public const int c2 = c1 + 5;

        public SampleClass(int p1, int p2) 
        {
            x = p1; 
            y = p2;
        }
    }

    static void Main()
    {
        SampleClass mC = new SampleClass(11, 22);
        Console.WriteLine("x = {0}, y = {1}", mC.x, mC.y);
        Console.WriteLine("c1 = {0}, c2 = {1}", 
                          SampleClass.c1, SampleClass.c2);
    }
}
```

# C# 运算符

## 算术运算符

下表显示了 C# 支持的所有算术运算符。假设变量 **A** 的值为 10，变量 **B** 的值为 20，则：

| 运算符  | 描述               | 实例              |
|------|------------------|-----------------|
| \+   | 把两个操作数相加         | A \+ B 将得到 30   |
| \-   | 从第一个操作数中减去第二个操作数 | A \- B 将得到 \-10 |
| \*   | 把两个操作数相乘         | A \* B 将得到 200  |
| /    | 分子除以分母           | B / A 将得到 2     |
| %    | 取模运算符，整除后的余数     | B % A 将得到 0     |
| \+\+ | 自增运算符，整数值增加 1    | A\+\+ 将得到 11    |
| \-\- | 自减运算符，整数值减少 1    | A\-\- 将得到 9     |

请看下面的实例，了解 C# 中所有可用的算术运算符：

```C#
using System;

namespace OperatorsAppl
{
    class Program
    {
        static void Main(string[] args)
        {
            int a = 21;
            int b = 10;
            int c;

            c = a + b;
            Console.WriteLine("Line 1 - c 的值是 {0}", c);
            c = a - b;
            Console.WriteLine("Line 2 - c 的值是 {0}", c);
            c = a * b;
            Console.WriteLine("Line 3 - c 的值是 {0}", c);
            c = a / b;
            Console.WriteLine("Line 4 - c 的值是 {0}", c);
            c = a % b;
            Console.WriteLine("Line 5 - c 的值是 {0}", c);

            // ++a 先进行自增运算再赋值
            c = ++a;
            Console.WriteLine("Line 6 - c 的值是 {0}", c);

            // 此时 a 的值为 22
            // --a 先进行自减运算再赋值
            c = --a;
            Console.WriteLine("Line 7 - c 的值是 {0}", c);
            Console.ReadLine();
        }
    }
}
```

```C#
using System;

namespace OperatorsAppl
{
    class Program
    {
        static void Main(string[] args)
        {
            int a = 1;
            int b;

            // a++ 先赋值再进行自增运算
            b = a++;
            Console.WriteLine("a = {0}", a);
            Console.WriteLine("b = {0}", b);
            Console.ReadLine();

            // ++a 先进行自增运算再赋值
            a = 1; // 重新初始化 a
            b = ++a;
            Console.WriteLine("a = {0}", a);
            Console.WriteLine("b = {0}", b);
            Console.ReadLine();

            // a-- 先赋值再进行自减运算
            a = 1;  // 重新初始化 a
            b= a--;
            Console.WriteLine("a = {0}", a);
            Console.WriteLine("b = {0}", b);
            Console.ReadLine();

            // --a 先进行自减运算再赋值
            a = 1;  // 重新初始化 a
            b= --a;
            Console.WriteLine("a = {0}", a);
            Console.WriteLine("b = {0}", b);
            Console.ReadLine();
        }
    }
}
```

## 关系运算符

下表显示了 C# 支持的所有关系运算符。假设变量 **A** 的值为 10，变量 **B** 的值为 20，则：

| 运算符 | 描述                              | 实例              |
|-----|---------------------------------|-----------------|
| ==  | 检查两个操作数的值是否相等，如果相等则条件为真。        | \(A == B\) 不为真。 |
| \!= | 检查两个操作数的值是否相等，如果不相等则条件为真。       | \(A \!= B\) 为真。 |
| >   | 检查左操作数的值是否大于右操作数的值，如果是则条件为真。    | \(A > B\) 不为真。  |
| <   | 检查左操作数的值是否小于右操作数的值，如果是则条件为真。    | \(A < B\) 为真。   |
| >=  | 检查左操作数的值是否大于或等于右操作数的值，如果是则条件为真。 | \(A >= B\) 不为真。 |
| <=  | 检查左操作数的值是否小于或等于右操作数的值，如果是则条件为真。 | \(A <= B\) 为真。  |

请看下面的实例，了解 C# 中所有可用的关系运算符：

```C#
using System;

class Program
{
  static void Main(string[] args)
  {
      int a = 21;
      int b = 10;
      
      if (a == b)
      {
          Console.WriteLine("Line 1 - a 等于 b");
      }
      else
      {
          Console.WriteLine("Line 1 - a 不等于 b");
      }
      if (a < b)
      {
          Console.WriteLine("Line 2 - a 小于 b");
      }
      else
      {
          Console.WriteLine("Line 2 - a 不小于 b");
      }
      if (a > b)
      {
          Console.WriteLine("Line 3 - a 大于 b");
      }
      else
      {
          Console.WriteLine("Line 3 - a 不大于 b");
      }
      /* 改变 a 和 b 的值 */
      a = 5;
      b = 20;
      if (a <= b)
      {
         Console.WriteLine("Line 4 - a 小于或等于 b");
      }
      if (b >= a)
      {
         Console.WriteLine("Line 5 - b 大于或等于 a");
      }
  }
}
```

## 逻辑运算符

下表显示了 C# 支持的所有逻辑运算符。假设变量 **A** 为布尔值 true，变量 **B** 为布尔值 false，则：

| 运算符  | 描述                                        | 实例               |
|------|-------------------------------------------|------------------|
| &&   | 称为逻辑与运算符。如果两个操作数都非零，则条件为真。                | \(A && B\) 为假。   |
| \|\| | 称为逻辑或运算符。如果两个操作数中有任意一个非零，则条件为真。           | \(A \|\| B\) 为真。 |
| \!   | 称为逻辑非运算符。用来逆转操作数的逻辑状态。如果条件为真则逻辑非运算符将使其为假。 | \!\(A && B\) 为真。 |

```C#
using System;

namespace OperatorsAppl
{
    class Program
    {
        static void Main(string[] args)
        {
            bool a = true;
            bool b = true;
           
            if (a && b)
            {
               Console.WriteLine("Line 1 - 条件为真");
            }
            if (a || b)
            {
                Console.WriteLine("Line 2 - 条件为真");
            }
            /* 改变 a 和 b 的值 */
            a = false;
            b = true;
            if (a && b)
            {
                Console.WriteLine("Line 3 - 条件为真");
            }
            else
            {
                Console.WriteLine("Line 3 - 条件不为真");
            }
            if (!(a && b))
            {
                Console.WriteLine("Line 4 - 条件为真");
            }
            Console.ReadLine();
        }
    }
}
```

## 位运算符

位运算符作用于位，并逐位执行操作。&、 | 和 ^ 的真值表如下所示：

| p | q | p & q | p \| q | p ^ q |
|---|---|-------|--------|-------|
| 0 | 0 | 0     | 0      | 0     |
| 0 | 1 | 0     | 1      | 1     |
| 1 | 1 | 1     | 1      | 0     |
| 1 | 0 | 0     | 1      | 1     |

假设如果 A = 60，且 B = 13，现在以二进制格式表示，它们如下所示：
A = 0011 1100
B = 0000 1101
-----------------
A&B = 0000 1100
A|B = 0011 1101
A^B = 0011 0001
~A  = 1100 0011
下表列出了 C# 支持的位运算符。假设变量 A 的值为 60，变量 B 的值为 13，则：

| 运算符 | 描述                                           | 实例                                            |
|-----|----------------------------------------------|-----------------------------------------------|
| &   | 如果同时存在于两个操作数中，二进制 AND 运算符复制一位到结果中。           | \(A & B\) 将得到 12，即为 0000 1100                 |
| \|  | 如果存在于任一操作数中，二进制 OR 运算符复制一位到结果中。              | \(A \| B\) 将得到 61，即为 0011 1101                |
| ^   | 如果存在于其中一个操作数中但不同时存在于两个操作数中，二进制异或运算符复制一位到结果中。 | \(A ^ B\) 将得到 49，即为 0011 0001                 |
| ~   | 按位取反运算符是一元运算符，具有"翻转"位效果，即0变成1，1变成0，包括符号位。    | \(~A \) 将得到 \-61，即为 1100 0011，一个有符号二进制数的补码形式。 |
| <<  | 二进制左移运算符。左操作数的值向左移动右操作数指定的位数。                | A << 2 将得到 240，即为 1111 0000                   |
| >>  | 二进制右移运算符。左操作数的值向右移动右操作数指定的位数。                | A >> 2 将得到 15，即为 0000 1111                    |

请看下面的实例，了解 C# 中所有可用的位运算符：

```C#
using System;
namespace OperatorsAppl
{
    class Program
    {
        static void Main(string[] args)
        {
            int a = 60;            /* 60 = 0011 1100 */  
            int b = 13;            /* 13 = 0000 1101 */
            int c = 0;           

             c = a & b;           /* 12 = 0000 1100 */ 
             Console.WriteLine("Line 1 - c 的值是 {0}", c );

             c = a | b;           /* 61 = 0011 1101 */
             Console.WriteLine("Line 2 - c 的值是 {0}", c);

             c = a ^ b;           /* 49 = 0011 0001 */
             Console.WriteLine("Line 3 - c 的值是 {0}", c);

             c = ~a;               /*-61 = 1100 0011 */
             Console.WriteLine("Line 4 - c 的值是 {0}", c);

             c = a << 2;     /* 240 = 1111 0000 */
             Console.WriteLine("Line 5 - c 的值是 {0}", c);

             c = a >> 2;     /* 15 = 0000 1111 */
             Console.WriteLine("Line 6 - c 的值是 {0}", c);
            Console.ReadLine();
        }
    }
}
```

## 赋值运算符

下表列出了 C# 支持的赋值运算符：

| 运算符 | 描述                               | 实例                          |
|-----|----------------------------------|-----------------------------|
| =   | 简单的赋值运算符，把右边操作数的值赋给左边操作数         | C = A \+ B 将把 A \+ B 的值赋给 C |
| \+= | 加且赋值运算符，把右边操作数加上左边操作数的结果赋值给左边操作数 | C \+= A 相当于 C = C \+ A      |
| \-= | 减且赋值运算符，把左边操作数减去右边操作数的结果赋值给左边操作数 | C \-= A 相当于 C = C \- A      |
| \*= | 乘且赋值运算符，把右边操作数乘以左边操作数的结果赋值给左边操作数 | C \*= A 相当于 C = C \* A      |
| /=  | 除且赋值运算符，把左边操作数除以右边操作数的结果赋值给左边操作数 | C /= A 相当于 C = C / A        |
| %=  | 求模且赋值运算符，求两个操作数的模赋值给左边操作数        | C %= A 相当于 C = C % A        |
| <<= | 左移且赋值运算符                         | C <<= 2 等同于 C = C << 2      |
| >>= | 右移且赋值运算符                         | C >>= 2 等同于 C = C >> 2      |
| &=  | 按位与且赋值运算符                        | C &= 2 等同于 C = C & 2        |
| ^=  | 按位异或且赋值运算符                       | C ^= 2 等同于 C = C ^ 2        |
| \|= | 按位或且赋值运算符                        | C \|= 2 等同于 C = C \| 2      |

请看下面的实例，了解 C# 中所有可用的赋值运算符：

```C#
using System;

namespace OperatorsAppl
{
    class Program
    {
        static void Main(string[] args)
        {
            int a = 21;
            int c;

            c = a;
            Console.WriteLine("Line 1 - =  c 的值 = {0}", c);

            c += a;
            Console.WriteLine("Line 2 - += c 的值 = {0}", c);

            c -= a;
            Console.WriteLine("Line 3 - -=  c 的值 = {0}", c);

            c *= a;
            Console.WriteLine("Line 4 - *=  c 的值 = {0}", c);

            c /= a;
            Console.WriteLine("Line 5 - /=  c 的值 = {0}", c);

            c = 200;
            c %= a;
            Console.WriteLine("Line 6 - %=  c 的值 = {0}", c);

            c <<= 2;
            Console.WriteLine("Line 7 - <<=  c 的值 = {0}", c);

            c >>= 2;
            Console.WriteLine("Line 8 - >>=  c 的值 = {0}", c);

            c &= 2;
            Console.WriteLine("Line 9 - &=  c 的值 = {0}", c);

            c ^= 2;
            Console.WriteLine("Line 10 - ^=  c 的值 = {0}", c);

            c |= 2;
            Console.WriteLine("Line 11 - |=  c 的值 = {0}", c);
            Console.ReadLine();
        }
    }
}
```

## 其他运算符

下表列出了 C# 支持的其他一些重要的运算符，包括 **sizeof**、**typeof** 和 **? :**。

| 运算符        | 描述                  | 实例                                                                             |
|------------|---------------------|--------------------------------------------------------------------------------|
| sizeof\(\) | 返回数据类型的大小。          | sizeof\(int\)，将返回 4\.                                                          |
| typeof\(\) | 返回 class 的类型。       | typeof\(StreamReader\);                                                        |
| &          | 返回变量的地址。            | &a; 将得到变量的实际地址。                                                                |
| \*         | 变量的指针。              | \*a; 将指向一个变量。                                                                  |
| ? :        | 条件表达式               | 如果条件为真 ? 则为 X : 否则为 Y                                                          |
| is         | 判断对象是否为某一类型。        | If\( Ford is Car\) // 检查 Ford 是否是 Car 类的一个对象。                                  |
| as         | 强制转换，即使转换失败也不会抛出异常。 | Object obj = new StringReader\("Hello"\);StringReader r = obj as StringReader; |

```C#
using System;

namespace OperatorsAppl
{
    
   class Program
   {
      static void Main(string[] args)
      {
         
         /* sizeof 运算符的实例 */
         Console.WriteLine("int 的大小是 {0}", sizeof(int));
         Console.WriteLine("short 的大小是 {0}", sizeof(short));
         Console.WriteLine("double 的大小是 {0}", sizeof(double));
         
         /* 三元运算符的实例 */
         int a, b;
         a = 10;
         b = (a == 1) ? 20 : 30;
         Console.WriteLine("b 的值是 {0}", b);

         b = (a == 10) ? 20 : 30;
         Console.WriteLine("b 的值是 {0}", b);
         Console.ReadLine();
      }
   }
}
```

## C# 中的运算符优先级

运算符的优先级确定表达式中项的组合。这会影响到一个表达式如何计算。某些运算符比其他运算符有更高的优先级，例如，乘除运算符具有比加减运算符更高的优先级。
例如 x = 7 + 3 * 2，在这里，x 被赋值为 13，而不是 20，因为运算符 * 具有比 + 更高的优先级，所以首先计算乘法 3 \*2，然后再加上 7。
下表将按运算符优先级从高到低列出各个运算符，具有较高优先级的运算符出现在表格的上面，具有较低优先级的运算符出现在表格的下面。在表达式中，较高优先级的运算符会优先被计算。

| 类别       | 运算符                                        | 结合性   |
|----------|--------------------------------------------|-------|
| 后缀       | \(\) \[\] \-> \. \+\+ \- \-                | 从左到右  |
| 一元       | \+ \- \! ~ \+\+ \- \- \(type\)\* & sizeof  | 从右到左  |
| 乘除       | \* / %                                     | 从左到右  |
| 加减       | \+ \-                                      | 从左到右  |
| 移位       | << >>                                      | 从左到右  |
| 关系       | < <= > >=                                  | 从左到右  |
| 相等       | == \!=                                     | 从左到右  |
| 位与 AND   | &                                          | 从左到右  |
| 位异或 XOR  | ^                                          | 从左到右  |
| 位或 OR    | \|                                         | 从左到右  |
| 逻辑与 AND  | &&                                         | 从左到右  |
| 逻辑或 OR   | \|\|                                       | 从左到右  |
| 条件       | ?:                                         | 从右到左  |
| 赋值       | = \+= \-= \*= /= %=>>= <<= &= ^= \|=       | 从右到左  |
| 逗号       | ,                                          | 从左到右  |

```C#
using System;

namespace OperatorsAppl
{
    
   class Program
   {
      static void Main(string[] args)
      {
         int a = 20;
         int b = 10;
         int c = 15;
         int d = 5;
         int e;
         e = (a + b) * c / d;     // ( 30 * 15 ) / 5
         Console.WriteLine("(a + b) * c / d 的值是 {0}", e);

         e = ((a + b) * c) / d;   // (30 * 15 ) / 5
         Console.WriteLine("((a + b) * c) / d 的值是 {0}", e);

         e = (a + b) * (c / d);   // (30) * (15/5)
         Console.WriteLine("(a + b) * (c / d) 的值是 {0}", e);

         e = a + (b * c) / d;    //  20 + (150/5)
         Console.WriteLine("a + (b * c) / d 的值是 {0}", e);
         Console.ReadLine();
      }
   }
}
```

# C# 判断

判断结构要求程序员指定一个或多个要评估或测试的条件，以及条件为真时要执行的语句（必需的）和条件为假时要执行的语句（可选的）。

下面是大多数编程语言中典型的判断结构的一般形式：
![](https://ipic-1259722072.cos.ap-beijing.myqcloud.com/rva0i.jpg)

## 判断语句

C# 提供了以下类型的判断语句。点击链接查看每个语句的细节。

| 语句              | 描述                                            |
|-----------------|-----------------------------------------------|
| if 语句           | 一个 if 语句 由一个布尔表达式后跟一个或多个语句组成。                 |
| if\.\.\.else 语句 | 一个 if 语句 后可跟一个可选的 else 语句，else 语句在布尔表达式为假时执行。 |
| 嵌套 if 语句        | 您可以在一个 if 或 else if 语句内使用另一个 if 或 else if 语句。 |
| switch 语句       | 一个 switch 语句允许测试一个变量等于多个值时的情况。                |
| 嵌套 switch 语句    | 您可以在一个 switch 语句内使用另一个 switch 语句。             |


## ? : 运算符

我们已经在前面的章节中讲解了 **条件运算符 ? :**，可以用来替代 **if...else** 语句。它的一般形式如下：

```
Exp1 ? Exp2 : Exp3;
```

其中，Exp1、Exp2 和 Exp3 是表达式。请注意，冒号的使用和位置。

? 表达式的值是由 Exp1 决定的。如果 Exp1 为真，则计算 Exp2 的值，结果即为整个 ? 表达式的值。如果 Exp1 为假，则计算 Exp3 的值，结果即为整个 ? 表达式的值。

# C# 循环

有的时候，可能需要多次执行同一块代码。一般情况下，语句是顺序执行的：函数中的第一个语句先执行，接着是第二个语句，依此类推。

编程语言提供了允许更为复杂的执行路径的多种控制结构。

循环语句允许我们多次执行一个语句或语句组，下面是大多数编程语言中循环语句的一般形式：
![](https://ipic-1259722072.cos.ap-beijing.myqcloud.com/q2j8u.jpg)

## 循环类型

C# 提供了以下几种循环类型。点击链接查看每个类型的细节。

| 循环类型             | 描述                                         |
|------------------|--------------------------------------------|
| while 循环         | 当给定条件为真时，重复语句或语句组。它会在执行循环主体之前测试条件。         |
| for/foreach 循环   | 多次执行一个语句序列，简化管理循环变量的代码。                    |
| do\.\.\.while 循环 | 除了它是在循环主体结尾测试条件外，其他与 while 语句类似。           |
| 嵌套循环             | 您可以在 while、for 或 do\.\.while 循环内使用一个或多个循环。 |

## 循环控制语句

循环控制语句更改执行的正常序列。当执行离开一个范围时，所有在该范围中创建的自动对象都会被销毁。

C# 提供了下列的控制语句。点击链接查看每个语句的细节。

| 控制语句        | 描述                                                    |
|-------------|-------------------------------------------------------|
| break 语句    | 终止 loop 或 switch 语句，程序流将继续执行紧接着 loop 或 switch 的下一条语句。 |
| continue 语句 | 引起循环跳过主体的剩余部分，立即重新开始测试条件。                             |

## 无限循环

如果条件永远不为假，则循环将变成无限循环。**for** 循环在传统意义上可用于实现无限循环。由于构成循环的三个表达式中任何一个都不是必需的，您可以将某些条件表达式留空来构成一个无限循环。

```C#
using System;

namespace Loops
{
    
    class Program
    {
        static void Main(string[] args)
        {
            for (; ; )
            {
                Console.WriteLine("Hey! I am Trapped");
            }
 
        }
    }
} 
```

当条件表达式不存在时，它被假设为真。您也可以设置一个初始值和增量表达式，但是一般情况下，程序员偏向于使用 for(;;) 结构来表示一个无限循环。

# C# 封装

**封装** 被定义为"把一个或多个项目封闭在一个物理的或者逻辑的包中"。在面向对象程序设计方法论中，封装是为了防止对实现细节的访问。

抽象和封装是面向对象程序设计的相关特性。抽象允许相关信息可视化，封装则使开发者_实现所需级别的抽象_。

C# 封装根据具体的需要，设置使用者的访问权限，并通过 **访问修饰符** 来实现。

一个 **访问修饰符** 定义了一个类成员的范围和可见性。C# 支持的访问修饰符如下所示：

  * public：所有对象都可以访问；
  * private：对象本身在对象内部可以访问；
  * protected：只有该类对象及其子类对象可以访问
  * internal：同一个程序集的对象可以访问；
  * protected internal：访问限于当前程序集或派生自包含类的类型。

## Public 访问修饰符

Public 访问修饰符允许一个类将其成员变量和成员函数暴露给其他的函数和对象。任何公有成员可以被外部的类访问。

下面的实例说明了这点：

```C#
using System;

namespace RectangleApplication
{
    class Rectangle
    {
        //成员变量
        public double length;
        public double width;

        public double GetArea()
        {
            return length * width;
        }
        public void Display()
        {
            Console.WriteLine("长度： {0}", length);
            Console.WriteLine("宽度： {0}", width);
            Console.WriteLine("面积： {0}", GetArea());
        }
    }// Rectangle 结束

    class ExecuteRectangle
    {
        static void Main(string[] args)
        {
            Rectangle r = new Rectangle();
            r.length = 4.5;
            r.width = 3.5;
            r.Display();
            Console.ReadLine();
        }
    }
}
```

在上面的实例中，成员变量 length 和 width 被声明为 **public**，所以它们可以被函数 Main() 使用 Rectangle 类的实例 **r** 访问。

成员函数 _Display()_ 和 _GetArea()_ 可以直接访问这些变量。

成员函数 _Display()_ 也被声明为 **public**，所以它也能被 _Main()_ 使用 Rectangle 类的实例 **r** 访问。

## Private 访问修饰符

Private 访问修饰符允许一个类将其成员变量和成员函数对其他的函数和对象进行隐藏。只有同一个类中的函数可以访问它的私有成员。即使是类的实例也不能访问它的私有成员。

下面的实例说明了这点：

```C#
using System;

namespace RectangleApplication
{
    class Rectangle
    {
        //成员变量
        private double length;
        private double width;

        public void Acceptdetails()
        {
            Console.WriteLine("请输入长度：");
            length = Convert.ToDouble(Console.ReadLine());
            Console.WriteLine("请输入宽度：");
            width = Convert.ToDouble(Console.ReadLine());
        }
        public double GetArea()
        {
            return length * width;
        }
        public void Display()
        {
            Console.WriteLine("长度： {0}", length);
            Console.WriteLine("宽度： {0}", width);
            Console.WriteLine("面积： {0}", GetArea());
        }
    }//end class Rectangle    
    class ExecuteRectangle
    {
        static void Main(string[] args)
        {
            Rectangle r = new Rectangle();
            r.Acceptdetails();
            r.Display();
            Console.ReadLine();
        }
    }
}
```

在上面的实例中，成员变量 length 和 width 被声明为 **private**，所以它们不能被函数 Main() 访问。

成员函数 _AcceptDetails()_ 和 _Display()_ 可以访问这些变量。

由于成员函数 _AcceptDetails()_ 和 _Display()_ 被声明为 **public**，所以它们可以被 _Main()_ 使用 Rectangle 类的实例 **r** 访问。

## Protected 访问修饰符

Protected 访问修饰符允许子类访问它的基类的成员变量和成员函数。这样有助于实现继承。我们将在继承的章节详细讨论这个。更详细地讨论这个。

## Internal 访问修饰符

Internal 访问说明符允许一个类将其成员变量和成员函数暴露给当前程序中的其他函数和对象。换句话说，带有 internal 访问修饰符的任何成员可以被定义在该成员所定义的应用程序内的任何类或方法访问。

下面的实例说明了这点：

```C#
using System;

namespace RectangleApplication
{
    class Rectangle
    {
        //成员变量
        internal double length;
        internal double width;
        
        double GetArea()
        {
            return length * width;
        }
       public void Display()
        {
            Console.WriteLine("长度： {0}", length);
            Console.WriteLine("宽度： {0}", width);
            Console.WriteLine("面积： {0}", GetArea());
        }
    }//end class Rectangle    
    class ExecuteRectangle
    {
        static void Main(string[] args)
        {
            Rectangle r = new Rectangle();
            r.length = 4.5;
            r.width = 3.5;
            r.Display();
            Console.ReadLine();
        }
    }
}
```

在上面的实例中，请注意成员函数 _GetArea()_ 声明的时候不带有任何访问修饰符。如果没有指定访问修饰符，则使用类成员的默认访问修饰符，即为 **private**。

## Protected Internal 访问修饰符

Protected Internal 访问修饰符允许在本类,派生类或者包含该类的程序集中访问。这也被用于实现继承。

# C# 方法

一个方法是把一些相关的语句组织在一起，用来执行一个任务的语句块。每一个 C# 程序至少有一个带有 Main 方法的类。

要使用一个方法，您需要：

  * 定义方法
  * 调用方法

## C# 中定义方法

当定义一个方法时，从根本上说是在声明它的结构的元素。在 C# 中，定义方法的语法如下：

```
<Access Specifier> <Return Type> <Method Name>(Parameter List) 
{ 
    Method Body 
}
```

下面是方法的各个元素：

  * **Access Specifier**：访问修饰符，这个决定了变量或方法对于另一个类的可见性。
  * **Return type**：返回类型，一个方法可以返回一个值。返回类型是方法返回的值的数据类型。如果方法不返回任何值，则返回类型为 **void**。
  * **Method name**：方法名称，是一个唯一的标识符，且是大小写敏感的。它不能与类中声明的其他标识符相同。
  * **Parameter list**：参数列表，使用圆括号括起来，该参数是用来传递和接收方法的数据。参数列表是指方法的参数类型、顺序和数量。参数是可选的，也就是说，一个方法可能不包含参数。
  * **Method body**：方法主体，包含了完成任务所需的指令集。

## 实例

下面的代码片段显示一个函数 _FindMax_ ，它接受两个整数值，并返回两个中的较大值。它有 public 访问修饰符，所以它可以使用类的实例从类的外部进行访问。

```C#
class NumberManipulator
{
   public int FindMax(int num1, int num2)
   {
      /* 局部变量声明 */
      int result;

      if (num1 > num2)
         result = num1;
      else
         result = num2;

      return result;
   }
   ...
}
```

## C# 中调用方法

您可以使用方法名调用方法。下面的实例演示了这点：

```C#
using System;

namespace CalculatorApplication
{
   class NumberManipulator
   {
      public int FindMax(int num1, int num2)
      {
         /* 局部变量声明 */
         int result;

         if (num1 > num2)
            result = num1;
         else
            result = num2;

         return result;
      }
      static void Main(string[] args)
      {
         /* 局部变量定义 */
         int a = 100;
         int b = 200;
         int ret;
         NumberManipulator n = new NumberManipulator();

         //调用 FindMax 方法
         ret = n.FindMax(a, b);
         Console.WriteLine("最大值是： {0}", ret );
         Console.ReadLine();
      }
   }
}
```

您也可以使用类的实例从另一个类中调用其他类的公有方法。例如，方法 FindMax 属于 NumberManipulator 类，您可以从另一个类 Test 中调用它。

```C#
using System;

namespace CalculatorApplication
{
    class NumberManipulator
    {
        public int FindMax(int num1, int num2)
        {
            /* 局部变量声明 */
            int result;

            if (num1 > num2)
                result = num1;
            else
                result = num2;

            return result;
        }
    }
    class Test
    {
        static void Main(string[] args)
        {
            /* 局部变量定义 */
            int a = 100;
            int b = 200;
            int ret;
            NumberManipulator n = new NumberManipulator();
            //调用 FindMax 方法
            ret = n.FindMax(a, b);
            Console.WriteLine("最大值是： {0}", ret );
            Console.ReadLine();

        }
    }
}
```

## 递归方法调用

一个方法可以自我调用。这就是所谓的 **递归**。下面的实例使用递归函数计算一个数的阶乘：

```C#
using System;

namespace CalculatorApplication
{
    class NumberManipulator
    {
        public int factorial(int num)
        {
            /* 局部变量定义 */
            int result;

            if (num == 1)
            {
                return 1;
            }
            else
            {
                result = factorial(num - 1) * num;
                return result;
            }
        }
    
        static void Main(string[] args)
        {
            NumberManipulator n = new NumberManipulator();
            //调用 factorial 方法
            Console.WriteLine("6 的阶乘是： {0}", n.factorial(6));
            Console.WriteLine("7 的阶乘是： {0}", n.factorial(7));
            Console.WriteLine("8 的阶乘是： {0}", n.factorial(8));
            Console.ReadLine();

        }
    }
}
```

## 参数传递

当调用带有参数的方法时，您需要向方法传递参数。在 C# 中，有三种向方法传递参数的方式：

| 方式   | 描述                                                                               |
|------|----------------------------------------------------------------------------------|
| 值参数  | 这种方式复制参数的实际值给函数的形式参数，实参和形参使用的是两个不同内存中的值。在这种情况下，当形参的值发生改变时，不会影响实参的值，从而保证了实参数据的安全。 |
| 引用参数 | 这种方式复制参数的内存位置的引用给形式参数。这意味着，当形参的值发生改变时，同时也改变实参的值。                                 |
| 输出参数 | 这种方式可以返回多个值。                                                                     |


## 按值传递参数

这是参数传递的默认方式。在这种方式下，当调用一个方法时，会为每个值参数创建一个新的存储位置。

实际参数的值会复制给形参，实参和形参使用的是两个不同内存中的值。所以，当形参的值发生改变时，不会影响实参的值，从而保证了实参数据的安全。下面的实例演示了这个概念：

```C#
using System;
namespace CalculatorApplication
{
   class NumberManipulator
   {
      public void swap(int x, int y)
      {
         int temp;
         
         temp = x; /* 保存 x 的值 */
         x = y;    /* 把 y 赋值给 x */
         y = temp; /* 把 temp 赋值给 y */
      }
      
      static void Main(string[] args)
      {
         NumberManipulator n = new NumberManipulator();
         /* 局部变量定义 */
         int a = 100;
         int b = 200;
         
         Console.WriteLine("在交换之前，a 的值： {0}", a);
         Console.WriteLine("在交换之前，b 的值： {0}", b);
         
         /* 调用函数来交换值 */
         n.swap(a, b);
         
         Console.WriteLine("在交换之后，a 的值： {0}", a);
         Console.WriteLine("在交换之后，b 的值： {0}", b);
         
         Console.ReadLine();
      }
   }
}
```

结果表明，即使在函数内改变了值，值也没有发生任何的变化。

## 按引用传递参数

引用参数是一个对变量的**内存位置的引用**。当按引用传递参数时，与值参数不同的是，它不会为这些参数创建一个新的存储位置。引用参数表示与提供给方法的实际参数具有相同的内存位置。

在 C# 中，使用 **ref** 关键字声明引用参数。下面的实例演示了这点：

```C#
using System;
namespace CalculatorApplication
{
   class NumberManipulator
   {
      public void swap(ref int x, ref int y)
      {
         int temp;

         temp = x; /* 保存 x 的值 */
         x = y;    /* 把 y 赋值给 x */
         y = temp; /* 把 temp 赋值给 y */
       }
   
      static void Main(string[] args)
      {
         NumberManipulator n = new NumberManipulator();
         /* 局部变量定义 */
         int a = 100;
         int b = 200;

         Console.WriteLine("在交换之前，a 的值： {0}", a);
         Console.WriteLine("在交换之前，b 的值： {0}", b);

         /* 调用函数来交换值 */
         n.swap(ref a, ref b);

         Console.WriteLine("在交换之后，a 的值： {0}", a);
         Console.WriteLine("在交换之后，b 的值： {0}", b);
 
         Console.ReadLine();

      }
   }
}
```

结果表明，_swap_ 函数内的值改变了，且这个改变可以在 _Main_ 函数中反映出来。

## 按输出传递参数

return 语句可用于只从函数中返回一个值。但是，可以使用 **输出参数** 来从函数中返回两个值。输出参数会把方法输出的数据赋给自己，其他方面与引用参数相似。

下面的实例演示了这点：

```C#
using System;

namespace CalculatorApplication
{
   class NumberManipulator
   {
      public void getValue(out int x )
      {
         int temp = 5;
         x = temp;
      }
   
      static void Main(string[] args)
      {
         NumberManipulator n = new NumberManipulator();
         /* 局部变量定义 */
         int a = 100;
         
         Console.WriteLine("在方法调用之前，a 的值： {0}", a);
         
         /* 调用函数来获取值 */
         n.getValue(out a);

         Console.WriteLine("在方法调用之后，a 的值： {0}", a);
         Console.ReadLine();

      }
   }
}
```

提供给输出参数的变量不需要赋值。当需要从一个参数没有指定初始值的方法中返回值时，输出参数特别有用。请看下面的实例，来理解这一点：

```C#
using System;

namespace CalculatorApplication
{
   class NumberManipulator
   {
      public void getValues(out int x, out int y )
      {
          Console.WriteLine("请输入第一个值： ");
          x = Convert.ToInt32(Console.ReadLine());
          Console.WriteLine("请输入第二个值： ");
          y = Convert.ToInt32(Console.ReadLine());
      }
   
      static void Main(string[] args)
      {
         NumberManipulator n = new NumberManipulator();
         /* 局部变量定义 */
         int a , b;
         
         /* 调用函数来获取值 */
         n.getValues(out a, out b);

         Console.WriteLine("在方法调用之后，a 的值： {0}", a);
         Console.WriteLine("在方法调用之后，b 的值： {0}", b);
         Console.ReadLine();
      }
   }
}
```

# C# 可空类型（Nullable）

## C# 单问号 ? 与 双问号 ?? 

? : 单问号用于对 int,double,bool 等无法直接赋值为 null 的数据类型进行 null 的赋值，意思是这个数据类型是 NullAble 类型的。
    
    int? i = 3 等同于 Nullable<int> i = new Nullable<int>(3); int i; //默认值0 int? ii; //默认值null

?? : 双问号 可用于判断一个变量在为 null 时返回一个指定的值。

接下来我们详细说明。

## C# 可空类型（Nullable）

C# 提供了一个特殊的数据类型，**nullable** 类型（可空类型），可空类型可以表示其基础值类型正常范围内的值，再加上一个 null 值。

例如，Nullable< Int32 >，读作"可空的 Int32"，可以被赋值为 -2,147,483,648 到 2,147,483,647 之间的任意值，也可以被赋值为 null 值。类似的，Nullable< bool > 变量可以被赋值为 true 或 false 或 null。

在处理数据库和其他包含可能未赋值的元素的数据类型时，将 null 赋值给数值类型或布尔型的功能特别有用。例如，数据库中的布尔型字段可以存储值 true 或 false，或者，该字段也可以未定义。

声明一个 **nullable** 类型（可空类型）的语法如下：

```
< data_type> ? <variable_name> = null;
```

下面的实例演示了可空数据类型的用法：

```C#
using System;
namespace CalculatorApplication
{
   class NullablesAtShow
   {
      static void Main(string[] args)
      {
         int? num1 = null;
         int? num2 = 45;
         double? num3 = new double?();
         double? num4 = 3.14157;
         
         bool? boolval = new bool?();

         // 显示值
         
         Console.WriteLine("显示可空类型的值： {0}, {1}, {2}, {3}", 
                            num1, num2, num3, num4);
         Console.WriteLine("一个可空的布尔值： {0}", boolval);
         Console.ReadLine();

      }
   }
}
```

## Null 合并运算符（ ?? ）

Null 合并运算符用于定义可空类型和引用类型的默认值。Null 合并运算符为类型转换定义了一个预设值，以防可空类型的值为 Null。Null 合并运算符把操作数类型隐式转换为另一个可空（或不可空）的值类型的操作数的类型。

如果第一个操作数的值为 null，则运算符返回第二个操作数的值，否则返回第一个操作数的值。下面的实例演示了这点：

```C#
using System;
namespace CalculatorApplication
{
   class NullablesAtShow
   {
         
      static void Main(string[] args)
      {
         
         double? num1 = null;
         double? num2 = 3.14157;
         double num3;
         num3 = num1 ?? 5.34;      // num1 如果为空值则返回 5.34
         Console.WriteLine("num3 的值： {0}", num3);
         num3 = num2 ?? 5.34;
         Console.WriteLine("num3 的值： {0}", num3);
         Console.ReadLine();

      }
   }
}
```

# C# 数组（Array）

数组是一个存储相同类型元素的固定大小的顺序集合。数组是用来存储数据的集合，通常认为数组是一个同一类型变量的集合。

声明数组变量并不是声明 number0、number1、...、number99 一个个单独的变量，而是声明一个就像 numbers 这样的变量，然后使用 numbers[0]、numbers[1]、...、numbers[99] 来表示一个个单独的变量。数组中某个指定的元素是通过索引来访问的。

所有的数组都是由连续的内存位置组成的。最低的地址对应第一个元素，最高的地址对应最后一个元素。

## 声明数组

在 C# 中声明一个数组，您可以使用下面的语法：

```
datatype[] arrayName;
```

其中，

* datatype 用于指定被存储在数组中的元素的类型。
* [ ] 指定数组的秩（维度）。秩指定数组的大小。
* arrayName 指定数组的名称。

例如：

```
double[] balance;
```

## 初始化数组

声明一个数组不会在内存中初始化数组。当初始化数组变量时，您可以赋值给数组。

数组是一个引用类型，所以您需要使用 **new** 关键字来创建数组的实例。

例如：

```
double[] balance = new double[10];
```

## 赋值给数组

您可以通过使用索引号赋值给一个单独的数组元素，比如：

```
double[] balance = new double[10]; balance[0] = 4500.0;
```

您可以在声明数组的同时给数组赋值，比如：

```
double[] balance = { 2340.0, 4523.69, 3421.0};
```

您也可以创建并初始化一个数组，比如：

```
int [] marks = new int[5] { 99, 98, 92, 97, 95};
```

在上述情况下，你也可以省略数组的大小，比如：

```
int [] marks = new int[] { 99, 98, 92, 97, 95};
```

您也可以赋值一个数组变量到另一个目标数组变量中。在这种情况下，目标和源会指向相同的内存位置：

```
int [] marks = new int[] { 99, 98, 92, 97, 95}; int[] score = marks;
```

当您创建一个数组时，C# 编译器会根据数组类型隐式初始化每个数组元素为一个默认值。例如，int 数组的所有元素都会被初始化为 0。

## 访问数组元素

元素是通过带索引的数组名称来访问的。这是通过把元素的索引放置在数组名称后的方括号中来实现的。例如：
    
    double salary = balance[9];

下面是一个实例，使用上面提到的三个概念，即声明、赋值、访问数组：

```C#
using System;
namespace ArrayApplication
{
   class MyArray
   {
      static void Main(string[] args)
      {
         int []  n = new int[10]; /* n 是一个带有 10 个整数的数组 */
         int i,j;


         /* 初始化数组 n 中的元素 */         
         for ( i = 0; i < 10; i++ )
         {
            n[ i ] = i + 100;
         }

         /* 输出每个数组元素的值 */
         for (j = 0; j < 10; j++ )
         {
            Console.WriteLine("Element[{0}] = {1}", j, n[j]);
         }
         Console.ReadKey();
      }
   }
}
```

## 使用 _foreach_ 循环

在前面的实例中，我们使用一个 for 循环来访问每个数组元素。您也可以使用一个 **foreach** 语句来遍历数组。

```C#
using System;

namespace ArrayApplication
{
   class MyArray
   {
      static void Main(string[] args)
      {
         int []  n = new int[10]; /* n 是一个带有 10 个整数的数组 */


         /* 初始化数组 n 中的元素 */         
         for ( int i = 0; i < 10; i++ )
         {
            n[i] = i + 100;
         }

         /* 输出每个数组元素的值 */
         foreach (int j in n )
         {
            int i = j-100;
            Console.WriteLine("Element[{0}] = {1}", i, j);
         }
         Console.ReadKey();
      }
   }
}
```

## C# 数组细节

在 C# 中，数组是非常重要的，且需要了解更多的细节。下面列出了 C# 程序员必须清楚的一些与数组相关的重要概念：

### C# 多维数组

C# 支持多维数组。多维数组又称为矩形数组。
您可以声明一个 string 变量的二维数组，如下：

```
string [,] names;
```

或者，您可以声明一个 int 变量的三维数组，如下：

```
int [ , , ] m;
```

#### 二维数组

多维数组最简单的形式是二维数组。一个二维数组，在本质上，是一个一维数组的列表。

一个二维数组可以被认为是一个带有 x 行和 y 列的表格。

因此，数组中的每个元素是使用形式为 a[ i , j ] 的元素名称来标识的，其中 a 是数组名称，i 和 j 是唯一标识 a 中每个元素的下标。

#### 初始化二维数组

多维数组可以通过在括号内为每行指定值来进行初始化。下面是一个带有 3 行 4 列的数组。

```
int [,] a = new int [3,4] { 
{0, 1, 2, 3} , /* 初始化索引号为 0 的行 */ 
{4, 5, 6, 7} , /* 初始化索引号为 1 的行 */ 
{8, 9, 10, 11} /* 初始化索引号为 2 的行 */ 
};
```

#### 访问二维数组元素

二维数组中的元素是通过使用下标（即数组的行索引和列索引）来访问的。例如：

```
int val = a[2,3];
```

上面的语句将获取数组中第 3 行第 4 个元素。您可以通过上面的示意图来进行验证。让我们来看看下面的程序，我们将使用嵌套循环来处理二维数组：

```C#
using System;

namespace ArrayApplication
{
    class MyArray
    {
        static void Main(string[] args)
        {
            /* 一个带有 5 行 2 列的数组 */
            int[,] a = new int[5, 2] {{0,0}, {1,2}, {2,4}, {3,6}, {4,8} };

            int i, j;

            /* 输出数组中每个元素的值 */
            for (i = 0; i < 5; i++)
            {
                for (j = 0; j < 2; j++)
                {
                    Console.WriteLine("a[{0},{1}] = {2}", i, j, a[i,j]);
                }
            }
           Console.ReadKey();
        }
    }
}
```

### C# 交错数组

交错数组是数组的数组。

交错数组是一维数组。

您可以声明一个带有 **int** 值的交错数组 _scores_，如下所示：

```
int [][] scores;
```

声明一个数组不会在内存中创建数组。创建上面的数组：

```
int[][] scores = new int[5][]; 
for (int i = 0; i < scores.Length; i++) 
{ 
    scores[i] = new int[4]; 
}
```

您可以初始化一个交错数组，如下所示：

```
int[][] scores = new int[2][]{new int[]{92,93,94},new int[]{85,66,87,88}};
```

其中，scores 是一个由两个整型数组组成的数组 -- scores[0] 是一个带有 3 个整数的数组，scores[1] 是一个带有 4 个整数的数组。

#### 实例

下面的实例演示了如何使用交错数组：
```C#
using System;

namespace ArrayApplication
{
    class MyArray
    {
        static void Main(string[] args)
        {
            /* 一个由 5 个整型数组组成的交错数组 */
            int[][] a = new int[][]{new int[]{0,0},new int[]{1,2}, 
            new int[]{2,4},new int[]{ 3, 6 }, new int[]{ 4, 8 } }; 

            int i, j;

            /* 输出数组中每个元素的值 */
            for (i = 0; i < 5; i++)
            {
                for (j = 0; j < 2; j++)
                {
                    Console.WriteLine("a[{0}][{1}] = {2}", i, j, a[i][j]);
                }
            }
           Console.ReadKey();
        }
    }
}
```

### C# 传递数组给函数

在 C# 中，您可以传递数组作为函数的参数。您可以通过指定不带索引的数组名称来给函数传递一个指向数组的指针。

#### 实例

下面的实例演示了如何传递数组给函数：

```C#
using System;

namespace ArrayApplication
{
   class MyArray
   {
      double getAverage(int[] arr, int size)
      {
         int i;
         double avg;
         int sum = 0;

         for (i = 0; i < size; ++i)
         {
            sum += arr[i];
         }

         avg = (double)sum / size;
         return avg;
      }
      static void Main(string[] args)
      {
         MyArray app = new MyArray();
         /* 一个带有 5 个元素的 int 数组 */
         int [] balance = new int[]{1000, 2, 3, 17, 50};
         double avg;

         /* 传递数组的指针作为参数 */
         avg = app.getAverage(balance, 5 ) ;

         /* 输出返回值 */
         Console.WriteLine( "平均值是： {0} ", avg );
         Console.ReadKey();
      }
   }
}
```

### C# 参数数组

有时，当声明一个方法时，您不能确定要传递给函数作为参数的参数数目。C# 参数数组解决了这个问题，参数数组通常用于传递未知数量的参数给函数。

#### params 关键字

在使用数组作为形参时，C# 提供了 params 关键字，使调用数组为形参的方法时，既可以传递数组实参，也可以传递一组数组元素。params 的使用格式为：

```
public 返回类型 方法名称( params 类型名称[] 数组名称 )
```

#### 实例

下面的实例演示了如何使用参数数组：

```C#
using System;

namespace ArrayApplication
{
   class ParamArray
   {
      public int AddElements(params int[] arr)
      {
         int sum = 0;
         foreach (int i in arr)
         {
            sum += i;
         }
         return sum;
      }
   }
      
   class TestClass
   {
      static void Main(string[] args)
      {
         ParamArray app = new ParamArray();
         int sum = app.AddElements(512, 720, 250, 567, 889);
         Console.WriteLine("总和是： {0}", sum);
         Console.ReadKey();
      }
   }
}
```

### C# Array 类

Array 类是 C# 中所有数组的基类，它是在 System 命名空间中定义。Array 类提供了各种用于数组的属性和方法。

#### Array 类的属性

下表列出了 Array 类中一些最常用的属性：

| 序号 | 属性 & 描述                                  |
|----|------------------------------------------|
| 1  | IsFixedSize获取一个值，该值指示数组是否带有固定大小。         |
| 2  | IsReadOnly获取一个值，该值指示数组是否只读。              |
| 3  | Length获取一个 32 位整数，该值表示所有维度的数组中的元素总数。     |
| 4  | LongLength获取一个 64 位整数，该值表示所有维度的数组中的元素总数。 |
| 5  | Rank获取数组的秩（维度）。                          |

如需了解 Array 类的完整的属性列表，请参阅微软的 C# 文档。

#### Array 类的方法

下表列出了 Array 类中一些最常用的方法：

| 序号 | 方法 & 描述                                                                       |
|----|-------------------------------------------------------------------------------|
| 1  | Clear根据元素的类型，设置数组中某个范围的元素为零、为 false 或者为 null。                                 |
| 2  | Copy\(Array, Array, Int32\)从数组的第一个元素开始复制某个范围的元素到另一个数组的第一个元素位置。长度由一个 32 位整数指定。 |
| 3  | CopyTo\(Array, Int32\)从当前的一维数组中复制所有的元素到一个指定的一维数组的指定索引位置。索引由一个 32 位整数指定。       |
| 4  | GetLength 获取一个 32 位整数，该值表示指定维度的数组中的元素总数。                                      |
| 5  | GetLongLength获取一个 64 位整数，该值表示指定维度的数组中的元素总数。                                   |
| 6  | GetLowerBound获取数组中指定维度的下界。                                                    |
| 7  | GetType获取当前实例的类型。从对象（Object）继承。                                               |
| 8  | GetUpperBound获取数组中指定维度的上界。                                                    |
| 9  | GetValue\(Int32\)获取一维数组中指定位置的值。索引由一个 32 位整数指定。                                |
| 10 | IndexOf\(Array, Object\)搜索指定的对象，返回整个一维数组中第一次出现的索引。                            |
| 11 | Reverse\(Array\)逆转整个一维数组中元素的顺序。                                               |
| 12 | SetValue\(Object, Int32\)给一维数组中指定位置的元素设置值。索引由一个 32 位整数指定。                     |
| 13 | Sort\(Array\)使用数组的每个元素的 IComparable 实现来排序整个一维数组中的元素。                          |
| 14 | ToString返回一个表示当前对象的字符串。从对象（Object）继承。                                         |

如需了解 Array 类的完整的方法列表，请参阅微软的 C# 文档。

#### 实例

下面的程序演示了 Array 类的一些方法的用法：

```C#
using System;
namespace ArrayApplication
{
    class MyArray
    {
        
        static void Main(string[] args)
        {
            int[] list = { 34, 72, 13, 44, 25, 30, 10 };

            Console.Write("原始数组： ");
            foreach (int i in list)
            {
                Console.Write(i + " ");
            }
            Console.WriteLine();
           
            // 逆转数组
            Array.Reverse(list);
            Console.Write("逆转数组： ");
            foreach (int i in list)
            {
                Console.Write(i + " ");
            }
            Console.WriteLine();
            
            // 排序数组
            Array.Sort(list);
            Console.Write("排序数组： ");
            foreach (int i in list)
            {
                Console.Write(i + " ");
            }
            Console.WriteLine();

           Console.ReadKey();
        }
    }
}
```

# C# 字符串（String）

在 C# 中，您可以使用字符数组来表示字符串，但是，更常见的做法是使用 **string** 关键字来声明一个字符串变量。string 关键字是 **System.String** 类的别名。

## 创建 String 对象

您可以使用以下方法之一来创建 string 对象：

  * 通过给 String 变量指定一个字符串
  * 通过使用 String 类构造函数
  * 通过使用字符串串联运算符（ + ）
  * 通过检索属性或调用一个返回字符串的方法
  * 通过格式化方法来转换一个值或对象为它的字符串表示形式

下面的实例演示了这点：

```C#
using System;

namespace StringApplication
{
    class Program
    {
        static void Main(string[] args)
        {
           //字符串，字符串连接
            string fname, lname;
            fname = "Rowan";
            lname = "Atkinson";

            string fullname = fname + lname;
            Console.WriteLine("Full Name: {0}", fullname);

            //通过使用 string 构造函数
            char[] letters = { 'H', 'e', 'l', 'l','o' };
            string greetings = new string(letters);
            Console.WriteLine("Greetings: {0}", greetings);

            //方法返回字符串
            string[] sarray = { "Hello", "From", "Tutorials", "Point" };
            string message = String.Join(" ", sarray);
            Console.WriteLine("Message: {0}", message);

            //用于转化值的格式化方法
            DateTime waiting = new DateTime(2012, 10, 10, 17, 58, 1);
            string chat = String.Format("Message sent at {0:t} on {0:D}", 
            waiting);
            Console.WriteLine("Message: {0}", chat);
            Console.ReadKey() ;
        }
    }
}
```

## String 类的属性

String 类有以下两个属性：

| 序号 | 属性名称 & 描述                           |
|----|-------------------------------------|
| 1  | Chars在当前 String 对象中获取 Char 对象的指定位置。 |
| 2  | Length在当前的 String 对象中获取字符数。         |

## String 类的方法

String 类有许多方法用于 string 对象的操作。下面的表格提供了一些最常用的方法：

| 序号 | 方法名称 & 描述                                                                                                                                          |
|----|----------------------------------------------------------------------------------------------------------------------------------------------------|
| 1  | public static int Compare\( string strA, string strB \) 比较两个指定的 string 对象，并返回一个表示它们在排列顺序中相对位置的整数。该方法区分大小写。                                         |
| 2  | public static int Compare\( string strA, string strB, bool ignoreCase \) 比较两个指定的 string 对象，并返回一个表示它们在排列顺序中相对位置的整数。但是，如果布尔参数为真时，该方法不区分大小写。          |
| 3  | public static string Concat\( string str0, string str1 \) 连接两个 string 对象。                                                                          |
| 4  | public static string Concat\( string str0, string str1, string str2 \) 连接三个 string 对象。                                                             |
| 5  | public static string Concat\( string str0, string str1, string str2, string str3 \) 连接四个 string 对象。                                                |
| 6  | public bool Contains\( string value \) 返回一个表示指定 string 对象是否出现在字符串中的值。                                                                              |
| 7  | public static string Copy\( string str \) 创建一个与指定字符串具有相同值的新的 String 对象。                                                                            |
| 8  | public void CopyTo\( int sourceIndex, char\[\] destination, int destinationIndex, int count \) 从 string 对象的指定位置开始复制指定数量的字符到 Unicode 字符数组中的指定位置。    |
| 9  | public bool EndsWith\( string value \) 判断 string 对象的结尾是否匹配指定的字符串。                                                                                  |
| 10 | public bool Equals\( string value \) 判断当前的 string 对象是否与指定的 string 对象具有相同的值。                                                                        |
| 11 | public static bool Equals\( string a, string b \) 判断两个指定的 string 对象是否具有相同的值。                                                                       |
| 12 | public static string Format\( string format, Object arg0 \) 把指定字符串中一个或多个格式项替换为指定对象的字符串表示形式。                                                        |
| 13 | public int IndexOf\( char value \) 返回指定 Unicode 字符在当前字符串中第一次出现的索引，索引从 0 开始。                                                                        |
| 14 | public int IndexOf\( string value \) 返回指定字符串在该实例中第一次出现的索引，索引从 0 开始。                                                                                |
| 15 | public int IndexOf\( char value, int startIndex \) 返回指定 Unicode 字符从该字符串中指定字符位置开始搜索第一次出现的索引，索引从 0 开始。                                               |
| 16 | public int IndexOf\( string value, int startIndex \) 返回指定字符串从该实例中指定字符位置开始搜索第一次出现的索引，索引从 0 开始。                                                      |
| 17 | public int IndexOfAny\( char\[\] anyOf \) 返回某一个指定的 Unicode 字符数组中任意字符在该实例中第一次出现的索引，索引从 0 开始。                                                        |
| 18 | public int IndexOfAny\( char\[\] anyOf, int startIndex \) 返回某一个指定的 Unicode 字符数组中任意字符从该实例中指定字符位置开始搜索第一次出现的索引，索引从 0 开始。                              |
| 19 | public string Insert\( int startIndex, string value \) 返回一个新的字符串，其中，指定的字符串被插入在当前 string 对象的指定索引位置。                                                 |
| 20 | public static bool IsNullOrEmpty\( string value \) 指示指定的字符串是否为 null 或者是否为一个空的字符串。                                                                  |
| 21 | public static string Join\( string separator, string\[\] value \) 连接一个字符串数组中的所有元素，使用指定的分隔符分隔每个元素。                                                  |
| 22 | public static string Join\( string separator, string\[\] value, int startIndex, int count \) 连接接一个字符串数组中的指定位置开始的指定元素，使用指定的分隔符分隔每个元素。               |
| 23 | public int LastIndexOf\( char value \) 返回指定 Unicode 字符在当前 string 对象中最后一次出现的索引位置，索引从 0 开始。                                                          |
| 24 | public int LastIndexOf\( string value \) 返回指定字符串在当前 string 对象中最后一次出现的索引位置，索引从 0 开始。                                                                |
| 25 | public string Remove\( int startIndex \) 移除当前实例中的所有字符，从指定位置开始，一直到最后一个位置为止，并返回字符串。                                                                  |
| 26 | public string Remove\( int startIndex, int count \) 从当前字符串的指定位置开始移除指定数量的字符，并返回字符串。                                                                 |
| 27 | public string Replace\( char oldChar, char newChar \) 把当前 string 对象中，所有指定的 Unicode 字符替换为另一个指定的 Unicode 字符，并返回新的字符串。                                |
| 28 | public string Replace\( string oldValue, string newValue \) 把当前 string 对象中，所有指定的字符串替换为另一个指定的字符串，并返回新的字符串。                                          |
| 29 | public string\[\] Split\( params char\[\] separator \) 返回一个字符串数组，包含当前的 string 对象中的子字符串，子字符串是使用指定的 Unicode 字符数组中的元素进行分隔的。                           |
| 30 | public string\[\] Split\( char\[\] separator, int count \) 返回一个字符串数组，包含当前的 string 对象中的子字符串，子字符串是使用指定的 Unicode 字符数组中的元素进行分隔的。int 参数指定要返回的子字符串的最大数目。 |
| 31 | public bool StartsWith\( string value \) 判断字符串实例的开头是否匹配指定的字符串。                                                                                     |
| 32 | public char\[\] ToCharArray\(\)返回一个带有当前 string 对象中所有字符的 Unicode 字符数组。                                                                              |
| 33 | public char\[\] ToCharArray\( int startIndex, int length \) 返回一个带有当前 string 对象中所有字符的 Unicode 字符数组，从指定的索引开始，直到指定的长度为止。                              |
| 34 | public string ToLower\(\)把字符串转换为小写并返回。                                                                                                             |
| 35 | public string ToUpper\(\)把字符串转换为大写并返回。                                                                                                             |
| 36 | public string Trim\(\)移除当前 String 对象中的所有前导空白字符和后置空白字符。                                                                                             |

上面的方法列表并不详尽，请访问 MSDN 库，查看完整的方法列表和 String 类构造函数。

## 实例

下面的实例演示了上面提到的一些方法：

**比较字符串**

```C#
using System;

namespace StringApplication
{
   class StringProg
   {
      static void Main(string[] args)
      {
         string str1 = "This is test";
         string str2 = "This is text";

         if (String.Compare(str1, str2) == 0)
         {
            Console.WriteLine(str1 + " and " + str2 +  " are equal.");
         }
         else
         {
            Console.WriteLine(str1 + " and " + str2 + " are not equal.");
         }
         Console.ReadKey() ;
      }
   }
}
```

**字符串包含字符串：**

```C#
using System;

namespace StringApplication
{
   class StringProg
   {
      static void Main(string[] args)
      {
         string str = "This is test";
         if (str.Contains("test"))
         {
            Console.WriteLine("The sequence 'test' was found.");
         }
         Console.ReadKey() ;
      }
   }
}
```

**获取子字符串：**

```C#
using System; 
namespace StringApplication 
{
        class StringProg 
        { 
                static void Main(string[] args) 
                { 
                        string str = "Last night I dreamt of San Pedro"; 
                        Console.WriteLine(str); 
                        string substr = str.Substring(23); 
                        Console.WriteLine(substr); 
                        Console.ReadKey() ; 
                } 
        } 
}
```

**连接字符串：**

```C#
using System;

namespace StringApplication
{
   class StringProg
   {
      static void Main(string[] args)
      {
         string[] starray = new string[]{"Down the way nights are dark",
         "And the sun shines daily on the mountain top",
         "I took a trip on a sailing ship",
         "And when I reached Jamaica",
         "I made a stop"};

         string str = String.Join("\n", starray);
         Console.WriteLine(str);
         Console.ReadKey() ;
      }
   }
}
```

# C# 结构体（Struct）

在 C# 中，结构体是值类型数据结构。它使得一个单一变量可以存储各种数据类型的相关数据。**struct** 关键字用于创建结构体。

结构体是用来代表一个记录。假设您想跟踪图书馆中书的动态。您可能想跟踪每本书的以下属性：

  * Title
  * Author
  * Subject
  * Book ID

## 定义结构体

为了定义一个结构体，您必须使用 struct 语句。struct 语句为程序定义了一个带有多个成员的新的数据类型。

例如，您可以按照如下的方式声明 Book 结构：

```C#
struct Books
{
   public string title;
   public string author;
   public string subject;
   public int book_id;
};  
```

下面的程序演示了结构的用法：

```C#
using System;
using System.Text;
     
struct Books
{
   public string title;
   public string author;
   public string subject;
   public int book_id;
};  

public class testStructure
{
   public static void Main(string[] args)
   {

      Books Book1;        /* 声明 Book1，类型为 Book */
      Books Book2;        /* 声明 Book2，类型为 Book */

      /* book 1 详述 */
      Book1.title = "C Programming";
      Book1.author = "Nuha Ali"; 
      Book1.subject = "C Programming Tutorial";
      Book1.book_id = 6495407;

      /* book 2 详述 */
      Book2.title = "Telecom Billing";
      Book2.author = "Zara Ali";
      Book2.subject =  "Telecom Billing Tutorial";
      Book2.book_id = 6495700;

      /* 打印 Book1 信息 */
      Console.WriteLine( "Book 1 title : {0}", Book1.title);
      Console.WriteLine("Book 1 author : {0}", Book1.author);
      Console.WriteLine("Book 1 subject : {0}", Book1.subject);
      Console.WriteLine("Book 1 book_id :{0}", Book1.book_id);

      /* 打印 Book2 信息 */
      Console.WriteLine("Book 2 title : {0}", Book2.title);
      Console.WriteLine("Book 2 author : {0}", Book2.author);
      Console.WriteLine("Book 2 subject : {0}", Book2.subject);
      Console.WriteLine("Book 2 book_id : {0}", Book2.book_id);       

      Console.ReadKey();

   }
}
```

## C# 结构的特点

您已经用了一个简单的名为 Books 的结构。在 C# 中的结构与传统的 C 或 C++ 中的结构不同。C# 中的结构有以下特点：

  * 结构可带有方法、字段、索引、属性、运算符方法和事件。
  * 结构可定义构造函数，但不能定义析构函数。但是，您不能为结构定义无参构造函数。无参构造函数(默认)是自动定义的，且不能被改变。
  * 与类不同，结构不能继承其他的结构或类。
  * 结构不能作为其他结构或类的基础结构。
  * 结构可实现一个或多个接口。
  * 结构成员不能指定为 abstract、virtual 或 protected。
  * 当您使用 **New** 操作符创建一个结构对象时，会调用适当的构造函数来创建结构。与类不同，结构可以不使用 New 操作符即可被实例化。
  * 如果不使用 New 操作符，只有在所有的字段都被初始化之后，字段才被赋值，对象才被使用。

## 类 vs 结构

类和结构有以下几个基本的不同点：

  * 类是引用类型，结构是值类型。
  * 结构不支持继承。
  * 结构不能声明默认的构造函数。

针对上述讨论，让我们重写前面的实例：

```C#
using System;
using System.Text;
     
struct Books
{
   private string title;
   private string author;
   private string subject;
   private int book_id;
   public void getValues(string t, string a, string s, int id)
   {
      title = t;
      author = a;
      subject = s;
      book_id =id; 
   }
   public void display()
   {
      Console.WriteLine("Title : {0}", title);
      Console.WriteLine("Author : {0}", author);
      Console.WriteLine("Subject : {0}", subject);
      Console.WriteLine("Book_id :{0}", book_id);
   }

};  

public class testStructure
{
   public static void Main(string[] args)
   {

      Books Book1 = new Books(); /* 声明 Book1，类型为 Book */
      Books Book2 = new Books(); /* 声明 Book2，类型为 Book */

      /* book 1 详述 */
      Book1.getValues("C Programming",
      "Nuha Ali", "C Programming Tutorial",6495407);

      /* book 2 详述 */
      Book2.getValues("Telecom Billing",
      "Zara Ali", "Telecom Billing Tutorial", 6495700);

      /* 打印 Book1 信息 */
      Book1.display();

      /* 打印 Book2 信息 */
      Book2.display(); 

      Console.ReadKey();

   }
}
```

# C# 枚举（Enum）

枚举是一组命名整型常量。枚举类型是使用 **enum** 关键字声明的。

C# 枚举是值类型。换句话说，枚举包含自己的值，且不能继承或传递继承。

## 声明 _enum_ 变量

声明枚举的一般语法：

```
enum <enum_name>
{ 
    enumeration list 
};
```

其中，

  * _enum_name_ 指定枚举的类型名称。
  * _enumeration list_ 是一个用逗号分隔的标识符列表。

枚举列表中的每个符号代表一个整数值，一个比它前面的符号大的整数值。默认情况下，第一个枚举符号的值是 0.例如：

```
enum Days { Sun, Mon, tue, Wed, thu, Fri, Sat };
```

## 实例

下面的实例演示了枚举变量的用法：

```C#
using System;

public class EnumTest
{
    enum Day { Sun, Mon, Tue, Wed, Thu, Fri, Sat };

    static void Main()
    {
        int x = (int)Day.Sun;
        int y = (int)Day.Fri;
        Console.WriteLine("Sun = {0}", x);
        Console.WriteLine("Fri = {0}", y);
    }
}
```

# C# 类（Class）

当你定义一个类时，你定义了一个数据类型的蓝图。这实际上并没有定义任何的数据，但它定义了类的名称意味着什么，也就是说，类的对象由什么组成及在这个对象上可执行什么操作。对象是类的实例。构成类的方法和变量成为类的成员。

## 类的定义

类的定义是以关键字 **class** 开始，后跟类的名称。类的主体，包含在一对花括号内。下面是类定义的一般形式：

```C#
<access specifier> class  class_name 
{
    // member variables
    <access specifier> <data type> variable1;
    <access specifier> <data type> variable2;
    ...
    <access specifier> <data type> variableN;
    // member methods
    <access specifier> <return type> method1(parameter_list) 
    {
        // method body 
    }
    <access specifier> <return type> method2(parameter_list) 
    {
        // method body 
    }
    ...
    <access specifier> <return type> methodN(parameter_list) 
    {
        // method body 
    }
}
```

请注意：

  * 访问标识符 <access specifier> 指定了对类及其成员的访问规则。如果没有指定，则使用默认的访问标识符。类的默认访问标识符是 **internal**，成员的默认访问标识符是 **private**。
  * 数据类型 <data type> 指定了变量的类型，返回类型 <return type> 指定了返回的方法返回的数据类型。
  * 如果要访问类的成员，你要使用点（.）运算符。
  * 点运算符链接了对象的名称和成员的名称。

下面的实例说明了目前为止所讨论的概念：

```C#
using System;
namespace BoxApplication
{
    class Box
    {
       public double length;   // 长度
       public double breadth;  // 宽度
       public double height;   // 高度
    }
    class Boxtester
    {
        static void Main(string[] args)
        {
            Box Box1 = new Box();        // 声明 Box1，类型为 Box
            Box Box2 = new Box();        // 声明 Box2，类型为 Box
            double volume = 0.0;         // 体积

            // Box1 详述
            Box1.height = 5.0;
            Box1.length = 6.0;
            Box1.breadth = 7.0;

            // Box2 详述
            Box2.height = 10.0;
            Box2.length = 12.0;
            Box2.breadth = 13.0;
           
            // Box1 的体积
            volume = Box1.height * Box1.length * Box1.breadth;
            Console.WriteLine("Box1 的体积： {0}",  volume);

            // Box2 的体积
            volume = Box2.height * Box2.length * Box2.breadth;
            Console.WriteLine("Box2 的体积： {0}", volume);
            Console.ReadKey();
        }
    }
}
```

## 成员函数和封装

类的成员函数是一个在类定义中有它的定义或原型的函数，就像其他变量一样。作为类的一个成员，它能在类的任何对象上操作，且能访问该对象的类的所有成员。

成员变量是对象的属性（从设计角度），且它们保持私有来实现封装。这些变量只能使用公共成员函数来访问。

让我们使用上面的概念来设置和获取一个类中不同的类成员的值：

```C#
using System;
namespace BoxApplication
{
    class Box
    {
       private double length;   // 长度
       private double breadth;  // 宽度
       private double height;   // 高度
       public void setLength( double len )
       {
            length = len;
       }

       public void setBreadth( double bre )
       {
            breadth = bre;
       }

       public void setHeight( double hei )
       {
            height = hei;
       }
       public double getVolume()
       {
           return length * breadth * height;
       }
    }
    class Boxtester
    {
        static void Main(string[] args)
        {
            Box Box1 = new Box();        // 声明 Box1，类型为 Box
            Box Box2 = new Box();                // 声明 Box2，类型为 Box
            double volume;                               // 体积


            // Box1 详述
            Box1.setLength(6.0);
            Box1.setBreadth(7.0);
            Box1.setHeight(5.0);

            // Box2 详述
            Box2.setLength(12.0);
            Box2.setBreadth(13.0);
            Box2.setHeight(10.0);
       
            // Box1 的体积
            volume = Box1.getVolume();
            Console.WriteLine("Box1 的体积： {0}" ,volume);

            // Box2 的体积
            volume = Box2.getVolume();
            Console.WriteLine("Box2 的体积： {0}", volume);
           
            Console.ReadKey();
        }
    }
}
```

## C# 中的构造函数

类的 **构造函数** 是类的一个特殊的成员函数，当创建类的新对象时执行。

构造函数的名称与类的名称完全相同，它没有任何返回类型。

下面的实例说明了构造函数的概念：

```C#
using System;
namespace LineApplication
{
   class Line
   {
      private double length;   // 线条的长度
      public Line()
      {
         Console.WriteLine("对象已创建");
      }

      public void setLength( double len )
      {
         length = len;
      }
      public double getLength()
      {
         return length;
      }

      static void Main(string[] args)
      {
         Line line = new Line();    
         // 设置线条长度
         line.setLength(6.0);
         Console.WriteLine("线条的长度： {0}", line.getLength());
         Console.ReadKey();
      }
   }
}
```

**默认的构造函数**没有任何参数。但是如果你需要一个带有参数的构造函数可以有参数，这种构造函数叫做**参数化构造函数**。这种技术可以帮助你在创建对象的同时给对象赋初始值，具体请看下面实例：

```C#
using System;
namespace LineApplication
{
   class Line
   {
      private double length;   // 线条的长度
      public Line(double len)  // 参数化构造函数
      {
         Console.WriteLine("对象已创建，length = {0}", len);
         length = len;
      }

      public void setLength( double len )
      {
         length = len;
      }
      public double getLength()
      {
         return length;
      }

      static void Main(string[] args)
      {
         Line line = new Line(10.0);
         Console.WriteLine("线条的长度： {0}", line.getLength()); 
         // 设置线条长度
         line.setLength(6.0);
         Console.WriteLine("线条的长度： {0}", line.getLength()); 
         Console.ReadKey();
      }
   }
}
```

## C# 中的析构函数

类的 **析构函数** 是类的一个特殊的成员函数，当类的对象超出范围时执行。

析构函数的名称是在类的名称前加上一个波浪形（~）作为前缀，它不返回值，也不带任何参数。

析构函数用于在结束程序（比如关闭文件、释放内存等）之前释放资源。析构函数不能继承或重载。

下面的实例说明了析构函数的概念：

```C#
using System;
namespace LineApplication
{
   class Line
   {
      private double length;   // 线条的长度
      public Line()  // 构造函数
      {
         Console.WriteLine("对象已创建");
      }
      ~Line() //析构函数
      {
         Console.WriteLine("对象已删除");
      }

      public void setLength( double len )
      {
         length = len;
      }
      public double getLength()
      {
         return length;
      }

      static void Main(string[] args)
      {
         Line line = new Line();
         // 设置线条长度
         line.setLength(6.0);
         Console.WriteLine("线条的长度： {0}", line.getLength());           
      }
   }
}
```

## C# 类的静态成员

我们可以使用 **static** 关键字把类成员定义为静态的。当我们声明一个类成员为静态时，意味着无论有多少个类的对象被创建，只会有一个该静态成员的副本。

关键字 **static** 意味着类中只有一个该成员的实例。静态变量用于定义常量，因为它们的值可以通过直接调用类而不需要创建类的实例来获取。静态变量可在成员函数或类的定义外部进行初始化。你也可以在类的定义内部初始化静态变量。

下面的实例演示了**静态变量**的用法：

```C#
using System;
namespace StaticVarApplication
{
    class StaticVar
    {
       public static int num;
        public void count()
        {
            num++;
        }
        public int getNum()
        {
            return num;
        }
    }
    class StaticTester
    {
        static void Main(string[] args)
        {
            StaticVar s1 = new StaticVar();
            StaticVar s2 = new StaticVar();
            s1.count();
            s1.count();
            s1.count();
            s2.count();
            s2.count();
            s2.count();         
            Console.WriteLine("s1 的变量 num： {0}", s1.getNum());
            Console.WriteLine("s2 的变量 num： {0}", s2.getNum());
            Console.ReadKey();
        }
    }
}
```

你也可以把一个**成员函数**声明为 **static**。这样的函数只能访问静态变量。静态函数在对象被创建之前就已经存在。下面的实例演示了**静态函数**的用法：

```C#
using System;
namespace StaticVarApplication
{
    class StaticVar
    {
       public static int num;
        public void count()
        {
            num++;
        }
        public static int getNum()
        {
            return num;
        }
    }
    class StaticTester
    {
        static void Main(string[] args)
        {
            StaticVar s = new StaticVar();
            s.count();
            s.count();
            s.count();                   
            Console.WriteLine("变量 num： {0}", StaticVar.getNum());
            Console.ReadKey();
        }
    }
}
```

# C# 继承

继承是面向对象程序设计中最重要的概念之一。继承允许我们根据一个类来定义另一个类，这使得创建和维护应用程序变得更容易。同时也有利于重用代码和节省开发时间。

当创建一个类时，程序员不需要完全重新编写新的数据成员和成员函数，只需要设计一个新的类，继承了已有的类的成员即可。这个已有的类被称为的**基类**，这个新的类被称为**派生类**。

继承的思想实现了 **属于（IS-A）** 关系。例如，哺乳动物 **属于（IS-A）** 动物，狗 **属于（IS-A）** 哺乳动物，因此狗 **属于（IS-A）** 动物。

## 基类和派生类

一个类可以派生自多个类或接口，这意味着它可以从多个基类或接口继承数据和函数。

C# 中创建派生类的语法如下：

```C#
<访问修饰符符> class <基类>
{
 ...
}
class <派生类> : <基类>
{
 ...
}
```

假设，有一个基类 Shape，它的派生类是 Rectangle：

```C#
using System;
namespace InheritanceApplication
{
   class Shape 
   {
      public void setWidth(int w)
      {
         width = w;
      }
      public void setHeight(int h)
      {
         height = h;
      }
      protected int width;
      protected int height;
   }

   // 派生类
   class Rectangle: Shape
   {
      public int getArea()
      { 
         return (width * height); 
      }
   }
   
   class RectangleTester
   {
      static void Main(string[] args)
      {
         Rectangle Rect = new Rectangle();

         Rect.setWidth(5);
         Rect.setHeight(7);

         // 打印对象的面积
         Console.WriteLine("总面积： {0}",  Rect.getArea());
         Console.ReadKey();
      }
   }
}
```

## 基类的初始化

派生类继承了基类的成员变量和成员方法。因此父类对象应在子类对象创建之前被创建。您可以在成员初始化列表中进行父类的初始化。

下面的程序演示了这点：

```C#
using System;
namespace RectangleApplication
{
   class Rectangle
   {
      // 成员变量
      protected double length;
      protected double width;
      public Rectangle(double l, double w)
      {
         length = l;
         width = w;
      }
      public double GetArea()
      {
         return length * width;
      }
      public void Display()
      {
         Console.WriteLine("长度： {0}", length);
         Console.WriteLine("宽度： {0}", width);
         Console.WriteLine("面积： {0}", GetArea());
      }
   }//end class Rectangle  
   class Tabletop : Rectangle
   {
      private double cost;
      public Tabletop(double l, double w) : base(l, w)
      { }
      public double GetCost()
      {
         double cost;
         cost = GetArea() * 70;
         return cost;
      }
      public void Display()
      {
         base.Display();
         Console.WriteLine("成本： {0}", GetCost());
      }
   }
   class ExecuteRectangle
   {
      static void Main(string[] args)
      {
         Tabletop t = new Tabletop(4.5, 7.5);
         t.Display();
         Console.ReadLine();
      }
   }
}
```

## C# 多重继承

多重继承指的是一个类别可以同时从多于一个父类继承行为与特征的功能。与单一继承相对，单一继承指一个类别只可以继承自一个父类。

**C# 不支持多重继承**。但是，您可以使用接口来实现多重继承。下面的程序演示了这点：

```C#
using System;
namespace InheritanceApplication
{
   class Shape 
   {
      public void setWidth(int w)
      {
         width = w;
      }
      public void setHeight(int h)
      {
         height = h;
      }
      protected int width;
      protected int height;
   }

   // 基类 PaintCost
   public interface PaintCost 
   {
      int getCost(int area);

   }
   // 派生类
   class Rectangle : Shape, PaintCost
   {
      public int getArea()
      {
         return (width * height);
      }
      public int getCost(int area)
      {
         return area * 70;
      }
   }
   class RectangleTester
   {
      static void Main(string[] args)
      {
         Rectangle Rect = new Rectangle();
         int area;
         Rect.setWidth(5);
         Rect.setHeight(7);
         area = Rect.getArea();
         // 打印对象的面积
         Console.WriteLine("总面积： {0}",  Rect.getArea());
         Console.WriteLine("油漆总成本： ${0}" , Rect.getCost(area));
         Console.ReadKey();
      }
   }
}
```

# C# 多态性

多态是同一个行为具有多个不同表现形式或形态的能力。

**多态性**意味着有多重形式。在面向对象编程范式中，多态性往往表现为"一个接口，多个功能"。

多态性可以是静态的或动态的。在**静态多态性**中，函数的响应是在编译时发生的。在**动态多态性**中，函数的响应是在运行时发生的。

在 C# 中，每个类型都是多态的，因为包括用户定义类型在内的所有类型都继承自 Object。

多态就是同一个接口，使用不同的实例而执行不同操作。

现实中，比如我们按下 F1 键这个动作：

  * 如果当前在 Flash 界面下弹出的就是 AS 3 的帮助文档；
  * 如果当前在 Word 下弹出的就是 Word 帮助；
  * 在 Windows 下弹出的就是 Windows 帮助和支持。

同一个事件发生在不同的对象上会产生不同的结果。

## 静态多态性

在编译时，函数和对象的连接机制被称为早期绑定，也被称为静态绑定。C# 提供了两种技术来实现静态多态性。分别为：

  * 函数重载
  * 运算符重载

运算符重载将在下一章节讨论，接下来我们将讨论函数重载。

## 函数重载

您可以在同一个范围内对相同的函数名有多个定义。函数的定义必须彼此不同，可以是参数列表中的参数类型不同，也可以是参数个数不同。不能重载只有返回类型不同的函数声明。

下面的实例演示了几个相同的函数 **Add()**，用于对不同个数参数进行相加处理：

```C#
using System;
namespace PolymorphismApplication
{
    public class TestData  
    {  
        public int Add(int a, int b, int c)  
        {  
            return a + b + c;  
        }  
        public int Add(int a, int b)  
        {  
            return a + b;  
        }  
    }  
    class Program  
    {  
        static void Main(string[] args)  
        {  
            TestData dataClass = new TestData();
            int add1 = dataClass.Add(1, 2);  
            int add2 = dataClass.Add(1, 2, 3);

            Console.WriteLine("add1 :" + add1);
            Console.WriteLine("add2 :" + add2);  
        }  
    }  
}
```

下面的实例演示了几个相同的函数 **print()**，用于打印不同的数据类型：

```C#
using System;
namespace PolymorphismApplication
{
   class Printdata
   {
      void print(int i)
      {
         Console.WriteLine("输出整型: {0}", i );
      }

      void print(double f)
      {
         Console.WriteLine("输出浮点型: {0}" , f);
      }

      void print(string s)
      {
         Console.WriteLine("输出字符串: {0}", s);
      }
      static void Main(string[] args)
      {
         Printdata p = new Printdata();
         // 调用 print 来打印整数
         p.print(1);
         // 调用 print 来打印浮点数
         p.print(1.23);
         // 调用 print 来打印字符串
         p.print("Hello Runoob");
         Console.ReadKey();
      }
   }
}
```

## 动态多态性

C# 允许您使用关键字 **abstract** 创建抽象类，用于提供接口的部分类的实现。当一个派生类继承自该抽象类时，实现即完成。**抽象类**包含抽象方法，抽象方法可被派生类实现。派生类具有更专业的功能。

请注意，下面是有关抽象类的一些规则：

  * 您不能创建一个抽象类的实例。
  * 您不能在一个抽象类外部声明一个抽象方法。
  * 通过在类定义前面放置关键字 **sealed**，可以将类声明为**密封类**。当一个类被声明为 **sealed** 时，它不能被继承。抽象类不能被声明为 sealed。

下面的程序演示了一个抽象类：

```C#
using System;
namespace PolymorphismApplication
{
   abstract class Shape
   {
       abstract public int area();
   }
   class Rectangle:  Shape
   {
      private int length;
      private int width;
      public Rectangle( int a=0, int b=0)
      {
         length = a;
         width = b;
      }
      public override int area ()
      { 
         Console.WriteLine("Rectangle 类的面积：");
         return (width * length); 
      }
   }

   class RectangleTester
   {
      static void Main(string[] args)
      {
         Rectangle r = new Rectangle(10, 7);
         double a = r.area();
         Console.WriteLine("面积： {0}",a);
         Console.ReadKey();
      }
   }
}
```

当有一个定义在类中的函数需要在继承类中实现时，可以使用**虚方法**。

虚方法是使用关键字 **virtual** 声明的。

虚方法可以在不同的继承类中有不同的实现。

对虚方法的调用是在运行时发生的。

动态多态性是通过 **抽象类** 和 **虚方法** 实现的。

以下实例创建了 Shape 基类，并创建派生类 Circle、 Rectangle、Triangle， Shape 类提供一个名为 Draw 的虚拟方法，在每个派生类中重写该方法以绘制该类的指定形状。

```C#
using System;
using System.Collections.Generic;

public class Shape
{
    public int X { get; private set; }
    public int Y { get; private set; }
    public int Height { get; set; }
    public int Width { get; set; }
   
    // 虚方法
    public virtual void Draw()
    {
        Console.WriteLine("执行基类的画图任务");
    }
}

class Circle : Shape
{
    public override void Draw()
    {
        Console.WriteLine("画一个圆形");
        base.Draw();
    }
}
class Rectangle : Shape
{
    public override void Draw()
    {
        Console.WriteLine("画一个长方形");
        base.Draw();
    }
}
class Triangle : Shape
{
    public override void Draw()
    {
        Console.WriteLine("画一个三角形");
        base.Draw();
    }
}

class Program
{
    static void Main(string[] args)
    {
        // 创建一个 List<Shape> 对象，并向该对象添加 Circle、Triangle 和 Rectangle
        var shapes = new List<Shape>
        {
            new Rectangle(),
            new Triangle(),
            new Circle()
        };

        // 使用 foreach 循环对该列表的派生类进行循环访问，并对其中的每个 Shape 对象调用 Draw 方法 
        foreach (var shape in shapes)
        {
            shape.Draw();
        }

        Console.WriteLine("按下任意键退出。");
        Console.ReadKey();
    }

}
```

下面的程序演示通过虚方法 area() 来计算不同形状图像的面积：

```C#
using System;
namespace PolymorphismApplication
{
   class Shape 
   {
      protected int width, height;
      public Shape( int a=0, int b=0)
      {
         width = a;
         height = b;
      }
      public virtual int area()
      {
         Console.WriteLine("父类的面积：");
         return 0;
      }
   }
   class Rectangle: Shape
   {
      public Rectangle( int a=0, int b=0): base(a, b)
      {

      }
      public override int area ()
      {
         Console.WriteLine("Rectangle 类的面积：");
         return (width * height); 
      }
   }
   class Triangle: Shape
   {
      public Triangle(int a = 0, int b = 0): base(a, b)
      {
      
      }
      public override int area()
      {
         Console.WriteLine("Triangle 类的面积：");
         return (width * height / 2); 
      }
   }
   class Caller
   {
      public void CallArea(Shape sh)
      {
         int a;
         a = sh.area();
         Console.WriteLine("面积： {0}", a);
      }
   }  
   class Tester
   {
      
      static void Main(string[] args)
      {
         Caller c = new Caller();
         Rectangle r = new Rectangle(10, 7);
         Triangle t = new Triangle(10, 5);
         c.CallArea(r);
         c.CallArea(t);
         Console.ReadKey();
      }
   }
}
```

# C# 运算符重载

您可以重定义或重载 C# 中内置的运算符。因此，程序员也可以使用用户自定义类型的运算符。重载运算符是具有特殊名称的函数，是通过关键字 **operator** 后跟运算符的符号来定义的。与其他函数一样，重载运算符有返回类型和参数列表。

例如，请看下面的函数：

```C#
public static Box operator+ (Box b, Box c)
{
   Box box = new Box();
   box.length = b.length + c.length;
   box.breadth = b.breadth + c.breadth;
   box.height = b.height + c.height;
   return box;
}
```

上面的函数为用户自定义的类 Box 实现了加法运算符（+）。它把两个 Box 对象的属性相加，并返回相加后的 Box 对象。

## 运算符重载的实现

下面的程序演示了完整的实现：

```C#
using System;

namespace OperatorOvlApplication
{
   class Box
   {
      private double length;      // 长度
      private double breadth;     // 宽度
      private double height;      // 高度

      public double getVolume()
      {
         return length * breadth * height;
      }
      public void setLength( double len )
      {
         length = len;
      }

      public void setBreadth( double bre )
      {
         breadth = bre;
      }

      public void setHeight( double hei )
      {
         height = hei;
      }
      // 重载 + 运算符来把两个 Box 对象相加
      public static Box operator+ (Box b, Box c)
      {
         Box box = new Box();
         box.length = b.length + c.length;
         box.breadth = b.breadth + c.breadth;
         box.height = b.height + c.height;
         return box;
      }

   }

   class Tester
   {
      static void Main(string[] args)
      {
         Box Box1 = new Box();         // 声明 Box1，类型为 Box
         Box Box2 = new Box();         // 声明 Box2，类型为 Box
         Box Box3 = new Box();         // 声明 Box3，类型为 Box
         double volume = 0.0;          // 体积

         // Box1 详述
         Box1.setLength(6.0);
         Box1.setBreadth(7.0);
         Box1.setHeight(5.0);

         // Box2 详述
         Box2.setLength(12.0);
         Box2.setBreadth(13.0);
         Box2.setHeight(10.0);

         // Box1 的体积
         volume = Box1.getVolume();
         Console.WriteLine("Box1 的体积： {0}", volume);

         // Box2 的体积
         volume = Box2.getVolume();
         Console.WriteLine("Box2 的体积： {0}", volume);

         // 把两个对象相加
         Box3 = Box1 + Box2;

         // Box3 的体积
         volume = Box3.getVolume();
         Console.WriteLine("Box3 的体积： {0}", volume);
         Console.ReadKey();
      }
   }
}
```

## 可重载和不可重载运算符

下表描述了 C# 中运算符重载的能力：

| 运算符                                     | 描述                     |
|-----------------------------------------|------------------------|
| \+, \-, \!, ~, \+\+, \-\-               | 这些一元运算符只有一个操作数，且可以被重载。 |
| \+, \-, \*, /, %                        | 这些二元运算符带有两个操作数，且可以被重载。 |
| ==, \!=, <, >, <=, >=                   | 这些比较运算符可以被重载。          |
| &&, \|\|                                | 这些条件逻辑运算符不能被直接重载。      |
| \+=, \-=, \*=, /=, %=                   | 这些赋值运算符不能被重载。          |
| =, \., ?:, \->, new, is, sizeof, typeof | 这些运算符不能被重载。            |

## 实例

针对上述讨论，让我们扩展上面的实例，重载更多的运算符：

```C#
using System;

namespace OperatorOvlApplication
{
    class Box
    {
       private double length;      // 长度
       private double breadth;     // 宽度
       private double height;      // 高度
      
       public double getVolume()
       {
         return length * breadth * height;
       }
      public void setLength( double len )
      {
          length = len;
      }

      public void setBreadth( double bre )
      {
          breadth = bre;
      }

      public void setHeight( double hei )
      {
          height = hei;
      }
      // 重载 + 运算符来把两个 Box 对象相加
      public static Box operator+ (Box b, Box c)
      {
          Box box = new Box();
          box.length = b.length + c.length;
          box.breadth = b.breadth + c.breadth;
          box.height = b.height + c.height;
          return box;
      }
      
      public static bool operator == (Box lhs, Box rhs)
      {
          bool status = false;
          if (lhs.length == rhs.length && lhs.height == rhs.height 
             && lhs.breadth == rhs.breadth)
          {
              status = true;
          }
          return status;
      }
      public static bool operator !=(Box lhs, Box rhs)
      {
          bool status = false;
          if (lhs.length != rhs.length || lhs.height != rhs.height 
              || lhs.breadth != rhs.breadth)
          {
              status = true;
          }
          return status;
      }
      public static bool operator <(Box lhs, Box rhs)
      {
          bool status = false;
          if (lhs.length < rhs.length && lhs.height 
              < rhs.height && lhs.breadth < rhs.breadth)
          {
              status = true;
          }
          return status;
      }

      public static bool operator >(Box lhs, Box rhs)
      {
          bool status = false;
          if (lhs.length > rhs.length && lhs.height 
              > rhs.height && lhs.breadth > rhs.breadth)
          {
              status = true;
          }
          return status;
      }

      public static bool operator <=(Box lhs, Box rhs)
      {
          bool status = false;
          if (lhs.length <= rhs.length && lhs.height 
              <= rhs.height && lhs.breadth <= rhs.breadth)
          {
              status = true;
          }
          return status;
      }

      public static bool operator >=(Box lhs, Box rhs)
      {
          bool status = false;
          if (lhs.length >= rhs.length && lhs.height 
             >= rhs.height && lhs.breadth >= rhs.breadth)
          {
              status = true;
          }
          return status;
      }
      public override string ToString()
      {
          return String.Format("({0}, {1}, {2})", length, breadth, height);
      }
   
   }
    
   class Tester
   {
      static void Main(string[] args)
      {
        Box Box1 = new Box();          // 声明 Box1，类型为 Box
        Box Box2 = new Box();          // 声明 Box2，类型为 Box
        Box Box3 = new Box();          // 声明 Box3，类型为 Box
        Box Box4 = new Box();
        double volume = 0.0;   // 体积

        // Box1 详述
        Box1.setLength(6.0);
        Box1.setBreadth(7.0);
        Box1.setHeight(5.0);

        // Box2 详述
        Box2.setLength(12.0);
        Box2.setBreadth(13.0);
        Box2.setHeight(10.0);

       // 使用重载的 ToString() 显示两个盒子
        Console.WriteLine("Box1： {0}", Box1.ToString());
        Console.WriteLine("Box2： {0}", Box2.ToString());
        
        // Box1 的体积
        volume = Box1.getVolume();
        Console.WriteLine("Box1 的体积： {0}", volume);

        // Box2 的体积
        volume = Box2.getVolume();
        Console.WriteLine("Box2 的体积： {0}", volume);

        // 把两个对象相加
        Box3 = Box1 + Box2;
        Console.WriteLine("Box3： {0}", Box3.ToString());
        // Box3 的体积
        volume = Box3.getVolume();
        Console.WriteLine("Box3 的体积： {0}", volume);

        //comparing the boxes
        if (Box1 > Box2)
          Console.WriteLine("Box1 大于 Box2");
        else
          Console.WriteLine("Box1 不大于 Box2");
        if (Box1 < Box2)
          Console.WriteLine("Box1 小于 Box2");
        else
          Console.WriteLine("Box1 不小于 Box2");
        if (Box1 >= Box2)
          Console.WriteLine("Box1 大于等于 Box2");
        else
          Console.WriteLine("Box1 不大于等于 Box2");
        if (Box1 <= Box2)
          Console.WriteLine("Box1 小于等于 Box2");
        else
          Console.WriteLine("Box1 不小于等于 Box2");
        if (Box1 != Box2)
          Console.WriteLine("Box1 不等于 Box2");
        else
          Console.WriteLine("Box1 等于 Box2");
        Box4 = Box3;
        if (Box3 == Box4)
          Console.WriteLine("Box3 等于 Box4");
        else
          Console.WriteLine("Box3 不等于 Box4");

        Console.ReadKey();
      }
    }
}
```

# C# 接口（Interface）

接口定义了所有类继承接口时应遵循的语法合同。接口定义了语法合同 **"是什么"** 部分，派生类定义了语法合同 **"怎么做"** 部分。

接口定义了属性、方法和事件，这些都是接口的成员。接口只包含了成员的声明。成员的定义是派生类的责任。接口提供了派生类应遵循的标准结构。

接口使得实现接口的类或结构在形式上保持一致。

抽象类在某种程度上与接口类似，但是，它们大多只是用在当只有少数方法由基类声明由派生类实现时。

* * *

## 定义接口: MyInterface.cs

接口使用 **interface** 关键字声明，它与类的声明类似。接口声明默认是 public 的。下面是一个接口声明的实例：

```
interface IMyInterface
{
    void MethodToImplement();
}
```

以上代码定义了接口 IMyInterface。通常接口命令以 I 字母开头，这个接口只有一个方法 MethodToImplement()，没有参数和返回值，当然我们可以按照需求设置参数和返回值。

值得注意的是，该方法并没有具体的实现。

### 接下来我们来实现以上接口：InterfaceImplementer.cs

```C#
using System;

interface IMyInterface
{
        // 接口成员
    void MethodToImplement();
}

class InterfaceImplementer : IMyInterface
{
    static void Main()
    {
        InterfaceImplementer iImp = new InterfaceImplementer();
        iImp.MethodToImplement();
    }

    public void MethodToImplement()
    {
        Console.WriteLine("MethodToImplement() called.");
    }
}
```

InterfaceImplementer 类实现了 IMyInterface 接口，接口的实现与类的继承语法格式类似：

```C#
class InterfaceImplementer : IMyInterface
```

继承接口后，我们需要实现接口的方法 MethodToImplement() , 方法名必须与接口定义的方法名一致。

* * *

## 接口继承: InterfaceInheritance.cs

以下实例定义了两个接口 IMyInterface 和 IParentInterface。

如果一个接口继承其他接口，那么实现类或结构就需要实现所有接口的成员。

以下实例 IMyInterface 继承了 IParentInterface 接口，因此接口实现类必须实现 MethodToImplement() 和 ParentInterfaceMethod() 方法：

```C#
using System;

interface IParentInterface
{
    void ParentInterfaceMethod();
}

interface IMyInterface : IParentInterface
{
    void MethodToImplement();
}

class InterfaceImplementer : IMyInterface
{
    static void Main()
    {
        InterfaceImplementer iImp = new InterfaceImplementer();
        iImp.MethodToImplement();
        iImp.ParentInterfaceMethod();
    }

    public void MethodToImplement()
    {
        Console.WriteLine("MethodToImplement() called.");
    }

    public void ParentInterfaceMethod()
    {
        Console.WriteLine("ParentInterfaceMethod() called.");
    }
}
```

# C# 命名空间（Namespace）

**命名空间**的设计目的是提供一种让一组名称与其他名称分隔开的方式。在一个命名空间中声明的类的名称与另一个命名空间中声明的相同的类的名称不冲突。

我们举一个计算机系统中的例子，一个文件夹(目录)中可以包含多个文件夹，每个文件夹中不能有相同的文件名，但不同文件夹中的文件可以重名。

## 定义命名空间

命名空间的定义是以关键字 **namespace** 开始，后跟命名空间的名称，如下所示：

```C#
namespace namespace_name
{
   // 代码声明
}
```

为了调用支持命名空间版本的函数或变量，会把命名空间的名称置于前面，如下所示：

```
namespace_name.item_name;
```

下面的程序演示了命名空间的用法：

```C#
using System;
namespace first_space
{
   class namespace_cl
   {
      public void func()
      {
         Console.WriteLine("Inside first_space");
      }
   }
}
namespace second_space
{
   class namespace_cl
   {
      public void func()
      {
         Console.WriteLine("Inside second_space");
      }
   }
}   
class TestClass
{
   static void Main(string[] args)
   {
      first_space.namespace_cl fc = new first_space.namespace_cl();
      second_space.namespace_cl sc = new second_space.namespace_cl();
      fc.func();
      sc.func();
      Console.ReadKey();
   }
}
```

## _using_ 关键字

**using** 关键字表明程序使用的是给定命名空间中的名称。例如，我们在程序中使用 **System** 命名空间，其中定义了类 Console。我们可以只写：

```
Console.WriteLine ("Hello there");
```

我们可以写完全限定名称，如下：

```
System.Console.WriteLine("Hello there");
```

您也可以使用 **using** 命名空间指令，这样在使用的时候就不用在前面加上命名空间名称。该指令告诉编译器随后的代码使用了指定命名空间中的名称。下面的代码演示了命名空间的应用。

让我们使用 using 指定重写上面的实例：
```C#
using System;
using first_space;
using second_space;

namespace first_space
{
   class abc
   {
      public void func()
      {
         Console.WriteLine("Inside first_space");
      }
   }
}
namespace second_space
{
   class efg
   {
      public void func()
      {
         Console.WriteLine("Inside second_space");
      }
   }
}   
class TestClass
{
   static void Main(string[] args)
   {
      abc fc = new abc();
      efg sc = new efg();
      fc.func();
      sc.func();
      Console.ReadKey();
   }
}
```

## 嵌套命名空间

命名空间可以被嵌套，即您可以在一个命名空间内定义另一个命名空间，如下所示：

```C#
namespace namespace_name1 
{
   // 代码声明
   namespace namespace_name2 
   {
     // 代码声明
   }
}
```

您可以使用点（.）运算符访问嵌套的命名空间的成员，如下所示：

```C#
using System;
using SomeNameSpace;
using SomeNameSpace.Nested;

namespace SomeNameSpace
{
    public class MyClass 
    {
        static void Main() 
        {
            Console.WriteLine("In SomeNameSpace");
            Nested.NestedNameSpaceClass.SayHello();
        }
    }

    // 内嵌命名空间
    namespace Nested   
    {
        public class NestedNameSpaceClass 
        {
            public static void SayHello() 
            {
                Console.WriteLine("In Nested");
            }
        }
    }
}
```

# C# 预处理器指令

预处理器指令指导编译器在实际编译开始之前对信息进行预处理。

所有的预处理器指令都是以 # 开始。且在一行上，只有空白字符可以出现在预处理器指令之前。预处理器指令不是语句，所以它们不以分号（;）结束。

C# 编译器没有一个单独的预处理器，但是，指令被处理时就像是有一个单独的预处理器一样。在 C# 中，预处理器指令用于在条件编译中起作用。与 C 和 C++ 不同的是，它们不是用来创建宏。一个预处理器指令必须是该行上的唯一指令。

## C# 预处理器指令列表

下表列出了 C# 中可用的预处理器指令：

| 预处理器指令      | 描述                                                        |
|-------------|-----------------------------------------------------------|
| \#define    | 它用于定义一系列成为符号的字符。                                          |
| \#undef     | 它用于取消定义符号。                                                |
| \#if        | 它用于测试符号是否为真。                                              |
| \#else      | 它用于创建复合条件指令，与 \#if 一起使用。                                  |
| \#elif      | 它用于创建复合条件指令。                                              |
| \#endif     | 指定一个条件指令的结束。                                              |
| \#line      | 它可以让您修改编译器的行数以及（可选地）输出错误和警告的文件名。                          |
| \#error     | 它允许从代码的指定位置生成一个错误。                                        |
| \#warning   | 它允许从代码的指定位置生成一级警告。                                        |
| \#region    | 它可以让您在使用 Visual Studio Code Editor 的大纲特性时，指定一个可展开或折叠的代码块。 |
| \#endregion | 它标识着 \#region 块的结束。                                       |

## #define 预处理器

#define 预处理器指令创建符号常量。

#define 允许您定义一个符号，这样，通过使用符号作为传递给 #if 指令的表达式，表达式将返回 true。它的语法如下：

```
#define symbol
```

下面的程序说明了这点：

```C#
#define PI 
using System;
namespace PreprocessorDAppl
{
   class Program
   {
      static void Main(string[] args)
      {
         #if (PI)
            Console.WriteLine("PI is defined");
         #else
            Console.WriteLine("PI is not defined");
         #endif
         Console.ReadKey();
      }
   }
}
```

## 条件指令

您可以使用 #if 指令来创建一个条件指令。条件指令用于测试符号是否为真。如果为真，编译器会执行 #if 和下一个指令之间的代码。

条件指令的语法：

```
#if symbol [operator symbol]...
```

其中，_symbol_ 是要测试的符号名称。您也可以使用 true 和 false，或在符号前放置否定运算符。

常见运算符有：

  * == (等于)
  * != (不等于)
  * && (与)
  * || (或)

您也可以用括号把符号和运算符进行分组。条件指令用于在调试版本或编译指定配置时编译代码。一个以 **#if** 指令开始的条件指令，必须显示地以一个 **#endif** 指令终止。

下面的程序演示了条件指令的用法：

```C#
#define DEBUG
#define VC_V10
using System;
public class TestClass
{
   public static void Main()
   {

      #if (DEBUG && !VC_V10)
         Console.WriteLine("DEBUG is defined");
      #elif (!DEBUG && VC_V10)
         Console.WriteLine("VC_V10 is defined");
      #elif (DEBUG && VC_V10)
         Console.WriteLine("DEBUG and VC_V10 are defined");
      #else
         Console.WriteLine("DEBUG and VC_V10 are not defined");
      #endif
      Console.ReadKey();
   }
}
```

# C# 正则表达式

**正则表达式** 是一种匹配输入文本的模式。.Net 框架提供了允许这种匹配的正则表达式引擎。模式由一个或多个字符、运算符和结构组成。

## 定义正则表达式

下面列出了用于定义正则表达式的各种类别的字符、运算符和结构。

  * 字符转义
  * 字符类
  * 定位点
  * 分组构造
  * 限定符
  * 反向引用构造
  * 备用构造
  * 替换
  * 杂项构造

### 字符转义

正则表达式中的反斜杠字符（\）指示其后跟的字符是特殊字符，或应按原义解释该字符。 

下表列出了转义字符：

| 转义字符        | 描述                                         | 模式                                               | 匹配                                        |
|-------------|--------------------------------------------|--------------------------------------------------|-------------------------------------------|
| \\a         | 与报警 \(bell\) 符 \\u0007 匹配。                 | \\a                                              | "Warning\!" \+ '\\u0007' 中的 "\\u0007"     |
| \\b         | 在字符类中，与退格键 \\u0008 匹配。                     | \[\\b\]\{3,\}                                    | "\\b\\b\\b\\b" 中的 "\\b\\b\\b\\b"          |
| \\t         | 与制表符 \\u0009 匹配。                           | \(\\w\+\)\\t                                     | "Name\\tAddr\\t" 中的 "Name\\t" 和 "Addr\\t" |
| \\r         | 与回车符 \\u000D 匹配。（\\r 与换行符 \\n 不是等效的。）      | \\r\\n\(\\w\+\)                                  | "\\r\\Hello\\nWorld\." 中的 "\\r\\nHello"   |
| \\v         | 与垂直制表符 \\u000B 匹配。                         | \[\\v\]\{2,\}                                    | "\\v\\v\\v" 中的 "\\v\\v\\v"                |
| \\f         | 与换页符 \\u000C 匹配。                           | \[\\f\]\{2,\}                                    | "\\f\\f\\f" 中的 "\\f\\f\\f"                |
| \\n         | 与换行符 \\u000A 匹配。                           | \\r\\n\(\\w\+\)                                  | "\\r\\Hello\\nWorld\." 中的 "\\r\\nHello"   |
| \\e         | 与转义符 \\u001B 匹配。                           | \\e                                              | "\\x001B" 中的 "\\x001B"                    |
| \\ nnn      | 使用八进制表示形式指定一个字符（nnn 由二到三位数字组成）。            | \\w\\040\\w                                      | "a bc d" 中的 "a b" 和 "c d"                 |
| \\x nn      | 使用十六进制表示形式指定字符（nn 恰好由两位数字组成）。              | \\w\\x20\\w                                      | "a bc d" 中的 "a b" 和 "c d"                 |
| \\c X \\c x | 匹配 X 或 x 指定的 ASCII 控件字符，其中 X 或 x 是控件字符的字母。 | \\cC                                             | "\\x0003" 中的 "\\x0003" \(Ctrl\-C\)        |
| \\u nnnn    | 使用十六进制表示形式匹配一个 Unicode 字符（由 nnnn 表示的四位数）。  | \\w\\u0020\\w                                    | "a bc d" 中的 "a b" 和 "c d"                 |
| \\          | 在后面带有不识别的转义字符时，与该字符匹配。                     | \\d\+\[\\\+\-x\\\*\]\\d\+\\d\+\[\\\+\-x\\\*\\d\+ | "\(2\+2\) \* 3\*9" 中的 "2\+2" 和 "3\*9"     |


### 字符类

字符类与一组字符中的任何一个字符匹配。

下表列出了字符类：

| 字符类                                               | 描述                                                                   | 模式                               | 匹配                                    |
|---------------------------------------------------|----------------------------------------------------------------------|----------------------------------|---------------------------------------|
| \[character\_group\]                              | 匹配 character\_group 中的任何单个字符。 默认情况下，匹配区分大小写。                         | \[mn\]                           | "mat" 中的 "m"，"moon" 中的 "m" 和 "n"      |
| \[^character\_group\]                             | 非：与不在 character\_group 中的任何单个字符匹配。 默认情况下，character\_group 中的字符区分大小写。 | \[^aei\]                         | "avail" 中的 "v" 和 "l"                  |
| \[ first \- last \]                               | 字符范围：与从 first 到 last 的范围中的任何单个字符匹配。                                  | \[b\-d\]                         | \[b\-d\]irds 可以匹配 Birds、 Cirds、 Dirds |
| \.                                                | 通配符：与除 \\n 之外的任何单个字符匹配。                                              |
| 若要匹配原意句点字符（\. 或 \\u002E），您必须在该字符前面加上转义符 \(\\\.\)。 | a\.e                                                                 | "have" 中的 "ave"， "mate" 中的 "ate" |
| \\p\{ name \}                                     | 与 name 指定的 Unicode 通用类别或命名块中的任何单个字符匹配。                               | \\p\{Lu\}                        | "City Lights" 中的 "C" 和 "L"            |
| \\P\{ name \}                                     | 与不在 name 指定的 Unicode 通用类别或命名块中的任何单个字符匹配。                             | \\P\{Lu\}                        | "City" 中的 "i"、 "t" 和 "y"              |
| \\w                                               | 与任何单词字符匹配。                                                           | \\w                              | "Room\#1" 中的 "R"、 "o"、 "m" 和 "1"      |
| \\W                                               | 与任何非单词字符匹配。                                                          | \\W                              | "Room\#1" 中的 "\#"                     |
| \\s                                               | 与任何空白字符匹配。                                                           | \\w\\s                           | "ID A1\.3" 中的 "D "                    |
| \\S                                               | 与任何非空白字符匹配。                                                          | \\s\\S                           | "int \_\_ctr" 中的 " \_"                |
| \\d                                               | 与任何十进制数字匹配。                                                          | \\d                              | "4 = IV" 中的 "4"                       |
| \\D                                               | 匹配不是十进制数的任意字符。                                                       | \\D                              | "4 = IV" 中的 " "、 "="、 " "、 "I" 和 "V"  |


### 定位点

定位点或原子零宽度断言会使匹配成功或失败，具体取决于字符串中的当前位置，但它们不会使引擎在字符串中前进或使用字符。

下表列出了定位点：

| 断言  | 描述                                | 模式             | 匹配                                                        |
|-----|-----------------------------------|----------------|-----------------------------------------------------------|
| ^   | 匹配必须从字符串或一行的开头开始。                 | ^\\d\{3\}      | "567\-777\-" 中的 "567"                                     |
| $   | 匹配必须出现在字符串的末尾或出现在行或字符串末尾的 \\n 之前。 | \-\\d\{4\}$    | "8\-12\-2012" 中的 "\-2012"                                 |
| \\A | 匹配必须出现在字符串的开头。                    | \\A\\w\{4\}    | "Code\-007\-" 中的 "Code"                                   |
| \\Z | 匹配必须出现在字符串的末尾或出现在字符串末尾的 \\n 之前。   | \-\\d\{3\}\\Z  | "Bond\-901\-007" 中的 "\-007"                               |
| \\z | 匹配必须出现在字符串的末尾。                    | \-\\d\{3\}\\z  | "\-901\-333" 中的 "\-333"                                   |
| \\G | 匹配必须出现在上一个匹配结束的地方。                | \\G\\\(\\d\\\) | "\(1\)\(3\)\(5\)\[7\]\(9\)" 中的 "\(1\)"、 "\(3\)" 和 "\(5\)" |
| \\b | 匹配一个单词边界，也就是指单词和空格间的位置。           | er\\b          | 匹配"never"中的"er"，但不能匹配"verb"中的"er"。                        |
| \\B | 匹配非单词边界。                          | er\\B          | 匹配"verb"中的"er"，但不能匹配"never"中的"er"。                        |

### 分组构造

分组构造描述了正则表达式的子表达式，通常用于捕获输入字符串的子字符串。

下表列出了分组构造：

| 分组构造                                | 描述                          | 模式                                                                                                         | 匹配                                                              |
|-------------------------------------|-----------------------------|------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------|
| \( subexpression \)                 | 捕获匹配的子表达式并将其分配到一个从零开始的序号中。  | \(\\w\)\\1                                                                                                 | "deep" 中的 "ee"                                                  |
| \(?< name >subexpression\)          | 将匹配的子表达式捕获到一个命名组中。          | \(?< double>\\w\)\\k< double>                                                                              | "deep" 中的 "ee"                                                  |
| \(?< name1 \-name2 >subexpression\) | 定义平衡组定义。                    | \(\(\(?'Open'\\\(\)\[^\\\(\\\)\]\*\)\+\(\(?'Close\-Open'\\\)\)\[^\\\(\\\)\]\*\)\+\)\*\(?\(Open\)\(?\!\)\)$ | "3\+2^\(\(1\-3\)\*\(3\-1\)\)" 中的 "\(\(1\-3\)\*\(3\-1\)\)"       |
| \(?: subexpression\)                | 定义非捕获组。                     | Write\(?:Line\)?                                                                                           | "Console\.WriteLine\(\)" 中的 "WriteLine"                         |
| \(?imnsx\-imnsx:subexpression\)     | 应用或禁用 subexpression 中指定的选项。 | A\\d\{2\}\(?i:\\w\+\)\\b                                                                                   | "A12xl A12XL a12xl" 中的 "A12xl" 和 "A12XL"                        |
| \(?= subexpression\)                | 零宽度正预测先行断言。                 | \\w\+\(?=\\\.\)                                                                                            | "He is\. The dog ran\. The sun is out\." 中的 "is"、 "ran" 和 "out" |
| \(?\! subexpression\)               | 零宽度负预测先行断言。                 | \\b\(?\!un\)\\w\+\\b                                                                                       | "unsure sure unity used" 中的 "sure" 和 "used"                     |
| \(?<=subexpression\)                | 零宽度正回顾后发断言。                 | \(?<=19\)\\d\{2\}\\b                                                                                       | "1851 1999 1950 1905 2003" 中的 "99"、"50"和 "05"                   |
| \(?<\! subexpression\)              | 零宽度负回顾后发断言。                 | \(?<\!wo\)man\\b                                                                                           | "Hi woman Hi man" 中的 "man"                                      |
| \(?> subexpression\)                | 非回溯（也称为"贪婪"）子表达式。           | \[13579\]\(?>A\+B\+\)                                                                                      | "1ABB 3ABBC 5AB 5AC" 中的 "1ABB"、 "3ABB" 和 "5AB"                  |

### 限定符

限定符指定在输入字符串中必须存在上一个元素（可以是字符、组或字符类）的多少个实例才能出现匹配项。 限定符包括下表中列出的语言元素。

下表列出了限定符：

| 限定符          | 描述                             | 模式            | 匹配                                                               |
|--------------|--------------------------------|---------------|------------------------------------------------------------------|
| \*           | 匹配上一个元素零次或多次。                  | \\d\*\\\.\\d  | "\.0"、 "19\.9"、 "219\.9"                                         |
| \+           | 匹配上一个元素一次或多次。                  | "be\+"        | "been" 中的 "bee"， "bent" 中的 "be"                                  |
| ?            | 匹配上一个元素零次或一次。                  | "rai?n"       | "ran"、 "rain"                                                    |
| \{ n \}      | 匹配上一个元素恰好 n 次。                 | ",\\d\{3\}"   | "1,043\.6" 中的 ",043"， "9,876,543,210" 中的 ",876"、 ",543" 和 ",210" |
| \{ n ,\}     | 匹配上一个元素至少 n 次。                 | "\\d\{2,\}"   | "166"、 "29"、 "1930"                                              |
| \{ n , m \}  | 匹配上一个元素至少 n 次，但不多于 m 次。        | "\\d\{3,5\}"  | "166"， "17668"， "193024" 中的 "19302"                              |
| \*?          | 匹配上一个元素零次或多次，但次数尽可能少。          | \\d\*?\\\.\\d | "\.0"、 "19\.9"、 "219\.9"                                         |
| \+?          | 匹配上一个元素一次或多次，但次数尽可能少。          | "be\+?"       | "been" 中的 "be"， "bent" 中的 "be"                                   |
| ??           | 匹配上一个元素零次或一次，但次数尽可能少。          | "rai??n"      | "ran"、 "rain"                                                    |
| \{ n \}?     | 匹配前导元素恰好 n 次。                  | ",\\d\{3\}?"  | "1,043\.6" 中的 ",043"， "9,876,543,210" 中的 ",876"、 ",543" 和 ",210" |
| \{ n ,\}?    | 匹配上一个元素至少 n 次，但次数尽可能少。         | "\\d\{2,\}?"  | "166"、 "29" 和 "1930"                                             |
| \{ n , m \}? | 匹配上一个元素的次数介于 n 和 m 之间，但次数尽可能少。 | "\\d\{3,5\}?" | "166"， "17668"， "193024" 中的 "193" 和 "024"                        |

### 反向引用构造

反向引用允许在同一正则表达式中随后标识以前匹配的子表达式。

下表列出了反向引用构造：

| 反向引用构造      | 描述                 | 模式                        | 匹配             |
|-------------|--------------------|---------------------------|----------------|
| \\ number   | 反向引用。 匹配编号子表达式的值。  | \(\\w\)\\1                | "seek" 中的 "ee" |
| \\k< name > | 命名反向引用。 匹配命名表达式的值。 | \(?< char>\\w\)\\k< char> | "seek" 中的 "ee" |

### 备用构造

备用构造用于修改正则表达式以启用 either/or 匹配。

下表列出了备用构造：

| 备用构造                            | 描述                                                                      | 模式                                              | 匹配                                                                   |
|---------------------------------|-------------------------------------------------------------------------|-------------------------------------------------|----------------------------------------------------------------------|
| \|                              | 匹配以竖线 \(\|\) 字符分隔的任何一个元素。                                               | th\(e\|is\|at\)                                 | "this is the day\. " 中的 "the" 和 "this"                               |
| \(?\( expression \)yes \| no \) | 如果正则表达式模式由 expression 匹配指定，则匹配 yes；否则匹配可选的 no 部分。 expression 被解释为零宽度断言。 | \(?\(A\)A\\d\{2\}\\b\|\\b\\d\{3\}\\b\)          | "A10 C103 910" 中的 "A10" 和 "910"                                      |
| \(?\( name \)yes \| no \)       | 如果 name 或已命名或已编号的捕获组具有匹配，则匹配 yes；否则匹配可选的 no。                            | \(?< quoted>"\)?\(?\(quoted\)\.\+?"\|\\S\+\\s\) | "Dogs\.jpg "Yiska playing\.jpg"" 中的 Dogs\.jpg 和 "Yiska playing\.jpg" |

### 替换

替换是替换模式中使用的正则表达式。

下表列出了用于替换的字符：

| 字符        | 描述                   | 模式                                                | 替换模式                  | 输入字符串      | 结果字符串            |
|-----------|----------------------|---------------------------------------------------|-----------------------|------------|------------------|
| $number   | 替换按组 number 匹配的子字符串。 | \\b\(\\w\+\)\(\\s\)\(\\w\+\)\\b                   | $3$2$1                | "one two"  | "two one"        |
| $\{name\} | 替换按命名组 name 匹配的子字符串。 | \\b\(?< word1>\\w\+\)\(\\s\)\(?< word2>\\w\+\)\\b | $\{word2\} $\{word1\} | "one two"  | "two one"        |
| $$        | 替换字符"$"。             | \\b\(\\d\+\)\\s?USD                               | $$$1                  | "103 USD"  | "$103"           |
| $&        | 替换整个匹配项的一个副本。        | \(\\$\*\(\\d\*\(\\\.\+\\d\+\)?\)\{1\}\)           | \*\*$&                | "$1\.30"   | "\*\*$1\.30\*\*" |
| $\`       | 替换匹配前的输入字符串的所有文本。    | B\+                                               | $\`                   | "AABBCC"   | "AAAACC"         |
| $'        | 替换匹配后的输入字符串的所有文本。    | B\+                                               | $'                    | "AABBCC"   | "AACCCC"         |
| $\+       | 替换最后捕获的组。            | B\+\(C\+\)                                        | $\+                   | "AABBCCDD" | AACCDD           |
| $\_       | 替换整个输入字符串。           | B\+                                               | $\_                   | "AABBCC"   | "AAAABBCCCC"     |

### 杂项构造

下表列出了各种杂项构造：

| 构造                | 描述                          | 实例                                                      |
|-------------------|-----------------------------|---------------------------------------------------------|
| \(?imnsx\-imnsx\) | 在模式中间对诸如不区分大小写这样的选项进行设置或禁用。 | \\bA\(?i\)b\\w\+\\b 匹配 "ABA Able Act" 中的 "ABA" 和 "Able" |
| \(?\#注释\)         | 内联注释。该注释在第一个右括号处终止。         | \\bA\(?\#匹配以A开头的单词\)\\w\+\\b                            |
| \# \[行尾\]         | 该注释以非转义的 \# 开头，并继续到行的结尾。    | \(?x\)\\bA\\w\+\\b\#匹配以 A 开头的单词                         |

## Regex 类

Regex 类用于表示一个正则表达式。

下表列出了 Regex 类中一些常用的方法：

| 序号 | 方法 & 描述                                                                                                    |
|----|------------------------------------------------------------------------------------------------------------|
| 1  | public bool IsMatch\( string input \) 指示 Regex 构造函数中指定的正则表达式是否在指定的输入字符串中找到匹配项。                             |
| 2  | public bool IsMatch\( string input, int startat \) 指示 Regex 构造函数中指定的正则表达式是否在指定的输入字符串中找到匹配项，从字符串中指定的开始位置开始。 |
| 3  | public static bool IsMatch\( string input, string pattern \) 指示指定的正则表达式是否在指定的输入字符串中找到匹配项。                  |
| 4  | public MatchCollection Matches\( string input \) 在指定的输入字符串中搜索正则表达式的所有匹配项。                                  |
| 5  | public string Replace\( string input, string replacement \) 在指定的输入字符串中，把所有匹配正则表达式模式的所有匹配的字符串替换为指定的替换字符串。   |
| 6  | public string\[\] Split\( string input \) 把输入字符串分割为子字符串数组，根据在 Regex 构造函数中指定的正则表达式模式定义的位置进行分割。              |

如需了解 Regex 类的完整的属性列表，请参阅微软的 C# 文档。

## 实例 1

下面的实例匹配了以 'S' 开头的单词：

```C#
using System;
using System.Text.RegularExpressions;

namespace RegExApplication
{
   class Program
   {
      private static void showMatch(string text, string expr)
      {
         Console.WriteLine("The Expression: " + expr);
         MatchCollection mc = Regex.Matches(text, expr);
         foreach (Match m in mc)
         {
            Console.WriteLine(m);
         }
      }
      static void Main(string[] args)
      {
         string str = "A Thousand Splendid Suns";

         Console.WriteLine("Matching words that start with 'S': ");
         showMatch(str, @"\bS\S*");
         Console.ReadKey();
      }
   }
}
```

## 实例 2

下面的实例匹配了以 'm' 开头以 'e' 结尾的单词：

```C#
using System;
using System.Text.RegularExpressions;

namespace RegExApplication
{
   class Program
   {
      private static void showMatch(string text, string expr)
      {
         Console.WriteLine("The Expression: " + expr);
         MatchCollection mc = Regex.Matches(text, expr);
         foreach (Match m in mc)
         {
            Console.WriteLine(m);
         }
      }
      static void Main(string[] args)
      {
         string str = "make maze and manage to measure it";

         Console.WriteLine("Matching words start with 'm' and ends with 'e':");
         showMatch(str, @"\bm\S*e\b");
         Console.ReadKey();
      }
   }
}
```

## 实例 3

下面的实例替换掉多余的空格：

```C#
using System;  
using System.Text.RegularExpressions;  
  
namespace RegExApplication  
{  
   class Program  
   {  
      static void Main(string[] args)  
      {  
         string input = "Hello   World   ";  
         string pattern = "\s+";  
         string replacement = " ";  
         Regex rgx = new Regex(pattern);  
         string result = rgx.Replace(input, replacement);  
  
         Console.WriteLine("Original String: {0}", input);  
         Console.WriteLine("Replacement String: {0}", result);      
         Console.ReadKey();  
      }  
   }  
}
```

# C# 异常处理

异常是在程序执行期间出现的问题。C# 中的异常是对程序运行时出现的特殊情况的一种响应，比如尝试除以零。

异常提供了一种把程序控制权从某个部分转移到另一个部分的方式。C# 异常处理时建立在四个关键词之上的：**try**、**catch**、**finally** 和 **throw**。

  * **try**：一个 try 块标识了一个将被激活的特定的异常的代码块。后跟一个或多个 catch 块。
  * **catch**：程序通过异常处理程序捕获异常。catch 关键字表示异常的捕获。
  * **finally**：finally 块用于执行给定的语句，不管异常是否被抛出都会执行。例如，如果您打开一个文件，不管是否出现异常文件都要被关闭。
  * **throw**：当问题出现时，程序抛出一个异常。使用 throw 关键字来完成。

## 语法

假设一个块将出现异常，一个方法使用 try 和 catch 关键字捕获异常。try/catch 块内的代码为受保护的代码，使用 try/catch 语法如下所示：

```
try
{
   // 引起异常的语句
}
catch( ExceptionName e1 )
{
   // 错误处理代码
}
catch( ExceptionName e2 )
{
   // 错误处理代码
}
catch( ExceptionName eN )
{
   // 错误处理代码
}
finally
{
   // 要执行的语句
}
```

您可以列出多个 catch 语句捕获不同类型的异常，以防 try 块在不同的情况下生成多个异常。

## C# 中的异常类

C# 异常是使用类来表示的。C# 中的异常类主要是直接或间接地派生于 **System.Exception** 类。**System.ApplicationException** 和 **System.SystemException** 类是派生于 System.Exception 类的异常类。

**System.ApplicationException** 类支持由应用程序生成的异常。所以程序员定义的异常都应派生自该类。

**System.SystemException** 类是所有预定义的系统异常的基类。

下表列出了一些派生自 Sytem.SystemException 类的预定义的异常类：

| 异常类                                | 描述                      |
|------------------------------------|-------------------------|
| System\.IO\.IOException            | 处理 I/O 错误。              |
| System\.IndexOutOfRangeException   | 处理当方法指向超出范围的数组索引时生成的错误。 |
| System\.ArrayTypeMismatchException | 处理当数组类型不匹配时生成的错误。       |
| System\.NullReferenceException     | 处理当依从一个空对象时生成的错误。       |
| System\.DivideByZeroException      | 处理当除以零时生成的错误。           |
| System\.InvalidCastException       | 处理在类型转换期间生成的错误。         |
| System\.OutOfMemoryException       | 处理空闲内存不足生成的错误。          |
| System\.StackOverflowException     | 处理栈溢出生成的错误。             |

## 异常处理

C# 以 try 和 catch 块的形式提供了一种结构化的异常处理方案。使用这些块，把核心程序语句与错误处理语句分离开。

这些错误处理块是使用 **try**、**catch** 和 **finally** 关键字实现的。下面是一个当除以零时抛出异常的实例：

```C#
using System;
namespace ErrorHandlingApplication
{
    class DivNumbers
    {
        int result;
        DivNumbers()
        {
            result = 0;
        }
        public void division(int num1, int num2)
        {
            try
            {
                result = num1 / num2;
            }
            catch (DivideByZeroException e)
            {
                Console.WriteLine("Exception caught: {0}", e);
            }
            finally
            {
                Console.WriteLine("Result: {0}", result);
            }

        }
        static void Main(string[] args)
        {
            DivNumbers d = new DivNumbers();
            d.division(25, 0);
            Console.ReadKey();
        }
    }
}
```

## 创建用户自定义异常

您也可以定义自己的异常。用户自定义的异常类是派生自 **ApplicationException** 类。下面的实例演示了这点：

```C#
using System;
namespace UserDefinedException
{
   class TestTemperature
   {
      static void Main(string[] args)
      {
         Temperature temp = new Temperature();
         try
         {
            temp.showTemp();
         }
         catch(TempIsZeroException e)
         {
            Console.WriteLine("TempIsZeroException: {0}", e.Message);
         }
         Console.ReadKey();
      }
   }
}
public class TempIsZeroException: ApplicationException
{
   public TempIsZeroException(string message): base(message)
   {
   }
}
public class Temperature
{
   int temperature = 0;
   public void showTemp()
   {
      if(temperature == 0)
      {
         throw (new TempIsZeroException("Zero Temperature found"));
      }
      else
      {
         Console.WriteLine("Temperature: {0}", temperature);
      }
   }
}
```

## 抛出对象

如果异常是直接或间接派生自 **System.Exception** 类，您可以抛出一个对象。您可以在 catch 块中使用 throw 语句来抛出当前的对象，如下所示：

```
Catch(Exception e)
{
   ...
   Throw e
}
```

# C# 文件的输入与输出

一个 **文件** 是一个存储在磁盘中带有指定名称和目录路径的数据集合。当打开文件进行读写时，它变成一个 **流**。

从根本上说，流是通过通信路径传递的字节序列。有两个主要的流：**输入流** 和 **输出流**。**输入流**用于从文件读取数据（读操作），**输出流**用于向文件写入数据（写操作）。

## C# I/O 类

System.IO 命名空间有各种不同的类，用于执行各种文件操作，如创建和删除文件、读取或写入文件，关闭文件等。

下表列出了一些 System.IO 命名空间中常用的非抽象类：

| I/O 类          | 描述                |
|----------------|-------------------|
| BinaryReader   | 从二进制流读取原始数据。      |
| BinaryWriter   | 以二进制格式写入原始数据。     |
| BufferedStream | 字节流的临时存储。         |
| Directory      | 有助于操作目录结构。        |
| DirectoryInfo  | 用于对目录执行操作。        |
| DriveInfo      | 提供驱动器的信息。         |
| File           | 有助于处理文件。          |
| FileInfo       | 用于对文件执行操作。        |
| FileStream     | 用于文件中任何位置的读写。     |
| MemoryStream   | 用于随机访问存储在内存中的数据流。 |
| Path           | 对路径信息执行操作。        |
| StreamReader   | 用于从字节流中读取字符。      |
| StreamWriter   | 用于向一个流中写入字符。      |
| StringReader   | 用于读取字符串缓冲区。       |
| StringWriter   | 用于写入字符串缓冲区。       |

## FileStream 类

System.IO 命名空间中的 **FileStream** 类有助于文件的读写与关闭。该类派生自抽象类 Stream。

您需要创建一个 **FileStream** 对象来创建一个新的文件，或打开一个已有的文件。创建 **FileStream** 对象的语法如下：

```
FileStream <object_name> = new FileStream( <file_name>,
<FileMode Enumerator>, <FileAccess Enumerator>, <FileShare Enumerator>);
```

例如，创建一个 FileStream 对象 **F** 来读取名为 **sample.txt** 的文件：

```C#
FileStream F = new FileStream("sample.txt", FileMode.Open, FileAccess.Read, FileShare.Read);
```

参数描述

FileMode

**FileMode** 枚举定义了各种打开文件的方法。FileMode 枚举的成员有：

  * **Append**：打开一个已有的文件，并将光标放置在文件的末尾。如果文件不存在，则创建文件。
  * **Create**：创建一个新的文件。如果文件已存在，则删除旧文件，然后创建新文件。
  * **CreateNew**：指定操作系统应创建一个新的文件。如果文件已存在，则抛出异常。
  * **Open**：打开一个已有的文件。如果文件不存在，则抛出异常。
  * **OpenOrCreate**：指定操作系统应打开一个已有的文件。如果文件不存在，则用指定的名称创建一个新的文件打开。
  * **Truncate**：打开一个已有的文件，文件一旦打开，就将被截断为零字节大小。然后我们可以向文件写入全新的数据，但是保留文件的初始创建日期。如果文件不存在，则抛出异常。

FileAccess

**FileAccess** 枚举的成员有：**Read**、**ReadWrite** 和 **Write**。

FileShare

**FileShare** 枚举的成员有：

  * **Inheritable**：允许文件句柄可由子进程继承。Win32 不直接支持此功能。
  * **None**：谢绝共享当前文件。文件关闭前，打开该文件的任何请求（由此进程或另一进程发出的请求）都将失败。 
  * **Read**：允许随后打开文件读取。如果未指定此标志，则文件关闭前，任何打开该文件以进行读取的请求（由此进程或另一进程发出的请求）都将失败。但是，即使指定了此标志，仍可能需要附加权限才能够访问该文件。
  * **ReadWrite**：允许随后打开文件读取或写入。如果未指定此标志，则文件关闭前，任何打开该文件以进行读取或写入的请求（由此进程或另一进程发出）都将失败。但是，即使指定了此标志，仍可能需要附加权限才能够访问该文件。 
  * **Write**：允许随后打开文件写入。如果未指定此标志，则文件关闭前，任何打开该文件以进行写入的请求（由此进程或另一进过程发出的请求）都将失败。但是，即使指定了此标志，仍可能需要附加权限才能够访问该文件。 
  * **Delete**：允许随后删除文件。

## 实例

下面的程序演示了 **FileStream** 类的用法：

```
using System;
using System.IO;

namespace FileIOApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            FileStream F = new FileStream("test.dat", 
            FileMode.OpenOrCreate, FileAccess.ReadWrite);

            for (int i = 1; i <= 20; i++)
            {
                F.WriteByte((byte)i);
            }

            F.Position = 0;

            for (int i = 0; i <= 20; i++)
            {
                Console.Write(F.ReadByte() + " ");
            }
            F.Close();
            Console.ReadKey();
        }
    }
}
```

## C# 高级文件操作

上面的实例演示了 C# 中简单的文件操作。但是，要充分利用 C# System.IO 类的强大功能，您需要知道这些类常用的属性和方法。

### C# 文本文件的读写

**StreamReader** 和 **StreamWriter** 类用于文本文件的数据读写。这些类从抽象基类 Stream 继承，Stream 支持文件流的字节读写。

#### StreamReader 类

**StreamReader** 类继承自抽象基类 TextReader，表示阅读器读取一系列字符。

下表列出了 **StreamReader** 类中一些常用的**方法**：

| 序号 | 方法 & 描述                                                               |
|----|-----------------------------------------------------------------------|
| 1  | public override void Close\(\)关闭 StreamReader 对象和基础流，并释放任何与读者相关的系统资源。 |
| 2  | public override int Peek\(\)返回下一个可用的字符，但不使用它。                         |
| 3  | public override int Read\(\)从输入流中读取下一个字符，并把字符位置往前移一个字符。               |

如需查看完整的方法列表，请访问微软的 C# 文档。

#### 实例

下面的实例演示了读取名为 Jamaica.txt 的文件。文件如下：

```
Down the way where the nights are gay
And the sun shines daily on the mountain top
I took a trip on a sailing ship
And when I reached Jamaica
I made a stop
```

```C#
using System;
using System.IO;

namespace FileApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            try
            {
                // 创建一个 StreamReader 的实例来读取文件 
                // using 语句也能关闭 StreamReader
                using (StreamReader sr = new StreamReader("c:/jamaica.txt"))
                {
                    string line;
                   
                    // 从文件读取并显示行，直到文件的末尾 
                    while ((line = sr.ReadLine()) != null)
                    {
                        Console.WriteLine(line);
                    }
                }
            }
            catch (Exception e)
            {
                // 向用户显示出错消息
                Console.WriteLine("The file could not be read:");
                Console.WriteLine(e.Message);
            }
            Console.ReadKey();
        }
    }
}
```

当您编译和执行上面的程序时，它会显示文件的内容。

#### StreamWriter 类

**StreamWriter** 类继承自抽象类 TextWriter，表示编写器写入一系列字符。

下表列出了 **StreamWriter** 类中一些常用的**方法**：

| 序号 | 方法 & 描述                                                                          |
|----|----------------------------------------------------------------------------------|
| 1  | public override void Close\(\)关闭当前的 StreamWriter 对象和基础流。                         |
| 2  | public override void Flush\(\)清理当前编写器的所有缓冲区，使得所有缓冲数据写入基础流。                       |
| 3  | public virtual void Write\(bool value\)把一个布尔值的文本表示形式写入到文本字符串或流。（继承自 TextWriter。） |
| 4  | public override void Write\( char value \) 把一个字符写入到流。                            |
| 5  | public virtual void Write\( decimal value \) 把一个十进制值的文本表示形式写入到文本字符串或流。           |
| 6  | public virtual void Write\( double value \) 把一个 8 字节浮点值的文本表示形式写入到文本字符串或流。        |
| 7  | public virtual void Write\( int value \) 把一个 4 字节有符号整数的文本表示形式写入到文本字符串或流。         |
| 8  | public override void Write\( string value \) 把一个字符串写入到流。                         |
| 9  | public virtual void WriteLine\(\)把行结束符写入到文本字符串或流。                                |

如需查看完整的方法列表，请访问微软的 C# 文档。

#### 实例

下面的实例演示了使用 StreamWriter 类向文件写入文本数据：

```C#
using System;
using System.IO;

namespace FileApplication
{
    class Program
    {
        static void Main(string[] args)
        {

            string[] names = new string[] {"Zara Ali", "Nuha Ali"};
            using (StreamWriter sw = new StreamWriter("names.txt"))
            {
                foreach (string s in names)
                {
                    sw.WriteLine(s);

                }
            }

            // 从文件中读取并显示每行
            string line = "";
            using (StreamReader sr = new StreamReader("names.txt"))
            {
                while ((line = sr.ReadLine()) != null)
                {
                    Console.WriteLine(line);
                }
            }
            Console.ReadKey();
        }
    }
}
```

### C# 二进制文件的读写

**BinaryReader** 和 **BinaryWriter** 类用于二进制文件的读写。

#### BinaryReader 类

**BinaryReader** 类用于从文件读取二进制数据。一个 **BinaryReader** 对象通过向它的构造函数传递 **FileStream** 对象而被创建。

下表列出了 **BinaryReader** 类中一些常用的**方法**：

| 序号 | 方法 & 描述                                                                                                      |
|----|--------------------------------------------------------------------------------------------------------------|
| 1  | public override void Close\(\)关闭 BinaryReader 对象和基础流。                                                        |
| 2  | public virtual int Read\(\)从基础流中读取字符，并把流的当前位置往前移。                                                            |
| 3  | public virtual bool ReadBoolean\(\)从当前流中读取一个布尔值，并把流的当前位置往前移一个字节。                                             |
| 4  | public virtual byte ReadByte\(\)从当前流中读取下一个字节，并把流的当前位置往前移一个字节。                                                |
| 5  | public virtual byte\[\] ReadBytes\( int count \) 从当前流中读取指定数目的字节到一个字节数组中，并把流的当前位置往前移指定数目的字节。                  |
| 6  | public virtual char ReadChar\(\)从当前流中读取下一个字节，并把流的当前位置按照所使用的编码和从流中读取的指定的字符往前移。                                |
| 7  | public virtual char\[\] ReadChars\( int count \)从当前流中读取指定数目的字节，在一个字符数组中返回数组，并把流的当前位置按照所使用的编码和从流中读取的指定的字符往前移。 |
| 8  | public virtual double ReadDouble\(\)从当前流中读取一个 8 字节浮点值，并把流的当前位置往前移八个字节。                                       |
| 9  | public virtual int ReadInt32\(\)从当前流中读取一个 4 字节有符号整数，并把流的当前位置往前移四个字节。                                         |
| 10 | public virtual string ReadString\(\) 从当前流中读取一个字符串。字符串以长度作为前缀，同时编码为一个七位的整数。                                   |

如需查看完整的方法列表，请访问微软的 C# 文档。

#### BinaryWriter 类

**BinaryWriter** 类用于向文件写入二进制数据。一个 **BinaryWriter** 对象通过向它的构造函数传递 **FileStream** 对象而被创建。

下表列出了 **BinaryWriter** 类中一些常用的**方法**：

| 序号 | 方法 & 描述                                                                                                              |
|----|----------------------------------------------------------------------------------------------------------------------|
| 1  | public override void Close\(\)关闭 BinaryWriter 对象和基础流。                                                                |
| 2  | public virtual void Flush\(\)清理当前编写器的所有缓冲区，使得所有缓冲数据写入基础设备。                                                           |
| 3  | public virtual long Seek\( int offset, SeekOrigin origin \) 设置当前流内的位置。                                               |
| 4  | public virtual void Write\( bool value \) 把一个单字节的布尔值写入到当前流中，0 表示 false，1 表示 true。                                    |
| 5  | public virtual void Write\( byte value \) 把一个无符号字节写入到当前流中，并把流的位置往前移一个字节。                                             |
| 6  | public virtual void Write\( byte\[\] buffer \) 把一个字节数组写入到基础流中。                                                       |
| 7  | public virtual void Write\( char ch \) 把一个 Unicode 字符写入到当前流中，并把流的当前位置按照所使用的编码和要写入到流中的指定的字符往前移。                       |
| 8  | public virtual void Write\( char\[\] chars \) 把一个字符数组写入到当前流中，并把流的当前位置按照所使用的编码和要写入到流中的指定的字符往前移。                       |
| 9  | public virtual void Write\( double value \) 把一个 8 字节浮点值写入到当前流中，并把流位置往前移八个字节。                                         |
| 10 | public virtual void Write\( int value \) 把一个 4 字节有符号整数写入到当前流中，并把流位置往前移四个字节。                                          |
| 11 | public virtual void Write\( string value \) 把一个以长度为前缀的字符串写入到 BinaryWriter 的当前编码的流中，并把流的当前位置按照所使用的编码和要写入到流中的指定的字符往前移。 |

如需查看完整的方法列表，请访问微软的 C# 文档。

#### 实例

下面的实例演示了读取和写入二进制数据：

```C#
using System;
using System.IO;

namespace BinaryFileApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            BinaryWriter bw;
            BinaryReader br;
            int i = 25;
            double d = 3.14157;
            bool b = true;
            string s = "I am happy";
            // 创建文件
            try
            {
                bw = new BinaryWriter(new FileStream("mydata",
                FileMode.Create));
            }
            catch (IOException e)
            {
                Console.WriteLine(e.Message + "\n Cannot create file.");
                return;
            }
            // 写入文件
            try
            {
                bw.Write(i);
                bw.Write(d);
                bw.Write(b);
                bw.Write(s);
            }
            catch (IOException e)
            {
                Console.WriteLine(e.Message + "\n Cannot write to file.");
                return;
            }

            bw.Close();
            // 读取文件
            try
            {
                br = new BinaryReader(new FileStream("mydata",
                FileMode.Open));
            }
            catch (IOException e)
            {
                Console.WriteLine(e.Message + "\n Cannot open file.");
                return;
            }
            try
            {
                i = br.ReadInt32();
                Console.WriteLine("Integer data: {0}", i);
                d = br.ReadDouble();
                Console.WriteLine("Double data: {0}", d);
                b = br.ReadBoolean();
                Console.WriteLine("Boolean data: {0}", b);
                s = br.ReadString();
                Console.WriteLine("String data: {0}", s);
            }
            catch (IOException e)
            {
                Console.WriteLine(e.Message + "\n Cannot read from file.");
                return;
            }
            br.Close();
            Console.ReadKey();
        }
    }
}
```

### C# Windows 文件系统的操作

C# 允许您使用各种目录和文件相关的类来操作目录和文件，比如 **DirectoryInfo** 类和 **FileInfo** 类。

#### DirectoryInfo 类

**DirectoryInfo** 类派生自 **FileSystemInfo** 类。它提供了各种用于创建、移动、浏览目录和子目录的方法。该类不能被继承。

下表列出了 **DirectoryInfo** 类中一些常用的**属性**：

| 序号 | 属性 & 描述                          |
|----|----------------------------------|
| 1  | Attributes获取当前文件或目录的属性。          |
| 2  | CreationTime获取当前文件或目录的创建时间。      |
| 3  | Exists获取一个表示目录是否存在的布尔值。          |
| 4  | Extension获取表示文件存在的字符串。           |
| 5  | FullName获取目录或文件的完整路径。            |
| 6  | LastAccessTime获取当前文件或目录最后被访问的时间。 |
| 7  | Name获取该 DirectoryInfo 实例的名称。     |

下表列出了 **DirectoryInfo** 类中一些常用的**方法**：

| 序号 | 方法 & 描述                                                                                                  |
|----|----------------------------------------------------------------------------------------------------------|
| 1  | public void Create\(\)创建一个目录。                                                                            |
| 2  | public DirectoryInfo CreateSubdirectory\( string path \) 在指定的路径上创建子目录。指定的路径可以是相对于 DirectoryInfo 类的实例的路径。 |
| 3  | public override void Delete\(\)如果为空的，则删除该 DirectoryInfo。                                                 |
| 4  | public DirectoryInfo\[\] GetDirectories\(\)返回当前目录的子目录。                                                   |
| 5  | public FileInfo\[\] GetFiles\(\)从当前目录返回文件列表。                                                             |
如需查看完整的属性和方法列表，请访问微软的 C# 文档。

## FileInfo 类

**FileInfo** 类派生自 **FileSystemInfo** 类。它提供了用于创建、复制、删除、移动、打开文件的属性和方法，且有助于 FileStream 对象的创建。该类不能被继承。

下表列出了 **FileInfo** 类中一些常用的**属性**：

| 序号 | 属性 & 描述                       |
|----|-------------------------------|
| 1  | Attributes获取当前文件的属性。          |
| 2  | CreationTime获取当前文件的创建时间。      |
| 3  | Directory获取文件所属目录的一个实例。       |
| 4  | Exists获取一个表示文件是否存在的布尔值。       |
| 5  | Extension获取表示文件存在的字符串。        |
| 6  | FullName获取文件的完整路径。            |
| 7  | LastAccessTime获取当前文件最后被访问的时间。 |
| 8  | LastWriteTime获取文件最后被写入的时间。    |
| 9  | Length获取当前文件的大小，以字节为单位。       |
| 10 | Name获取文件的名称。                  |

下表列出了 **FileInfo** 类中一些常用的**方法**：

| 序号 | 方法 & 描述                                                                                                                               |
|----|---------------------------------------------------------------------------------------------------------------------------------------|
| 1  | public StreamWriter AppendText\(\)创建一个 StreamWriter，追加文本到由 FileInfo 的实例表示的文件中。                                                        |
| 2  | public FileStream Create\(\)创建一个文件。                                                                                                   |
| 3  | public override void Delete\(\)永久删除一个文件。                                                                                              |
| 4  | public void MoveTo\( string destFileName \) 移动一个指定的文件到一个新的位置，提供选项来指定新的文件名。                                                            |
| 5  | public FileStream Open\( FileMode mode \) 以指定的模式打开一个文件。                                                                               |
| 6  | public FileStream Open\( FileMode mode, FileAccess access \) 以指定的模式，使用 read、write 或 read/write 访问，来打开一个文件。                            |
| 7  | public FileStream Open\( FileMode mode, FileAccess access, FileShare share \) 以指定的模式，使用 read、write 或 read/write 访问，以及指定的分享选项，来打开一个文件。 |
| 8  | public FileStream OpenRead\(\)创建一个只读的 FileStream。                                                                                     |
| 9  | public FileStream OpenWrite\(\)创建一个只写的 FileStream。                                                                                    |
如需查看完整的属性和方法列表，请访问微软的 C# 文档。

## 实例

下面的实例演示了上面提到的类的用法：

```C#
using System;
using System.IO;

namespace WindowsFileApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            // 创建一个 DirectoryInfo 对象
            DirectoryInfo mydir = new DirectoryInfo(@"c:\Windows");

            // 获取目录中的文件以及它们的名称和大小
            FileInfo [] f = mydir.GetFiles();
            foreach (FileInfo file in f)
            {
                Console.WriteLine("File Name: {0} Size: {1}",
                    file.Name, file.Length);
            }
            Console.ReadKey();
        }
    }
}
```

当您编译和执行上面的程序时，它会显示文件的名称及它们在 Windows 目录中的大小。

# C# 特性（Attribute）

**特性（Attribute）**是用于在运行时传递程序中各种元素（比如类、方法、结构、枚举、组件等）的行为信息的声明性标签。您可以通过使用特性向程序添加声明性信息。一个声明性标签是通过放置在它所应用的元素前面的方括号（[ ]）来描述的。

特性（Attribute）用于添加元数据，如编译器指令和注释、描述、方法、类等其他信息。.Net 框架提供了两种类型的特性：_预定义_特性和_自定义_特性。

## 规定特性（Attribute）

规定特性（Attribute）的语法如下：

```
[attribute(positional_parameters, name_parameter = value, ...)] element
```

特性（Attribute）的名称和值是在方括号内规定的，放置在它所应用的元素之前。positional_parameters 规定必需的信息，name_parameter 规定可选的信息。

## 预定义特性（Attribute）

.Net 框架提供了三种预定义特性：

  * AttributeUsage
  * Conditional
  * Obsolete

### AttributeUsage

预定义特性 **AttributeUsage** 描述了如何使用一个自定义特性类。它规定了特性可应用到的项目的类型。

规定该特性的语法如下：

```
[AttributeUsage(
   validon,
   AllowMultiple=allowmultiple,
   Inherited=inherited
)]
```

其中：

  * 参数 validon 规定特性可被放置的语言元素。它是枚举器 _AttributeTargets_ 的值的组合。默认值是 _AttributeTargets.All_。
  * 参数 _allowmultiple_（可选的）为该特性的 _AllowMultiple_ 属性（property）提供一个布尔值。如果为 true，则该特性是多用的。默认值是 false（单用的）。
  * 参数 _inherited_（可选的）为该特性的 _Inherited_ 属性（property）提供一个布尔值。如果为 true，则该特性可被派生类继承。默认值是 false（不被继承）。

例如：

```
[AttributeUsage(AttributeTargets.Class |
AttributeTargets.Constructor |
AttributeTargets.Field |
AttributeTargets.Method |
AttributeTargets.Property, 
AllowMultiple = true)]
```

### Conditional

这个预定义特性标记了一个条件方法，其执行依赖于指定的预处理标识符。

它会引起方法调用的条件编译，取决于指定的值，比如 **Debug** 或 **Trace**。例如，当调试代码时显示变量的值。

规定该特性的语法如下：

```C#
[Conditional(
   conditionalSymbol
)]
```

例如：

```
[Conditional("DEBUG")]
```

下面的实例演示了该特性：

```C#
#define DEBUG
using System;
using System.Diagnostics;
public class Myclass
{
    [Conditional("DEBUG")]
    public static void Message(string msg)
    {
        Console.WriteLine(msg);
    }
}
class Test
{
    static void function1()
    {
        Myclass.Message("In Function 1.");
        function2();
    }
    static void function2()
    {
        Myclass.Message("In Function 2.");
    }
    public static void Main()
    {
        Myclass.Message("In Main function.");
        function1();
        Console.ReadKey();
    }
}
```

### Obsolete

这个预定义特性标记了不应被使用的程序实体。它可以让您通知编译器丢弃某个特定的目标元素。例如，当一个新方法被用在一个类中，但是您仍然想要保持类中的旧方法，您可以通过显示一个应该使用新方法，而不是旧方法的消息，来把它标记为 obsolete（过时的）。

规定该特性的语法如下：

```
[Obsolete( message )] [Obsolete( message, iserror )]
```

其中：

  * 参数 _message_ ，是一个字符串，描述项目为什么过时以及该替代使用什么。
  * 参数 _iserror_ ，是一个布尔值。如果该值为 true，编译器应把该项目的使用当作一个错误。默认值是 false（编译器生成一个警告）。

下面的实例演示了该特性：

```C#
using System;
public class MyClass
{
   [Obsolete("Don't use OldMethod, use NewMethod instead", true)]
   static void OldMethod()
   { 
      Console.WriteLine("It is the old method");
   }
   static void NewMethod()
   { 
      Console.WriteLine("It is the new method"); 
   }
   public static void Main()
   {
      OldMethod();
   }
}
```

当您尝试编译该程序时，编译器会给出一个错误消息说明：

```
Don't use OldMethod, use NewMethod instead
```

## 创建自定义特性（Attribute）

.Net 框架允许创建自定义特性，用于存储声明性的信息，且可在运行时被检索。该信息根据设计标准和应用程序需要，可与任何目标元素相关。

创建并使用自定义特性包含四个步骤：

  * 声明自定义特性
  * 构建自定义特性
  * 在目标程序元素上应用自定义特性
  * 通过反射访问特性

最后一个步骤包含编写一个简单的程序来读取元数据以便查找各种符号。元数据是用于描述其他数据的数据和信息。该程序应使用反射来在运行时访问特性。我们将在下一章详细讨论这点。

### 声明自定义特性

一个新的自定义特性应派生自 **System.Attribute** 类。例如：

```C#
// 一个自定义特性 BugFix 被赋给类及其成员
[AttributeUsage(AttributeTargets.Class |
AttributeTargets.Constructor |
AttributeTargets.Field |
AttributeTargets.Method |
AttributeTargets.Property,
AllowMultiple = true)]

public class DeBugInfo : System.Attribute
```

在上面的代码中，我们已经声明了一个名为 _DeBugInfo_ 的自定义特性。

### 构建自定义特性

让我们构建一个名为 _DeBugInfo_ 的自定义特性，该特性将存储调试程序获得的信息。它存储下面的信息：

  * bug 的代码编号
  * 辨认该 bug 的开发人员名字
  * 最后一次审查该代码的日期
  * 一个存储了开发人员标记的字符串消息

我们的 _DeBugInfo_ 类将带有三个用于存储前三个信息的私有属性（property）和一个用于存储消息的公有属性（property）。所以 bug 编号、开发人员名字和审查日期将是 DeBugInfo 类的必需的定位（ positional）参数，消息将是一个可选的命名（named）参数。

每个特性必须至少有一个构造函数。必需的定位（ positional）参数应通过构造函数传递。下面的代码演示了 _DeBugInfo_ 类：

```C#
// 一个自定义特性 BugFix 被赋给类及其成员
[AttributeUsage(AttributeTargets.Class |
AttributeTargets.Constructor |
AttributeTargets.Field |
AttributeTargets.Method |
AttributeTargets.Property,
AllowMultiple = true)]

public class DeBugInfo : System.Attribute
{
  private int bugNo;
  private string developer;
  private string lastReview;
  public string message;

  public DeBugInfo(int bg, string dev, string d)
  {
      this.bugNo = bg;
      this.developer = dev;
      this.lastReview = d;
  }

  public int BugNo
  {
      get
      {
          return bugNo;
      }
  }
  public string Developer
  {
      get
      {
          return developer;
      }
  }
  public string LastReview
  {
      get
      {
          return lastReview;
      }
  }
  public string Message
  {
      get
      {
          return message;
      }
      set
      {
          message = value;
      }
  }
}
```

### 应用自定义特性

通过把特性放置在紧接着它的目标之前，来应用该特性：

```C#
[DeBugInfo(45, "Zara Ali", "12/8/2012", Message = "Return type mismatch")]  
[DeBugInfo(49, "Nuha Ali", "10/10/2012", Message = "Unused variable")]  
class Rectangle  
{  
  // 成员变量  
  protected double length;  
  protected double width;  
  public Rectangle(double l, double w)  
  {  
      length = l;  
      width = w;  
  }  
  [DeBugInfo(55, "Zara Ali", "19/10/2012",  
  Message = "Return type mismatch")]  
  public double GetArea()  
  {  
      return length * width;  
  }  
  [DeBugInfo(56, "Zara Ali", "19/10/2012")]  
  public void Display()  
  {  
      Console.WriteLine("Length: {0}", length);  
      Console.WriteLine("Width: {0}", width);  
      Console.WriteLine("Area: {0}", GetArea());  
  }  
}
```

在下一章中，我们将使用 Reflection 类对象来检索这些信息。

# C# 反射（Reflection）

反射指程序可以访问、检测和修改它本身状态或行为的一种能力。

程序集包含模块，而模块包含类型，类型又包含成员。反射则提供了封装程序集、模块和类型的对象。

您可以使用反射动态地创建类型的实例，将类型绑定到现有对象，或从现有对象中获取类型。然后，可以调用类型的方法或访问其字段和属性。 

### 优缺点

优点：

  * 1、反射提高了程序的灵活性和扩展性。 
  * 2、降低耦合性，提高自适应能力。 
  * 3、它允许程序创建和控制任何类的对象，无需提前硬编码目标类。

缺点：

  * 1、性能问题：使用反射基本上是一种解释操作，用于字段和方法接入时要远慢于直接代码。因此反射机制主要应用在对灵活性和拓展性要求很高的系统框架上，普通程序不建议使用。 
  * 2、使用反射会模糊程序内部逻辑；程序员希望在源代码中看到程序的逻辑，反射却绕过了源代码的技术，因而会带来维护的问题，反射代码比相应的直接代码更复杂。

## 反射（Reflection）的用途

反射（Reflection）有下列用途：

  * 它允许在运行时查看特性（attribute）信息。
  * 它允许审查集合中的各种类型，以及实例化这些类型。
  * 它允许延迟绑定的方法和属性（property）。
  * 它允许在运行时创建新类型，然后使用这些类型执行一些任务。

## 查看元数据

我们已经在上面的章节中提到过，使用反射（Reflection）可以查看特性（attribute）信息。

**System.Reflection** 类的 **MemberInfo** 对象需要被初始化，用于发现与类相关的特性（attribute）。为了做到这点，您可以定义目标类的一个对象，如下：

```C#
System.Reflection.MemberInfo info = typeof(MyClass);
```

下面的程序演示了这点：

```C#
using System;

[AttributeUsage(AttributeTargets.All)]
public class HelpAttribute : System.Attribute
{
   public readonly string Url;

   public string Topic  // Topic 是一个命名（named）参数
   {
      get
      {
         return topic;
      }
      set
      {

         topic = value;
      }
   }

   public HelpAttribute(string url)  // url 是一个定位（positional）参数
   {
      this.Url = url;
   }

   private string topic;
}
[HelpAttribute("Information on the class MyClass")]
class MyClass
{
}

namespace AttributeAppl
{
   class Program
   {
      static void Main(string[] args)
      {
         System.Reflection.MemberInfo info = typeof(MyClass);
         object[] attributes = info.GetCustomAttributes(true);
         for (int i = 0; i < attributes.Length; i++)
         {
            System.Console.WriteLine(attributes[i]);
         }
         Console.ReadKey();

      }
   }
}
```

当上面的代码被编译和执行时，它会显示附加到类 _MyClass_ 上的自定义特性：

```
HelpAttribute
```

## 实例

在本实例中，我们将使用在上一章中创建的 _DeBugInfo_ 特性，并使用反射（Reflection）来读取 _Rectangle_ 类中的元数据。

```C#
using System;
using System.Reflection;
namespace BugFixApplication
{
   // 一个自定义特性 BugFix 被赋给类及其成员
   [AttributeUsage(AttributeTargets.Class |
   AttributeTargets.Constructor |
   AttributeTargets.Field |
   AttributeTargets.Method |
   AttributeTargets.Property,
   AllowMultiple = true)]

   public class DeBugInfo : System.Attribute
   {
      private int bugNo;
      private string developer;
      private string lastReview;
      public string message;

      public DeBugInfo(int bg, string dev, string d)
      {
         this.bugNo = bg;
         this.developer = dev;
         this.lastReview = d;
      }

      public int BugNo
      {
         get
         {
            return bugNo;
         }
      }
      public string Developer
      {
         get
         {
            return developer;
         }
      }
      public string LastReview
      {
         get
         {
            return lastReview;
         }
      }
      public string Message
      {
         get
         {
            return message;
         }
         set
         {
            message = value;
         }
      }
   }
   [DeBugInfo(45, "Zara Ali", "12/8/2012",
        Message = "Return type mismatch")]
   [DeBugInfo(49, "Nuha Ali", "10/10/2012",
        Message = "Unused variable")]
   class Rectangle
   {
      // 成员变量
      protected double length;
      protected double width;
      public Rectangle(double l, double w)
      {
         length = l;
         width = w;
      }
      [DeBugInfo(55, "Zara Ali", "19/10/2012",
           Message = "Return type mismatch")]
      public double GetArea()
      {
         return length * width;
      }
      [DeBugInfo(56, "Zara Ali", "19/10/2012")]
      public void Display()
      {
         Console.WriteLine("Length: {0}", length);
         Console.WriteLine("Width: {0}", width);
         Console.WriteLine("Area: {0}", GetArea());
      }
   }//end class Rectangle  
   
   class ExecuteRectangle
   {
      static void Main(string[] args)
      {
         Rectangle r = new Rectangle(4.5, 7.5);
         r.Display();
         Type type = typeof(Rectangle);
         // 遍历 Rectangle 类的特性
         foreach (Object attributes in type.GetCustomAttributes(false))
         {
            DeBugInfo dbi = (DeBugInfo)attributes;
            if (null != dbi)
            {
               Console.WriteLine("Bug no: {0}", dbi.BugNo);
               Console.WriteLine("Developer: {0}", dbi.Developer);
               Console.WriteLine("Last Reviewed: {0}",
                                        dbi.LastReview);
               Console.WriteLine("Remarks: {0}", dbi.Message);
            }
         }
         
         // 遍历方法特性
         foreach (MethodInfo m in type.GetMethods())
         {
            foreach (Attribute a in m.GetCustomAttributes(true))
            {
               DeBugInfo dbi = (DeBugInfo)a;
               if (null != dbi)
               {
                  Console.WriteLine("Bug no: {0}, for Method: {1}",
                                                dbi.BugNo, m.Name);
                  Console.WriteLine("Developer: {0}", dbi.Developer);
                  Console.WriteLine("Last Reviewed: {0}",
                                                dbi.LastReview);
                  Console.WriteLine("Remarks: {0}", dbi.Message);
               }
            }
         }
         Console.ReadLine();
      }
   }
}
```

# C# 属性（Property）

**属性（Property）** 是类（class）、结构（structure）和接口（interface）的命名（named）成员。类或结构中的成员变量或方法称为 **域（Field）**。属性（Property）是域（Field）的扩展，且可使用相同的语法来访问。它们使用 **访问器（accessors）** 让私有域的值可被读写或操作。

属性（Property）不会确定存储位置。相反，它们具有可读写或计算它们值的 **访问器（accessors）**。

例如，有一个名为 Student 的类，带有 age、name 和 code 的私有域。我们不能在类的范围以外直接访问这些域，但是我们可以拥有访问这些私有域的属性。

## 访问器（Accessors）

属性（Property）的**访问器（accessor）**包含有助于获取（读取或计算）或设置（写入）属性的可执行语句。访问器（accessor）声明可包含一个 get 访问器、一个 set 访问器，或者同时包含二者。例如：

```C#
// 声明类型为 string 的 Code 属性  
public string Code  
{  
   get  
   {  
      return code;  
   }  
   set  
   {  
      code = value;  
   }  
}  
  
// 声明类型为 string 的 Name 属性  
public string Name  
{  
   get  
   {  
     return name;  
   }  
   set  
   {  
     name = value;  
   }  
}  
  
// 声明类型为 int 的 Age 属性  
public int Age  
{   
   get  
   {  
      return age;  
   }  
   set  
   {  
      age = value;  
   }  
}

```

## 实例

下面的实例演示了属性（Property）的用法：

```C#
using System;
namespace runoob
{
   class Student
   {

      private string code = "N.A";
      private string name = "not known";
      private int age = 0;

      // 声明类型为 string 的 Code 属性
      public string Code
      {
         get
         {
            return code;
         }
         set
         {
            code = value;
         }
      }
   
      // 声明类型为 string 的 Name 属性
      public string Name
      {
         get
         {
            return name;
         }
         set
         {
            name = value;
         }
      }

      // 声明类型为 int 的 Age 属性
      public int Age
      {
         get
         {
            return age;
         }
         set
         {
            age = value;
         }
      }
      public override string ToString()
      {
         return "Code = " + Code +", Name = " + Name + ", Age = " + Age;
      }
    }
    class ExampleDemo
    {
      public static void Main()
      {
         // 创建一个新的 Student 对象
         Student s = new Student();
            
         // 设置 student 的 code、name 和 age
         s.Code = "001";
         s.Name = "Zara";
         s.Age = 9;
         Console.WriteLine("Student Info: {0}", s);
         // 增加年龄
         s.Age += 1;
         Console.WriteLine("Student Info: {0}", s);
         Console.ReadKey();
       }
   }
}
```

## 抽象属性（Abstract Properties）

抽象类可拥有抽象属性，这些属性应在派生类中被实现。下面的程序说明了这点：

```C#
using System;
namespace runoob
{
   public abstract class Person
   {
      public abstract string Name
      {
         get;
         set;
      }
      public abstract int Age
      {
         get;
         set;
      }
   }
   class Student : Person
   {

      private string code = "N.A";
      private string name = "N.A";
      private int age = 0;

      // 声明类型为 string 的 Code 属性
      public string Code
      {
         get
         {
            return code;
         }
         set
         {
            code = value;
         }
      }
   
      // 声明类型为 string 的 Name 属性
      public override string Name
      {
         get
         {
            return name;
         }
         set
         {
            name = value;
         }
      }

      // 声明类型为 int 的 Age 属性
      public override int Age
      {
         get
         {
            return age;
         }
         set
         {
            age = value;
         }
      }
      public override string ToString()
      {
         return "Code = " + Code +", Name = " + Name + ", Age = " + Age;
      }
   }
   class ExampleDemo
   {
      public static void Main()
      {
         // 创建一个新的 Student 对象
         Student s = new Student();
            
         // 设置 student 的 code、name 和 age
         s.Code = "001";
         s.Name = "Zara";
         s.Age = 9;
         Console.WriteLine("Student Info:- {0}", s);
         // 增加年龄
         s.Age += 1;
         Console.WriteLine("Student Info:- {0}", s);
         Console.ReadKey();
       }
   }
}
```

# C# 索引器（Indexer）

**索引器（Indexer）** 允许一个对象可以像数组一样被索引。当您为类定义一个索引器时，该类的行为就会像一个 **虚拟数组（virtual array）** 一样。您可以使用数组访问运算符（[ ]）来访问该类的实例。

## 语法

一维索引器的语法如下：

```C#
element-type this[int index] 
{
   // get 访问器
   get 
   {
      // 返回 index 指定的值
   }

   // set 访问器
   set 
   {
      // 设置 index 指定的值 
   }
}
```

## 索引器（Indexer）的用途

索引器的行为的声明在某种程度上类似于属性（property）。就像属性（property），您可使用 **get** 和 **set** 访问器来定义索引器。但是，属性返回或设置一个特定的数据成员，而索引器返回或设置对象实例的一个特定值。换句话说，它把实例数据分为更小的部分，并索引每个部分，获取或设置每个部分。

定义一个属性（property）包括提供属性名称。索引器定义的时候不带有名称，但带有 **this** 关键字，它指向对象实例。下面的实例演示了这个概念：

```C#
using System;
namespace IndexerApplication
{
   class IndexedNames
   {
      private string[] namelist = new string[size];
      static public int size = 10;
      public IndexedNames()
      {
         for (int i = 0; i < size; i++)
         namelist[i] = "N. A.";
      }
      public string this[int index]
      {
         get
         {
            string tmp;

            if( index >= 0 && index <= size-1 )
            {
               tmp = namelist[index];
            }
            else
            {
               tmp = "";
            }

            return ( tmp );
         }
         set
         {
            if( index >= 0 && index <= size-1 )
            {
               namelist[index] = value;
            }
         }
      }

      static void Main(string[] args)
      {
         IndexedNames names = new IndexedNames();
         names[0] = "Zara";
         names[1] = "Riz";
         names[2] = "Nuha";
         names[3] = "Asif";
         names[4] = "Davinder";
         names[5] = "Sunil";
         names[6] = "Rubic";
         for ( int i = 0; i < IndexedNames.size; i++ )
         {
            Console.WriteLine(names[i]);
         }
         Console.ReadKey();
      }
   }
}
```

## 重载索引器（Indexer）

索引器（Indexer）可被重载。索引器声明的时候也可带有多个参数，且每个参数可以是不同的类型。没有必要让索引器必须是整型的。C# 允许索引器可以是其他类型，例如，字符串类型。

下面的实例演示了重载索引器：

```C#
using System;
namespace IndexerApplication
{
   class IndexedNames
   {
      private string[] namelist = new string[size];
      static public int size = 10;
      public IndexedNames()
      {
         for (int i = 0; i < size; i++)
         {
          namelist[i] = "N. A.";
         }
      }
      public string this[int index]
      {
         get
         {
            string tmp;

            if( index >= 0 && index <= size-1 )
            {
               tmp = namelist[index];
            }
            else
            {
               tmp = "";
            }

            return ( tmp );
         }
         set
         {
            if( index >= 0 && index <= size-1 )
            {
               namelist[index] = value;
            }
         }
      }
      public int this[string name]
      {
         get
         {
            int index = 0;
            while(index < size)
            {
               if (namelist[index] == name)
               {
                return index;
               }
               index++;
            }
            return index;
         }

      }

      static void Main(string[] args)
      {
         IndexedNames names = new IndexedNames();
         names[0] = "Zara";
         names[1] = "Riz";
         names[2] = "Nuha";
         names[3] = "Asif";
         names[4] = "Davinder";
         names[5] = "Sunil";
         names[6] = "Rubic";
         // 使用带有 int 参数的第一个索引器
         for (int i = 0; i < IndexedNames.size; i++)
         {
            Console.WriteLine(names[i]);
         }
         // 使用带有 string 参数的第二个索引器
         Console.WriteLine(names["Nuha"]);
         Console.ReadKey();
      }
   }
}
```

# C# 委托（Delegate）

C# 中的委托（Delegate）类似于 C 或 C++ 中函数的指针。**委托（Delegate）** 是存有对某个方法的引用的一种引用类型变量。引用可在运行时被改变。

委托（Delegate）特别用于实现事件和回调方法。所有的委托（Delegate）都派生自 **System.Delegate** 类。

## 声明委托（Delegate）

委托声明决定了可由该委托引用的方法。委托可指向一个与其具有相同标签的方法。

例如，假设有一个委托：

```
public delegate int MyDelegate (string s);
```

上面的委托可被用于引用任何一个带有一个单一的 _string_ 参数的方法，并返回一个 _int_ 类型变量。

声明委托的语法如下：

```
delegate <return type> <delegate-name> <parameter list>
```

## 实例化委托（Delegate）

一旦声明了委托类型，委托对象必须使用 **new** 关键字来创建，且与一个特定的方法有关。当创建委托时，传递到 **new** 语句的参数就像方法调用一样书写，但是不带有参数。例如：

```
public delegate void printString(string s);  
...  
printString ps1 = new printString(WriteToScreen);  
printString ps2 = new printString(WriteToFile);  
```

下面的实例演示了委托的声明、实例化和使用，该委托可用于引用带有一个整型参数的方法，并返回一个整型值。

```C#
using System;

delegate int NumberChanger(int n);
namespace DelegateAppl
{
   class TestDelegate
   {
      static int num = 10;
      public static int AddNum(int p)
      {
         num += p;
         return num;
      }

      public static int MultNum(int q)
      {
         num *= q;
         return num;
      }
      public static int getNum()
      {
         return num;
      }

      static void Main(string[] args)
      {
         // 创建委托实例
         NumberChanger nc1 = new NumberChanger(AddNum);
         NumberChanger nc2 = new NumberChanger(MultNum);
         // 使用委托对象调用方法
         nc1(25);
         Console.WriteLine("Value of Num: {0}", getNum());
         nc2(5);
         Console.WriteLine("Value of Num: {0}", getNum());
         Console.ReadKey();
      }
   }
}
```

## 委托的多播（Multicasting of a Delegate）

委托对象可使用 "+" 运算符进行合并。一个合并委托调用它所合并的两个委托。只有相同类型的委托可被合并。"-" 运算符可用于从合并的委托中移除组件委托。 

使用委托的这个有用的特点，您可以创建一个委托被调用时要调用的方法的调用列表。这被称为委托的 **多播（multicasting）**，也叫组播。下面的程序演示了委托的多播：

```C#
using System;

delegate int NumberChanger(int n);
namespace DelegateAppl
{
   class TestDelegate
   {
      static int num = 10;
      public static int AddNum(int p)
      {
         num += p;
         return num;
      }

      public static int MultNum(int q)
      {
         num *= q;
         return num;
      }
      public static int getNum()
      {
         return num;
      }

      static void Main(string[] args)
      {
         // 创建委托实例
         NumberChanger nc;
         NumberChanger nc1 = new NumberChanger(AddNum);
         NumberChanger nc2 = new NumberChanger(MultNum);
         nc = nc1;
         nc += nc2;
         // 调用多播
         nc(5);
         Console.WriteLine("Value of Num: {0}", getNum());
         Console.ReadKey();
      }
   }
}
```

## 委托（Delegate）的用途

下面的实例演示了委托的用法。委托 _printString_ 可用于引用带有一个字符串作为输入的方法，并不返回任何东西。

我们使用这个委托来调用两个方法，第一个把字符串打印到控制台，第二个把字符串打印到文件：

```C#
using System;
using System.IO;

namespace DelegateAppl
{
   class PrintString
   {
      static FileStream fs;
      static StreamWriter sw;
      // 委托声明
      public delegate void printString(string s);

      // 该方法打印到控制台
      public static void WriteToScreen(string str)
      {
         Console.WriteLine("The String is: {0}", str);
      }
      // 该方法打印到文件
      public static void WriteToFile(string s)
      {
         fs = new FileStream("c:\\message.txt",
         FileMode.Append, FileAccess.Write);
         sw = new StreamWriter(fs);
         sw.WriteLine(s);
         sw.Flush();
         sw.Close();
         fs.Close();
      }
      // 该方法把委托作为参数，并使用它调用方法
      public static void sendString(printString ps)
      {
         ps("Hello World");
      }
      static void Main(string[] args)
      {
         printString ps1 = new printString(WriteToScreen);
         printString ps2 = new printString(WriteToFile);
         sendString(ps1);
         sendString(ps2);
         Console.ReadKey();
      }
   }
}
```

# C# 事件（Event）

**事件（Event）** 基本上说是一个用户操作，如按键、点击、鼠标移动等等，或者是一些提示信息，如系统生成的通知。应用程序需要在事件发生时响应事件。例如，中断。

C# 中使用事件机制实现线程间的通信。

## 通过事件使用委托

事件在类中声明且生成，且通过使用同一个类或其他类中的委托与事件处理程序关联。包含事件的类用于发布事件。这被称为 **发布器（publisher）** 类。其他接受该事件的类被称为 **订阅器（subscriber）** 类。事件使用 **发布-订阅（publisher-subscriber）** 模型。

**发布器（publisher）** 是一个包含事件和委托定义的对象。事件和委托之间的联系也定义在这个对象中。发布器（publisher）类的对象调用这个事件，并通知其他的对象。

**订阅器（subscriber）** 是一个接受事件并提供事件处理程序的对象。在发布器（publisher）类中的委托调用订阅器（subscriber）类中的方法（事件处理程序）。

## 声明事件（Event）

在类的内部声明事件，首先必须声明该事件的委托类型。例如：

```
public delegate void BoilerLogHandler(string status);
```

然后，声明事件本身，使用 **event** 关键字：

```
// 基于上面的委托定义事件 
public event BoilerLogHandler BoilerEventLog;
```

上面的代码定义了一个名为 _BoilerLogHandler_ 的委托和一个名为 _BoilerEventLog_ 的事件，该事件在生成的时候会调用委托。

## 实例

```C#
using System;
namespace SimpleEvent
{
  using System;
  /***********发布器类***********/
  public class EventTest
  {
    private int value;

    public delegate void NumManipulationHandler();


    public event NumManipulationHandler ChangeNum;
    protected virtual void OnNumChanged()
    {
      if ( ChangeNum != null )
      {
        ChangeNum(); /* 事件被触发 */
      }else {
        Console.WriteLine( "event not fire" );
        Console.ReadKey(); /* 回车继续 */
      }
    }


    public EventTest()
    {
      int n = 5;
      SetValue( n );
    }


    public void SetValue( int n )
    {
      if ( value != n )
      {
        value = n;
        OnNumChanged();
      }
    }
  }


  /***********订阅器类***********/

  public class subscribEvent
  {
    public void printf()
    {
      Console.WriteLine( "event fire" );
      Console.ReadKey(); /* 回车继续 */
    }
  }

  /***********触发***********/
  public class MainClass
  {
    public static void Main()
    {
      EventTest e = new EventTest(); /* 实例化对象,第一次没有触发事件 */
      subscribEvent v = new subscribEvent(); /* 实例化对象 */
      e.ChangeNum += new EventTest.NumManipulationHandler( v.printf ); /* 注册 */
      e.SetValue( 7 );
      e.SetValue( 11 );
    }
  }
}
```

本实例提供一个简单的用于热水锅炉系统故障排除的应用程序。当维修工程师检查锅炉时，锅炉的温度和压力会随着维修工程师的备注自动记录到日志文件中。

```C#
using System;
using System.IO;

namespace BoilerEventAppl
{

   // boiler 类
   class Boiler
   {
      private int temp;
      private int pressure;
      public Boiler(int t, int p)
      {
         temp = t;
         pressure = p;
      }

      public int getTemp()
      {
         return temp;
      }
      public int getPressure()
      {
         return pressure;
      }
   }
   // 事件发布器
   class DelegateBoilerEvent
   {
      public delegate void BoilerLogHandler(string status);

      // 基于上面的委托定义事件
      public event BoilerLogHandler BoilerEventLog;

      public void LogProcess()
      {
         string remarks = "O. K";
         Boiler b = new Boiler(100, 12);
         int t = b.getTemp();
         int p = b.getPressure();
         if(t > 150 || t < 80 || p < 12 || p > 15)
         {
            remarks = "Need Maintenance";
         }
         OnBoilerEventLog("Logging Info:\n");
         OnBoilerEventLog("Temparature " + t + "\nPressure: " + p);
         OnBoilerEventLog("\nMessage: " + remarks);
      }

      protected void OnBoilerEventLog(string message)
      {
         if (BoilerEventLog != null)
         {
            BoilerEventLog(message);
         }
      }
   }
   // 该类保留写入日志文件的条款
   class BoilerInfoLogger
   {
      FileStream fs;
      StreamWriter sw;
      public BoilerInfoLogger(string filename)
      {
         fs = new FileStream(filename, FileMode.Append, FileAccess.Write);
         sw = new StreamWriter(fs);
      }
      public void Logger(string info)
      {
         sw.WriteLine(info);
      }
      public void Close()
      {
         sw.Close();
         fs.Close();
      }
   }
   // 事件订阅器
   public class RecordBoilerInfo
   {
      static void Logger(string info)
      {
         Console.WriteLine(info);
      }//end of Logger

      static void Main(string[] args)
      {
         BoilerInfoLogger filelog = new BoilerInfoLogger("e:\\boiler.txt");
         DelegateBoilerEvent boilerEvent = new DelegateBoilerEvent();
         boilerEvent.BoilerEventLog += new 
         DelegateBoilerEvent.BoilerLogHandler(Logger);
         boilerEvent.BoilerEventLog += new 
         DelegateBoilerEvent.BoilerLogHandler(filelog.Logger);
         boilerEvent.LogProcess();
         Console.ReadLine();
         filelog.Close();
      }//end of main

   }//end of RecordBoilerInfo
}
```

# C# 集合（Collection）

集合（Collection）类是专门用于数据存储和检索的类。这些类提供了对栈（stack）、队列（queue）、列表（list）和哈希表（hash table）的支持。大多数集合类实现了相同的接口。

集合（Collection）类服务于不同的目的，如为元素动态分配内存，基于索引访问列表项等等。这些类创建 Object 类的对象的集合。在 C# 中，Object 类是所有数据类型的基类。

## C# 动态数组（ArrayList）

动态数组（ArrayList）代表了可被单独索引的对象的有序集合。它基本上可以替代一个数组。但是，与数组不同的是，您可以使用**索引**在指定的位置添加和移除项目，动态数组会自动重新调整它的大小。它也允许在列表中进行动态内存分配、增加、搜索、排序各项。

### ArrayList 类的方法和属性

下表列出了 **ArrayList** 类的一些常用的 **属性**：

| 属性          | 描述                           |
|-------------|------------------------------|
| Capacity    | 获取或设置 ArrayList 可以包含的元素个数。   |
| Count       | 获取 ArrayList 中实际包含的元素个数。     |
| IsFixedSize | 获取一个值，表示 ArrayList 是否具有固定大小。 |
| IsReadOnly  | 获取一个值，表示 ArrayList 是否只读。     |
| Item        | 获取或设置指定索引处的元素。               |

下表列出了 **ArrayList** 类的一些常用的 **方法**：

| 序号 | 方法名 & 描述                                                                                          |
|----|---------------------------------------------------------------------------------------------------|
| 1  | public virtual int Add\( object value \); 在 ArrayList 的末尾添加一个对象。                                  |
| 2  | public virtual void AddRange\( ICollection c \); 在 ArrayList 的末尾添加 ICollection 的元素。               |
| 3  | public virtual void Clear\(\);从 ArrayList 中移除所有的元素。                                               |
| 4  | public virtual bool Contains\( object item \); 判断某个元素是否在 ArrayList 中。                             |
| 5  | public virtual ArrayList GetRange\( int index, int count \); 返回一个 ArrayList，表示源 ArrayList 中元素的子集。 |
| 6  | public virtual int IndexOf\(object\);返回某个值在 ArrayList 中第一次出现的索引，索引从零开始。                           |
| 7  | public virtual void Insert\( int index, object value \); 在 ArrayList 的指定索引处，插入一个元素。               |
| 8  | public virtual void InsertRange\( int index, ICollection c \); 在 ArrayList 的指定索引处，插入某个集合的元素。      |
| 9  | public virtual void Remove\( object obj \); 从 ArrayList 中移除第一次出现的指定对象。                            |
| 10 | public virtual void RemoveAt\( int index \); 移除 ArrayList 的指定索引处的元素。                              |
| 11 | public virtual void RemoveRange\( int index, int count \); 从 ArrayList 中移除某个范围的元素。                |
| 12 | public virtual void Reverse\(\);逆转 ArrayList 中元素的顺序。                                              |
| 13 | public virtual void SetRange\( int index, ICollection c \); 复制某个集合的元素到 ArrayList 中某个范围的元素上。       |
| 14 | public virtual void Sort\(\);对 ArrayList 中的元素进行排序。                                                |
| 15 | public virtual void TrimToSize\(\);设置容量为 ArrayList 中元素的实际个数。                                      |

### 实例

下面的实例演示了动态数组（ArrayList）的概念：

```C#
using System;
using System.Collections;

namespace CollectionApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            ArrayList al = new ArrayList();

            Console.WriteLine("Adding some numbers:");
            al.Add(45);
            al.Add(78);
            al.Add(33);
            al.Add(56);
            al.Add(12);
            al.Add(23);
            al.Add(9);
            
            Console.WriteLine("Capacity: {0} ", al.Capacity);
            Console.WriteLine("Count: {0}", al.Count);
                      
            Console.Write("Content: ");
            foreach (int i in al)
            {
                Console.Write(i + " ");
            }
            Console.WriteLine();
            Console.Write("Sorted Content: ");
            al.Sort();
            foreach (int i in al)
            {
                Console.Write(i + " ");
            }
            Console.WriteLine();
            Console.ReadKey();
        }
    }
}
```

## C# 哈希表（Hashtable）

Hashtable 类代表了一系列基于键的哈希代码组织起来的**键/值**对。它使用**键**来访问集合中的元素。

当您使用**键**访问元素时，则使用哈希表，而且您可以识别一个有用的键值。哈希表中的每一项都有一个**键/值**对。键用于访问集合中的项目。

### Hashtable 类的方法和属性

下表列出了 **Hashtable** 类的一些常用的 **属性**：

| 属性          | 描述                                 |
|-------------|------------------------------------|
| Count       | 获取 Hashtable 中包含的键值对个数。            |
| IsFixedSize | 获取一个值，表示 Hashtable 是否具有固定大小。       |
| IsReadOnly  | 获取一个值，表示 Hashtable 是否只读。           |
| Item        | 获取或设置与指定的键相关的值。                    |
| Keys        | 获取一个 ICollection，包含 Hashtable 中的键。 |
| Values      | 获取一个 ICollection，包含 Hashtable 中的值。 |

下表列出了 **Hashtable** 类的一些常用的 **方法**：

| 序号 | 方法名 & 描述                                                                            |
|----|-------------------------------------------------------------------------------------|
| 1  | public virtual void Add\( object key, object value \); 向 Hashtable 添加一个带有指定的键和值的元素。 |
| 2  | public virtual void Clear\(\); 从 Hashtable 中移除所有的元素。                                |
| 3  | public virtual bool ContainsKey\( object key \); 判断 Hashtable 是否包含指定的键。             |
| 4  | public virtual bool ContainsValue\( object value \); 判断 Hashtable 是否包含指定的值。         |
| 5  | public virtual void Remove\( object key \); 从 Hashtable 中移除带有指定的键的元素。               |

### 实例

下面的实例演示了哈希表（Hashtable）的概念：

```C#
using System;
using System.Collections;

namespace CollectionsApplication
{
   class Program
   {
      static void Main(string[] args)
      {
         Hashtable ht = new Hashtable();


         ht.Add("001", "Zara Ali");
         ht.Add("002", "Abida Rehman");
         ht.Add("003", "Joe Holzner");
         ht.Add("004", "Mausam Benazir Nur");
         ht.Add("005", "M. Amlan");
         ht.Add("006", "M. Arif");
         ht.Add("007", "Ritesh Saikia");

         if (ht.ContainsValue("Nuha Ali"))
         {
            Console.WriteLine("This student name is already in the list");
         }
         else
         {
            ht.Add("008", "Nuha Ali");
         }
         // 获取键的集合 
         ICollection key = ht.Keys;

         foreach (string k in key)
         {
            Console.WriteLine(k + ": " + ht[k]);
         }
         Console.ReadKey();
      }
   }
}
```

## C# 排序列表（SortedList）

SortedList 类代表了一系列按照键来排序的**键/值**对，这些键值对可以通过键和索引来访问。

排序列表是数组和哈希表的组合。它包含一个可使用键或索引访问各项的列表。如果您使用索引访问各项，则它是一个动态数组（ArrayList），如果您使用键访问各项，则它是一个哈希表（Hashtable）。集合中的各项总是按键值排序。

### SortedList 类的方法和属性

下表列出了 **SortedList** 类的一些常用的 **属性**：

| 属性          | 描述                            |
|-------------|-------------------------------|
| Capacity    | 获取或设置 SortedList 的容量。         |
| Count       | 获取 SortedList 中的元素个数。         |
| IsFixedSize | 获取一个值，表示 SortedList 是否具有固定大小。 |
| IsReadOnly  | 获取一个值，表示 SortedList 是否只读。     |
| Item        | 获取或设置与 SortedList 中指定的键相关的值。  |
| Keys        | 获取 SortedList 中的键。            |
| Values      | 获取 SortedList 中的值。            |

下表列出了 **SortedList** 类的一些常用的 **方法**：

| 序号 | 方法名 & 描述                                                                               |
|----|----------------------------------------------------------------------------------------|
| 1  | public virtual void Add\( object key, object value \); 向 SortedList 添加一个带有指定的键和值的元素。   |
| 2  | public virtual void Clear\(\); 从 SortedList 中移除所有的元素。                                  |
| 3  | public virtual bool ContainsKey\( object key \); 判断 SortedList 是否包含指定的键。               |
| 4  | public virtual bool ContainsValue\( object value \); 判断 SortedList 是否包含指定的值。           |
| 5  | public virtual object GetByIndex\( int index \); 获取 SortedList 的指定索引处的值。               |
| 6  | public virtual object GetKey\( int index \); 获取 SortedList 的指定索引处的键。                   |
| 7  | public virtual IList GetKeyList\(\); 获取 SortedList 中的键。                                |
| 8  | public virtual IList GetValueList\(\); 获取 SortedList 中的值。                              |
| 9  | public virtual int IndexOfKey\( object key \); 返回 SortedList 中的指定键的索引，索引从零开始。          |
| 10 | public virtual int IndexOfValue\( object value \); 返回 SortedList 中的指定值第一次出现的索引，索引从零开始。 |
| 11 | public virtual void Remove\( object key \); 从 SortedList 中移除带有指定的键的元素。                 |
| 12 | public virtual void RemoveAt\( int index \); 移除 SortedList 的指定索引处的元素。                  |
| 13 | public virtual void TrimToSize\(\); 设置容量为 SortedList 中元素的实际个数。                         |

### 实例

下面的实例演示了排序列表（SortedList）的概念：

```C#
using System;
using System.Collections;

namespace CollectionsApplication
{
   class Program
   {
      static void Main(string[] args)
      {
         SortedList sl = new SortedList();

         sl.Add("001", "Zara Ali");
         sl.Add("002", "Abida Rehman");
         sl.Add("003", "Joe Holzner");
         sl.Add("004", "Mausam Benazir Nur");
         sl.Add("005", "M. Amlan");
         sl.Add("006", "M. Arif");
         sl.Add("007", "Ritesh Saikia");

         if (sl.ContainsValue("Nuha Ali"))
         {
            Console.WriteLine("This student name is already in the list");
         }
         else
         {
            sl.Add("008", "Nuha Ali");
         }

         // 获取键的集合 
         ICollection key = sl.Keys;

         foreach (string k in key)
         {
            Console.WriteLine(k + ": " + sl[k]);
         }
      }
   }
}
```

## C# 堆栈（Stack）

堆栈（Stack）代表了一个**后进先出**的对象集合。当您需要对各项进行后进先出的访问时，则使用堆栈。当您在列表中添加一项，称为**推入**元素，当您从列表中移除一项时，称为**弹出**元素。

### Stack 类的方法和属性

下表列出了 **Stack** 类的一些常用的 **属性**：

| 属性    | 描述                 |
|-------|--------------------|
| Count | 获取 Stack 中包含的元素个数。 |

下表列出了 **Stack** 类的一些常用的 **方法**：

| 序号 | 方法名 & 描述                                                         |
|----|------------------------------------------------------------------|
| 1  | public virtual void Clear\(\); 从 Stack 中移除所有的元素。                 |
| 2  | public virtual bool Contains\( object obj \); 判断某个元素是否在 Stack 中。 |
| 3  | public virtual object Peek\(\);返回在 Stack 的顶部的对象，但不移除它。           |
| 4  | public virtual object Pop\(\);移除并返回在 Stack 的顶部的对象。               |
| 5  | public virtual void Push\( object obj \);向 Stack 的顶部添加一个对象。      |
| 6  | public virtual object\[\] ToArray\(\);复制 Stack 到一个新的数组中。         |

### 实例

下面的实例演示了堆栈（Stack）的使用：

```C#
using System;
using System.Collections;

namespace CollectionsApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            Stack st = new Stack();

            st.Push('A');
            st.Push('M');
            st.Push('G');
            st.Push('W');
            
            Console.WriteLine("Current stack: ");
            foreach (char c in st)
            {
                Console.Write(c + " ");
            }
            Console.WriteLine();
            
            st.Push('V');
            st.Push('H');
            Console.WriteLine("The next poppable value in stack: {0}", 
            st.Peek());
            Console.WriteLine("Current stack: ");           
            foreach (char c in st)
            {
               Console.Write(c + " ");
            }
            Console.WriteLine();

            Console.WriteLine("Removing values ");
            st.Pop();
            st.Pop();
            st.Pop();
            
            Console.WriteLine("Current stack: ");
            foreach (char c in st)
            {
               Console.Write(c + " "); 
            }
        }
    }
}
```

## C# 队列（Queue）

队列（Queue）代表了一个**先进先出**的对象集合。当您需要对各项进行先进先出的访问时，则使用队列。当您在列表中添加一项，称为**入队**，当您从列表中移除一项时，称为**出队**。

### Queue 类的方法和属性

下表列出了 **Queue** 类的一些常用的 **属性**：

| 属性    | 描述                 |
|-------|--------------------|
| Count | 获取 Queue 中包含的元素个数。 |

下表列出了 **Queue** 类的一些常用的 **方法**：

| 序号 | 方法名 & 描述                                                         |
|----|------------------------------------------------------------------|
| 1  | public virtual void Clear\(\); 从 Queue 中移除所有的元素。                 |
| 2  | public virtual bool Contains\( object obj \); 判断某个元素是否在 Queue 中。 |
| 3  | public virtual object Dequeue\(\);移除并返回在 Queue 的开头的对象。           |
| 4  | public virtual void Enqueue\( object obj \); 向 Queue 的末尾添加一个对象。  |
| 5  | public virtual object\[\] ToArray\(\);复制 Queue 到一个新的数组中。         |
| 6  | public virtual void TrimToSize\(\);设置容量为 Queue 中元素的实际个数。         |

### 实例

下面的实例演示了队列（Queue）的使用：

```C#
using System;
using System.Collections;

namespace CollectionsApplication
{
   class Program
   {
      static void Main(string[] args)
      {
         Queue q = new Queue();

         q.Enqueue('A');
         q.Enqueue('M');
         q.Enqueue('G');
         q.Enqueue('W');
         
         Console.WriteLine("Current queue: ");
         foreach (char c in q)
            Console.Write(c + " ");
         Console.WriteLine();
         q.Enqueue('V');
         q.Enqueue('H');
         Console.WriteLine("Current queue: ");         
         foreach (char c in q)
            Console.Write(c + " ");
         Console.WriteLine();
         Console.WriteLine("Removing some values ");
         char ch = (char)q.Dequeue();
         Console.WriteLine("The removed value: {0}", ch);
         ch = (char)q.Dequeue();
         Console.WriteLine("The removed value: {0}", ch);
         Console.ReadKey();
      }
   }
}
```

## C# 点阵列（BitArray）

BitArray 类管理一个紧凑型的位值数组，它使用布尔值来表示，其中 true 表示位是开启的（1），false 表示位是关闭的（0）。

当您需要存储位，但是事先不知道位数时，则使用点阵列。您可以使用**整型索引**从点阵列集合中访问各项，索引从零开始。

### BitArray 类的方法和属性

下表列出了 **BitArray** 类的一些常用的 **属性**：

| 属性         | 描述                        |
|------------|---------------------------|
| Count      | 获取 BitArray 中包含的元素个数。     |
| IsReadOnly | 获取一个值，表示 BitArray 是否只读。   |
| Item       | 获取或设置 BitArray 中指定位置的位的值。 |
| Length     | 获取或设置 BitArray 中的元素个数。    |

下表列出了 **BitArray** 类的一些常用的 **方法**：

| 序号 | 方法名 & 描述                                                                                   |
|----|--------------------------------------------------------------------------------------------|
| 1  | public BitArray And\( BitArray value \); 对当前的 BitArray 中的元素和指定的 BitArray 中的相对应的元素执行按位与操作。  |
| 2  | public bool Get\( int index \); 获取 BitArray 中指定位置的位的值。                                     |
| 3  | public BitArray Not\(\);把当前的 BitArray 中的位值反转，以便设置为 true 的元素变为 false，设置为 false 的元素变为 true。  |
| 4  | public BitArray Or\( BitArray value \); 对当前的 BitArray 中的元素和指定的 BitArray 中的相对应的元素执行按位或操作。   |
| 5  | public void Set\( int index, bool value \); 把 BitArray 中指定位置的位设置为指定的值。                     |
| 6  | public void SetAll\( bool value \); 把 BitArray 中的所有位设置为指定的值。                               |
| 7  | public BitArray Xor\( BitArray value \); 对当前的 BitArray 中的元素和指定的 BitArray 中的相对应的元素执行按位异或操作。 |

### 实例

下面的实例演示了点阵列（BitArray）的使用：

```C#
using System;
using System.Collections;

namespace CollectionsApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            // 创建两个大小为 8 的点阵列
            BitArray ba1 = new BitArray(8);
            BitArray ba2 = new BitArray(8);
            byte[] a = { 60 };
            byte[] b = { 13 };
            
            // 把值 60 和 13 存储到点阵列中
            ba1 = new BitArray(a);
            ba2 = new BitArray(b);

            // ba1 的内容
            Console.WriteLine("Bit array ba1: 60");
            for (int i = 0; i < ba1.Count; i++)
            {
                Console.Write("{0, -6} ", ba1[i]);
            }
            Console.WriteLine();
            
            // ba2 的内容
            Console.WriteLine("Bit array ba2: 13");
            for (int i = 0; i < ba2.Count; i++)
            {
                Console.Write("{0, -6} ", ba2[i]);
            }
            Console.WriteLine();
           
            
            BitArray ba3 = new BitArray(8);
            ba3 = ba1.And(ba2);

            // ba3 的内容
            Console.WriteLine("Bit array ba3 after AND operation: 12");
            for (int i = 0; i < ba3.Count; i++)
            {
                Console.Write("{0, -6} ", ba3[i]);
            }
            Console.WriteLine();

            ba3 = ba1.Or(ba2);
            // ba3 的内容
            Console.WriteLine("Bit array ba3 after OR operation: 61");
            for (int i = 0; i < ba3.Count; i++)
            {
                Console.Write("{0, -6} ", ba3[i]);
            }
            Console.WriteLine();
            
            Console.ReadKey();
        }
    }
}
```

# C# 泛型（Generic）

**泛型（Generic）** 允许您延迟编写类或方法中的编程元素的数据类型的规范，直到实际在程序中使用它的时候。换句话说，泛型允许您编写一个可以与任何数据类型一起工作的类或方法。

您可以通过数据类型的替代参数编写类或方法的规范。当编译器遇到类的构造函数或方法的函数调用时，它会生成代码来处理指定的数据类型。下面这个简单的实例将有助于您理解这个概念：

```C#
using System;
using System.Collections.Generic;

namespace GenericApplication
{
    public class MyGenericArray<T>
    {
        private T[] array;
        public MyGenericArray(int size)
        {
            array = new T[size + 1];
        }
        public T getItem(int index)
        {
            return array[index];
        }
        public void setItem(int index, T value)
        {
            array[index] = value;
        }
    }
           
    class Tester
    {
        static void Main(string[] args)
        {
            // 声明一个整型数组
            MyGenericArray<int> intArray = new MyGenericArray<int>(5);
            // 设置值
            for (int c = 0; c < 5; c++)
            {
                intArray.setItem(c, c*5);
            }
            // 获取值
            for (int c = 0; c < 5; c++)
            {
                Console.Write(intArray.getItem(c) + " ");
            }
            Console.WriteLine();
            // 声明一个字符数组
            MyGenericArray<char> charArray = new MyGenericArray<char>(5);
            // 设置值
            for (int c = 0; c < 5; c++)
            {
                charArray.setItem(c, (char)(c+97));
            }
            // 获取值
            for (int c = 0; c < 5; c++)
            {
                Console.Write(charArray.getItem(c) + " ");
            }
            Console.WriteLine();
            Console.ReadKey();
        }
    }
}
```

## 泛型（Generic）的特性

使用泛型是一种增强程序功能的技术，具体表现在以下几个方面：

  * 它有助于您最大限度地重用代码、保护类型的安全以及提高性能。
  * 您可以创建泛型集合类。.NET 框架类库在 _System.Collections.Generic_ 命名空间中包含了一些新的泛型集合类。您可以使用这些泛型集合类来替代 _System.Collections_ 中的集合类。
  * 您可以创建自己的泛型接口、泛型类、泛型方法、泛型事件和泛型委托。 
  * 您可以对泛型类进行约束以访问特定数据类型的方法。
  * 关于泛型数据类型中使用的类型的信息可在运行时通过使用反射获取。

## 泛型（Generic）方法

在上面的实例中，我们已经使用了泛型类，我们可以通过类型参数声明泛型方法。下面的程序说明了这个概念：

```C#
using System;
using System.Collections.Generic;

namespace GenericMethodAppl
{
    class Program
    {
        static void Swap<T>(ref T lhs, ref T rhs)
        {
            T temp;
            temp = lhs;
            lhs = rhs;
            rhs = temp;
        }
        static void Main(string[] args)
        {
            int a, b;
            char c, d;
            a = 10;
            b = 20;
            c = 'I';
            d = 'V';

            // 在交换之前显示值
            Console.WriteLine("Int values before calling swap:");
            Console.WriteLine("a = {0}, b = {1}", a, b);
            Console.WriteLine("Char values before calling swap:");
            Console.WriteLine("c = {0}, d = {1}", c, d);

            // 调用 swap
            Swap<int>(ref a, ref b);
            Swap<char>(ref c, ref d);

            // 在交换之后显示值
            Console.WriteLine("Int values after calling swap:");
            Console.WriteLine("a = {0}, b = {1}", a, b);
            Console.WriteLine("Char values after calling swap:");
            Console.WriteLine("c = {0}, d = {1}", c, d);
            Console.ReadKey();
        }
    }
}
```

## 泛型（Generic）委托

您可以通过类型参数定义泛型委托。例如：

```C#
delegate T NumberChanger<T>(T n);
```

下面的实例演示了委托的使用：

```C#
using System;
using System.Collections.Generic;

delegate T NumberChanger<T>(T n);
namespace GenericDelegateAppl
{
    class TestDelegate
    {
        static int num = 10;
        public static int AddNum(int p)
        {
            num += p;
            return num;
        }

        public static int MultNum(int q)
        {
            num *= q;
            return num;
        }
        public static int getNum()
        {
            return num;
        }

        static void Main(string[] args)
        {
            // 创建委托实例
            NumberChanger<int> nc1 = new NumberChanger<int>(AddNum);
            NumberChanger<int> nc2 = new NumberChanger<int>(MultNum);
            // 使用委托对象调用方法
            nc1(25);
            Console.WriteLine("Value of Num: {0}", getNum());
            nc2(5);
            Console.WriteLine("Value of Num: {0}", getNum());
            Console.ReadKey();
        }
    }
}
```

# C# 匿名方法

我们已经提到过，委托是用于引用与其具有相同标签的方法。换句话说，您可以使用委托对象调用可由委托引用的方法。

**匿名方法（Anonymous methods）** 提供了一种传递代码块作为委托参数的技术。匿名方法是没有名称只有主体的方法。

在匿名方法中您不需要指定返回类型，它是从方法主体内的 return 语句推断的。

## 编写匿名方法的语法

匿名方法是通过使用 **delegate** 关键字创建委托实例来声明的。例如：

```C#
delegate void NumberChanger(int n);
...
NumberChanger nc = delegate(int x)
{
    Console.WriteLine("Anonymous Method: {0}", x);
};
```

代码块 _Console.WriteLine("Anonymous Method: {0}", x);_ 是匿名方法的主体。

委托可以通过匿名方法调用，也可以通过命名方法调用，即，通过向委托对象传递方法参数。

例如：

```
nc(10);
```

## 实例

下面的实例演示了匿名方法的概念：

```C#
using System;

delegate void NumberChanger(int n);
namespace DelegateAppl
{
    class TestDelegate
    {
        static int num = 10;
        public static void AddNum(int p)
        {
            num += p;
            Console.WriteLine("Named Method: {0}", num);
        }

        public static void MultNum(int q)
        {
            num *= q;
            Console.WriteLine("Named Method: {0}", num);
        }

        static void Main(string[] args)
        {
            // 使用匿名方法创建委托实例
            NumberChanger nc = delegate(int x)
            {
               Console.WriteLine("Anonymous Method: {0}", x);
            };
            
            // 使用匿名方法调用委托
            nc(10);

            // 使用命名方法实例化委托
            nc =  new NumberChanger(AddNum);
            
            // 使用命名方法调用委托
            nc(5);

            // 使用另一个命名方法实例化委托
            nc =  new NumberChanger(MultNum);
            
            // 使用命名方法调用委托
            nc(2);
            Console.ReadKey();
        }
    }
}
```

# C# 不安全代码

当一个代码块使用 **unsafe** 修饰符标记时，C# 允许在函数中使用指针变量。**不安全代码**或非托管代码是指使用了**指针**变量的代码块。

## 指针变量

**指针** 是值为另一个变量的地址的变量，即，内存位置的直接地址。就像其他变量或常量，您必须在使用指针存储其他变量地址之前声明指针。

指针变量声明的一般形式为：

```
type* var-name;
```

下面是指针类型声明的实例：

| 实例          | 描述               |
|-------------|------------------|
| int\* p     | p 是指向整数的指针。      |
| double\* p  | p 是指向双精度数的指针。    |
| float\* p   | p 是指向浮点数的指针。     |
| int\*\* p   | p 是指向整数的指针的指针。   |
| int\*\[\] p | p 是指向整数的指针的一维数组。 |
| char\* p    | p 是指向字符的指针。      |
| void\* p    | p 是指向未知类型的指针。    |

在同一个声明中声明多个指针时，星号 * 仅与基础类型一起写入；而不是用作每个指针名称的前缀。 例如:

```
int* p1, p2, p3; // 正确  
int *p1, *p2, *p3; // 错误 
```

下面的实例说明了 C# 中使用了 **unsafe** 修饰符时指针的使用：

```C#
using System;
namespace UnsafeCodeApplication
{
    class Program
    {
        static unsafe void Main(string[] args)
        {
            int var = 20;
            int* p = &var;
            Console.WriteLine("Data is: {0} ",  var);
            Console.WriteLine("Address is: {0}",  (int)p);
            Console.ReadKey();
        }
    }
}
```

您也可以不用声明整个方法作为不安全代码，只需要声明方法的一部分作为不安全代码。下面的实例说明了这点。

## 使用指针检索数据值

您可以使用 **ToString()** 方法检索存储在指针变量所引用位置的数据。下面的实例演示了这点：

```C#
using System;
namespace UnsafeCodeApplication
{
   class Program
   {
      public static void Main()
      {
         unsafe
         {
            int var = 20;
            int* p = &var;
            Console.WriteLine("Data is: {0} " , var);
            Console.WriteLine("Data is: {0} " , p->ToString());
            Console.WriteLine("Address is: {0} " , (int)p);
         }
         Console.ReadKey();
      }
   }
}
```

## 传递指针作为方法的参数

您可以向方法传递指针变量作为方法的参数。下面的实例说明了这点：

```C#
using System;
namespace UnsafeCodeApplication
{
   class TestPointer
   {
      public unsafe void swap(int* p, int *q)
      {
         int temp = *p;
         *p = *q;
         *q = temp;
      }

      public unsafe static void Main()
      {
         TestPointer p = new TestPointer();
         int var1 = 10;
         int var2 = 20;
         int* x = &var1;
         int* y = &var2;
         
         Console.WriteLine("Before Swap: var1:{0}, var2: {1}", var1, var2);
         p.swap(x, y);

         Console.WriteLine("After Swap: var1:{0}, var2: {1}", var1, var2);
         Console.ReadKey();
      }
   }
}
```

## 使用指针访问数组元素

在 C# 中，数组名称和一个指向与数组数据具有相同数据类型的指针是不同的变量类型。例如，int *p 和 int[] p 是不同的类型。您可以增加指针变量 p，因为它在内存中不是固定的，但是数组地址在内存中是固定的，所以您不能增加数组 p。

因此，如果您需要使用指针变量访问数组数据，可以像我们通常在 C 或 C++ 中所做的那样，使用 **fixed** 关键字来固定指针。

下面的实例演示了这点：

```C#
using System;
namespace UnsafeCodeApplication
{
   class TestPointer
   {
      public unsafe static void Main()
      {
         int[]  list = {10, 100, 200};
         fixed(int *ptr = list)

         /* 显示指针中数组地址 */
         for ( int i = 0; i < 3; i++)
         {
            Console.WriteLine("Address of list[{0}]={1}",i,(int)(ptr + i));
            Console.WriteLine("Value of list[{0}]={1}", i, *(ptr + i));
         }
         Console.ReadKey();
      }
   }
}
```

## 编译不安全代码

为了编译不安全代码，您必须切换到命令行编译器指定 **/unsafe** 命令行。

例如，为了编译包含不安全代码的名为 prog1.cs 的程序，需在命令行中输入命令：

```C#
csc /unsafe prog1.cs
```

如果您使用的是 Visual Studio IDE，那么您需要在项目属性中启用不安全代码。

步骤如下：

  * 通过双击资源管理器（Solution Explorer）中的属性（properties）节点，打开**项目属性（project properties）**。
  * 点击 **Build** 标签页。
  * 选择选项"**Allow unsafe code**"。

# C# 多线程

**线程** 被定义为程序的执行路径。每个线程都定义了一个独特的控制流。如果您的应用程序涉及到复杂的和耗时的操作，那么设置不同的线程执行路径往往是有益的，每个线程执行特定的工作。

线程是**轻量级进程**。一个使用线程的常见实例是现代操作系统中并行编程的实现。使用线程节省了 CPU 周期的浪费，同时提高了应用程序的效率。

到目前为止我们编写的程序是一个单线程作为应用程序的运行实例的单一的过程运行的。但是，这样子应用程序同时只能执行一个任务。为了同时执行多个任务，它可以被划分为更小的线程。

## 线程生命周期

线程生命周期开始于 System.Threading.Thread 类的对象被创建时，结束于线程被终止或完成执行时。

下面列出了线程生命周期中的各种状态：

  * **未启动状态**：当线程实例被创建但 Start 方法未被调用时的状况。
  * **就绪状态**：当线程准备好运行并等待 CPU 周期时的状况。
  * **不可运行状态**：下面的几种情况下线程是不可运行的：

    * 已经调用 Sleep 方法
    * 已经调用 Wait 方法
    * 通过 I/O 操作阻塞
  * **死亡状态**：当线程已完成执行或已中止时的状况。

## 主线程

在 C# 中，**System.Threading.Thread** 类用于线程的工作。它允许创建并访问多线程应用程序中的单个线程。进程中第一个被执行的线程称为**主线程**。

当 C# 程序开始执行时，主线程自动创建。使用 **Thread** 类创建的线程被主线程的子线程调用。您可以使用 Thread 类的 **CurrentThread** 属性访问线程。

下面的程序演示了主线程的执行：

```C#
using System;
using System.Threading;

namespace MultithreadingApplication
{
    class MainThreadProgram
    {
        static void Main(string[] args)
        {
            Thread th = Thread.CurrentThread;
            th.Name = "MainThread";
            Console.WriteLine("This is {0}", th.Name);
            Console.ReadKey();
        }
    }
}
```

## Thread 类常用的属性和方法

下表列出了 **Thread** 类的一些常用的 **属性**：

| 属性                 | 描述                                             |
|--------------------|------------------------------------------------|
| CurrentContext     | 获取线程正在其中执行的当前上下文。                              |
| CurrentCulture     | 获取或设置当前线程的区域性。                                 |
| CurrentPrinciple   | 获取或设置线程的当前负责人（对基于角色的安全性而言）。                    |
| CurrentThread      | 获取当前正在运行的线程。                                   |
| CurrentUICulture   | 获取或设置资源管理器使用的当前区域性以便在运行时查找区域性特定的资源。            |
| ExecutionContext   | 获取一个 ExecutionContext 对象，该对象包含有关当前线程的各种上下文的信息。 |
| IsAlive            | 获取一个值，该值指示当前线程的执行状态。                           |
| IsBackground       | 获取或设置一个值，该值指示某个线程是否为后台线程。                      |
| IsThreadPoolThread | 获取一个值，该值指示线程是否属于托管线程池。                         |
| ManagedThreadId    | 获取当前托管线程的唯一标识符。                                |
| Name               | 获取或设置线程的名称。                                    |
| Priority           | 获取或设置一个值，该值指示线程的调度优先级。                         |
| ThreadState        | 获取一个值，该值包含当前线程的状态。                             |

下表列出了 **Thread** 类的一些常用的 **方法**：

| 序号 | 方法名 & 描述                                                                                                                                                                                                                                                                                                                                |
|----|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1  | public void Abort\(\)在调用此方法的线程上引发 ThreadAbortException，以开始终止此线程的过程。调用此方法通常会终止线程。                                                                                                                                                                                                                                                        |
| 2  | public static LocalDataStoreSlot AllocateDataSlot\(\)在所有的线程上分配未命名的数据槽。为了获得更好的性能，请改用以 ThreadStaticAttribute 属性标记的字段。                                                                                                                                                                                                                     |
| 3  | public static LocalDataStoreSlot AllocateNamedDataSlot\( string name\) 在所有线程上分配已命名的数据槽。为了获得更好的性能，请改用以 ThreadStaticAttribute 属性标记的字段。                                                                                                                                                                                                    |
| 4  | public static void BeginCriticalRegion\(\)通知主机执行将要进入一个代码区域，在该代码区域内线程中止或未经处理的异常的影响可能会危害应用程序域中的其他任务。                                                                                                                                                                                                                                      |
| 5  | public static void BeginThreadAffinity\(\)通知主机托管代码将要执行依赖于当前物理操作系统线程的标识的指令。                                                                                                                                                                                                                                                              |
| 6  | public static void EndCriticalRegion\(\)通知主机执行将要进入一个代码区域，在该代码区域内线程中止或未经处理的异常仅影响当前任务。                                                                                                                                                                                                                                                    |
| 7  | public static void EndThreadAffinity\(\)通知主机托管代码已执行完依赖于当前物理操作系统线程的标识的指令。                                                                                                                                                                                                                                                                |
| 8  | public static void FreeNamedDataSlot\(string name\)为进程中的所有线程消除名称与槽之间的关联。为了获得更好的性能，请改用以 ThreadStaticAttribute 属性标记的字段。                                                                                                                                                                                                                   |
| 9  | public static Object GetData\( LocalDataStoreSlot slot \) 在当前线程的当前域中从当前线程上指定的槽中检索值。为了获得更好的性能，请改用以 ThreadStaticAttribute 属性标记的字段。                                                                                                                                                                                                        |
| 10 | public static AppDomain GetDomain\(\)返回当前线程正在其中运行的当前域。                                                                                                                                                                                                                                                                                  |
| 11 | public static AppDomain GetDomainID\(\)返回唯一的应用程序域标识符。                                                                                                                                                                                                                                                                                   |
| 12 | public static LocalDataStoreSlot GetNamedDataSlot\( string name \) 查找已命名的数据槽。为了获得更好的性能，请改用以 ThreadStaticAttribute 属性标记的字段。                                                                                                                                                                                                              |
| 13 | public void Interrupt\(\)中断处于 WaitSleepJoin 线程状态的线程。                                                                                                                                                                                                                                                                                    |
| 14 | public void Join\(\)在继续执行标准的 COM 和 SendMessage 消息泵处理期间，阻塞调用线程，直到某个线程终止为止。此方法有不同的重载形式。                                                                                                                                                                                                                                                   |
| 15 | public static void MemoryBarrier\(\)按如下方式同步内存存取：执行当前线程的处理器在对指令重新排序时，不能采用先执行 MemoryBarrier 调用之后的内存存取，再执行 MemoryBarrier 调用之前的内存存取的方式。                                                                                                                                                                                                     |
| 16 | public static void ResetAbort\(\)取消为当前线程请求的 Abort。                                                                                                                                                                                                                                                                                      |
| 17 | public static void SetData\( LocalDataStoreSlot slot, Object data \) 在当前正在运行的线程上为此线程的当前域在指定槽中设置数据。为了获得更好的性能，请改用以 ThreadStaticAttribute 属性标记的字段。                                                                                                                                                                                         |
| 18 | public void Start\(\)开始一个线程。                                                                                                                                                                                                                                                                                                            |
| 19 | public static void Sleep\( int millisecondsTimeout \) 让线程暂停一段时间。                                                                                                                                                                                                                                                                        |
| 20 | public static void SpinWait\( int iterations \) 导致线程等待由 iterations 参数定义的时间量。                                                                                                                                                                                                                                                            |
| 21 | public static byte VolatileRead\( ref byte address \)；public static double VolatileRead\( ref double address \)；public static int VolatileRead\( ref int address \)；public static Object VolatileRead\( ref Object address \) 读取字段值。无论处理器的数目或处理器缓存的状态如何，该值都是由计算机的任何处理器写入的最新值。此方法有不同的重载形式。这里只给出了一些形式。                                    |
| 22 | public static void VolatileWrite\( ref byte address, byte value \)；public static void VolatileWrite\( ref double address, double value \)；public static void VolatileWrite\( ref int address, int value \)；public static void VolatileWrite\( ref Object address, Object value \) 立即向字段写入一个值，以使该值对计算机中的所有处理器都可见。此方法有不同的重载形式。这里只给出了一些形式。 |
| 23 | public static bool Yield\(\)导致调用线程执行准备好在当前处理器上运行的另一个线程。由操作系统选择要执行的线程。                                                                                                                                                                                                                                                                   |

## 创建线程

线程是通过扩展 Thread 类创建的。扩展的 Thread 类调用 **Start()** 方法来开始子线程的执行。

下面的程序演示了这个概念：

```C#
using System;
using System.Threading;

namespace MultithreadingApplication
{
    class ThreadCreationProgram
    {
        public static void CallToChildThread()
        {
            Console.WriteLine("Child thread starts");
        }
        
        static void Main(string[] args)
        {
            ThreadStart childref = new ThreadStart(CallToChildThread);
            Console.WriteLine("In Main: Creating the Child thread");
            Thread childThread = new Thread(childref);
            childThread.Start();
            Console.ReadKey();
        }
    }
}
```

## 管理线程

Thread 类提供了各种管理线程的方法。

下面的实例演示了 **sleep()** 方法的使用，用于在一个特定的时间暂停线程。

```C#
using System;
using System.Threading;

namespace MultithreadingApplication
{
    class ThreadCreationProgram
    {
        public static void CallToChildThread()
        {
            Console.WriteLine("Child thread starts");
            // 线程暂停 5000 毫秒
            int sleepfor = 5000; 
            Console.WriteLine("Child Thread Paused for {0} seconds", 
                              sleepfor / 1000);
            Thread.Sleep(sleepfor);
            Console.WriteLine("Child thread resumes");
        }
        
        static void Main(string[] args)
        {
            ThreadStart childref = new ThreadStart(CallToChildThread);
            Console.WriteLine("In Main: Creating the Child thread");
            Thread childThread = new Thread(childref);
            childThread.Start();
            Console.ReadKey();
        }
    }
}
```

## 销毁线程

**Abort()** 方法用于销毁线程。

通过抛出 **threadabortexception** 在运行时中止线程。这个异常不能被捕获，如果有 _finally_ 块，控制会被送至 _finally_ 块。

下面的程序说明了这点：

```C#
using System;
using System.Threading;

namespace MultithreadingApplication
{
    class ThreadCreationProgram
    {
        public static void CallToChildThread()
        {
            try
            {

                Console.WriteLine("Child thread starts");
                // 计数到 10
                for (int counter = 0; counter <= 10; counter++)
                {
                    Thread.Sleep(500);
                    Console.WriteLine(counter);
                }
                Console.WriteLine("Child Thread Completed");

            }
            catch (ThreadAbortException e)
            {
                Console.WriteLine("Thread Abort Exception");
            }
            finally
            {
                Console.WriteLine("Couldn't catch the Thread Exception");
            }

        }
        
        static void Main(string[] args)
        {
            ThreadStart childref = new ThreadStart(CallToChildThread);
            Console.WriteLine("In Main: Creating the Child thread");
            Thread childThread = new Thread(childref);
            childThread.Start();
            // 停止主线程一段时间
            Thread.Sleep(2000);
            // 现在中止子线程
            Console.WriteLine("In Main: Aborting the Child thread");
            childThread.Abort();
            Console.ReadKey();
        }
    }
}
```
