# SDSR-OCT 代码学习

**def**

使用 `def` 开始函数定义，紧接着是函数名，'parameters ' 为函数的参数，内部为函数的具体功能实现代码，如果想要函数有返回值, 在 `expressions` 中的逻辑代码中用 `return` 返回。

```python
def function_name(parameters):
    expressions
```

实例：

```python
def func(a,b):
    c=a+b
    print('the c is ', c)
```

定义一个加法函数，a和b是带传入的参数值，函数的功能就是把a和b加起来。运行脚本后，在 Python 提示符内调用函数 `func`, 如果不指定参数 `func()`, 那么将会出错; 输出 `func(1, 2)`，将 `a=1, b=2` 传入函数，输出 `the c is 3` 。

**super**

**super()**方法设计目的是用来解决多重继承时父类的查找问题，可避免直接使用父类的名字



**argparse**   命令行选项、参数和子命令解析器

-- 创建解析器 --

```Python
ap= argparse.ArgumentParser(description='Process some integers.')
```

ArgumentParser 对象包含将命令行解析成 Python 数据类型所需的全部信息。

--添加参数--

```Python
ap.add_argument('integers', metavar='N', type=int, nargs='+', help='an integer for the accumulator')
```

给一个 ArgumentParser 添加**程序参数信息**是通过调用 add_argument() 方法完成的。

其中给属性名前面添加“--”，可以将它变成可选参数。

![image-20210510175633542](C:\Users\striv\AppData\Roaming\Typora\typora-user-images\image-20210510175633542.png)

