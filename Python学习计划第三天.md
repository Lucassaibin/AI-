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
命名关键字参数

def functionname(arg1, arg2=v, args, *, nkw, *kw):
       "函数_文档字符串"
       function_suite
       return [expression]

*, nkw - 命名关键字参数，用户想要输入的关键字参数，定义方式是在nkw 前面加个分隔符 *。
如果要限制关键字参数的名字，就可以用「命名关键字参数」
使用命名关键字参数时，要特别注意不能缺少参数名。
2.变量作用域
