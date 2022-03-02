## 一、异常处理

我们在编写程序时，会存在许多错误而使程序无法继续，`try`很好的解决了这个问题

**常见内置异常类型**

|异常类型|作用
|--------|----
|ArithmeticError|所有数值计算异常的基类
|EOFError|没有内建输入,到达EOF 标记
|NameError|未声明/初始化对象 (没有属性)
|SyntaxError|Python 语法错误
|IndentationError|	缩进错误
|Exception|常规错误的基类
|IOError|	输入/输出操作失败
|KeyError|	映射中没有这个键
|IndexError|序列中没有此索引(index)
|TypeError|	对类型无效的操作
|ZeroDivisionError|	除(或取模)零 (所有数据类型)
|ValueError|传入无效的参数

<details><summary>格式查看</summary>
<pre><code>try:
    可能异常的代码
except 异常类型A:
    处理异常代码A
except 异常类型B:
    处理异常代码B
...
except:
    前面未捕抓到的异常
else:
    未发生异常处理的代码，可选择写不写
finally:
    无论如何都要执行的代码，可选择写不写
</code></pre>
</details>

例如:
```
try:
    a = 10
    b = 0
    print(a / b)
except ZeroDivisionError:
    print("除数不能为零")
```
用try来检查代码是否有异常(`try`必须和`except`配合使用)

用`except 异常类型:`来处理异常状态，例如:`ZeroDivisionError`在正常情况下除零时，代码会报错，而使用try后，就会打印`除数不能为零`

时间问题以后列举

## 二、主动异常

主动异常:raise,assert

**[返回目录](https://github.com/3114aaa/Python-directory)
[下一章](https://github.com/3114aaa/Python-3)**
