# AI-
1.Python函数定义的可变参数

顾名思义，可变参数就是传入的参数个数是可变的，可以是 0, 1, 2 到任意个，是不定长的参数。

def functionname(arg1, arg2=v, *args):
       "函数_文档字符串"
       function_suite
       return [expression]

*args - 可变参数，可以是从零个到任意个，自动组装成元组。
加了星号（*）的变量名会存放所有未命名的变量参数。
4. 关键字参数

def functionname(arg1, arg2=v, args, *kw):
       "函数_文档字符串"
       function_suite
       return [expression]

**kw - 关键字参数，可以是从零个到任意个，自动组装成字典。
3命名关键字参数

def functionname(arg1, arg2=v, args, *, nkw, *kw):
       "函数_文档字符串"
       function_suite
       return [expression]

*, nkw - 命名关键字参数，用户想要输入的关键字参数，定义方式是在nkw 前面加个分隔符 *。
如果要限制关键字参数的名字，就可以用「命名关键字参数」
使用命名关键字参数时，要特别注意不能缺少参数名。
2.变量作用域
匿名函数的定义
在 Python 里有两类函数：

第一类：用 def 关键词定义的正规函数
第二类：用 lambda 关键词定义的匿名函数
Python 使用 lambda 关键词来创建匿名函数，而非def关键词，它没有函数名，其语法结构如下：

lambda argument_list: expression

lambda - 定义匿名函数的关键词。
argument_list - 函数参数，它们可以是位置参数、默认参数、关键字参数，和正规函数里的参数类型一样。
:- 冒号，在函数参数和表达式中间要加个冒号。
expression - 只是一个表达式，输入函数参数，输出一些值。
注意：

expression 中没有 return 语句，因为 lambda 不需要它来返回，表达式本身结果就是返回值。
匿名函数拥有自己的命名空间，且不能访问自己参数列表之外或全局命名空间里的参数。
类与对象
Python 的魔法方法¶
据说，Python 的对象天生拥有一些神奇的方法，它们是面向对象的 Python 的一切...

它们是可以给你的类增加魔力的特殊方法...

如果你的对象实现了这些方法中的某一个，那么这个方法就会在特殊的情况下被 Python 所调用，而这一切都是自动发生的...

类有一个名为__init__(self[, param1, param2...])的魔法方法，该方法在类实例化时会自动调用。
