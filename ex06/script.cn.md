大家好，欢迎回到我们的 Python 编程练习系列课程。今天我们要解决一个稍微复杂一点的问题。不过别担心，我会一步步引导大家来解决这个问题。

```py
"""
习题6(level 2)

写一个程序，根据给定公式计算结果并打印输出，
Q = [(2 * C * D) / H]的平方根，
其中C和H是常量, C = 50, H = 30，
D是变量，由用户通过控制台输入，输入可以由多个通过逗号分隔。

示例：
输入: 100,150,180
输出: 18,22,24
"""
```

今天我们的任务是编写一个程序，根据给定的公式计算并打印值：Q 等于[(2 * C * D) / H]的平方根。这里，C 是 50，H 是 30。D 是一个变量，它的值应该以逗号分隔的序列输入到我们的程序中。

[这边我建议你暂停视频，先自己思考一下如何实现，最好能自己把 Python 代码写出来]

好，下面我给出我的实现代码：

```python
# 导入math模块以使用sqrt函数
import math

# 定义常量c和h
c = 50
h = 30

# 定义结果列表
result = []

# 要求用户输入d的值，用逗号分隔，并将此输入分隔成数字列表
d_values = input("请输入D的值，用逗号分隔：").split(',')

# 遍历d_values中的每一个d，使用给定的公式计算q，添加到结果列表中
for d in d_values:
    q = math.sqrt((2 * c * int(d)) / h)
    q = round(q)
    result.append(str(q))

# 以逗号分隔的形式打印输出
print(", ".join(result))
```

再重复总结一下：在这段代码中，我们首先导入了`math`模块，这样可以使用求平方根`sqrt`函数。然后我们定义了常量 c 和 h。我们要求用户输入 d 的值，用逗号分隔，并将此输入用逗号分割成数字列表。然后我们遍历 d 的每个值，使用给定的公式计算 q，并打印 q 的四舍五入值。

下面我用问题中给出的例子来测试我们的代码：d 的值是分别是 100，150 和 180。输出应该是分别是 18，22，24。

```python
# 测试
# 输入：100,150,180
# 预期输出：18,22,24
```

这个问题主要涉及到 Python 的数学模块，字符串分割方法`split`，`for` 循环，和 `round` 函数的使用。

好的，今天的课程就到这里。我希望对大家有帮助。感谢观看，记得点赞和订阅波波微课频道，我们下节课再见。
