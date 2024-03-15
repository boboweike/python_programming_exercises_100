大家好，欢迎回到我们的 Python 编程练习系列课程。今天我们要来解决一个新的问题。这个问题是关于 Python 中的类，这是面向对象编程的一个基本概念。

我们的任务是定义一个至少有两个方法的类。第一个方法，`getString`，可以从控制台输入获取一个字符串。第二个方法，`printString`，将以大写形式打印出字符串。

[这边我建议你暂停视频，先自己思考一下如何实现，最好能自己把 Python 代码写出来]

好，下面我来编写代码。

```python
# 定义一个名为 MyClass 的类
class MyClass:
    # __init__ 是一个特殊的方法，被称为类的构造函数或初始化方法
    # 当我们创建类的新实例时，Python 会自动调用这个方法
    def __init__(self):
        # 在这个方法中，我们创建了一个名为 my_string 的实例变量，并将其初始值设置为空字符串
        self.my_string = ""

    # 定义一个名为 getString 的方法，用于从控制台获取输入
    def getString(self):
        # 使用 input 函数获取用户输入，并将其存储在 my_string 变量中
        self.my_string = input("请输入一个字符串：")

    # 定义一个名为 printString 的方法，用于打印大写的字符串
    def printString(self):
        # 使用 upper 方法将 my_string 变量中的字符串转换为大写，然后打印出来
        print(self.my_string.upper())
```

总结一下：在这段代码中，我们首先定义了我们的类`MyClass`。在类内部，我们有一个`__init__`方法，这是 Python 类中的一个特殊方法，被称为构造函数。当从类创建对象时，会调用此方法，它允许类初始化类实例的属性。

然后我们定义了两个方法。`getString`使用`input`函数获取控制台输入，并将它赋值给`my_string`。`printString`使用`upper`方法以大写形式打印`my_string`。

下面我们来测试一下我们的类，我这边直接拷贝代码：

```python
# 创建 MyClass 类的一个实例
test = MyClass()
# 调用 getString 方法获取用户输入
test.getString()
# 调用 printString 方法打印大写的字符串
test.printString()
```

在这个测试中，我们首先创建了一个`MyClass`的对象`test`。然后我们调用`getString`方法获取输入，再调用`printString`方法以大写形式打印它。

下面我来运行一下这个程序，输入"test MyClass"，结果输出也是`test MyClass`，结果正确。

这就是这个练习的全部内容！我们学习了 Python 的类、方法、`input`函数和`upper`方法。

感谢观看，记得点赞和订阅波波微课频道，我们下节课再见。
