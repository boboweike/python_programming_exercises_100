# 习题 2

大家好，欢迎回到我们的 Python 编程练习系列课程。

今天的任务是编写一个 Python 程序，可以计算给定数字的阶乘。结果应该打印在一行上。例如，如果我们输入数字 8，输出应该是 40320。

一个数字的阶乘是所有小于或等于该数字的正整数的乘积。所以，我们需要将从 1 到给定数字中的所有数字进行相乘。

好，下面我来给出解决这个问题的 Python 代码。我将提供非递归和递归两种解决办法。

先给出非递归的解决办法：

```python
# 非递归实现
# 非递归实现
def compute_factorial_non_recursive(n):
    # 将结果初始化为1
    result = 1

    # 将1到n的所有数字相乘
    for i in range(1, n + 1):
        result *= i

    # 打印结果
    return result


# 用测试输入调用函数并输出结果
print(compute_factorial_non_recursive(8))
```

我重新总结一下上面的解决办法。在这个函数`compute_factorial_non_recursive`中，我们首先将`result`初始化为 1。然后我们将从 1 到`n`的所有数字相乘，并更新`result`。最后，我们返回结果`result`。

现在，我来编写递归解决办法：

```python
# 递归实现
def compute_factorial_recursive(n):
    # 基本情况：1的阶乘是1
    if n == 1:
        return 1

    # 递归情况：n的阶乘 = n乘以(n-1)的阶乘
    else:
        return n * compute_factorial_recursive(n - 1)


# 用测试输入调用函数并打印结果
print(compute_factorial_recursive(8))
```

我重新总结一下上面的解决方案。在递归函数`compute_factorial_recursive`中，我们有一个基本情况，如果`n`是 1，我们返回 1。对于递归情况，我们返回`n`乘以`n-1`的阶乘。

让我们用测试输入 8 运行代码。你可以看到，两个函数都打印出 40320，这是 8 的阶乘。

现在，让我们编写一个单元测试来验证我们的解决方案，那么这边为了节省时间，我直接拷贝代码：

```python
# 单元测试代码
def test_compute_factorial():
    assert compute_factorial_non_recursive(5) == 120
    assert compute_factorial_non_recursive(6) == 720
    assert compute_factorial_non_recursive(7) == 5040
    assert compute_factorial_non_recursive(8) == 40320

    assert compute_factorial_recursive(5) == 120
    assert compute_factorial_recursive(6) == 720
    assert compute_factorial_recursive(7) == 5040
    assert compute_factorial_recursive(8) == 40320


# 运行单元测试
test_compute_factorial()
```

在这个单元测试中，我们检查`compute_factorial_non_recursive`和`compute_factorial_recursive`函数，对于输入数字 5、6、7 和 8，能否返回正确的阶乘。如果函数工作正常，测试将通过，不会有任何错误。

在这个练习中，我们学习了 Python 的`for`循环，并学习了如何非递归和递归地计算一个数字的阶乘。这些也是你在 Python 编程中会经常使用的基本概念。

这就是这次的练习。希望对你有帮助。感谢观看，记得点赞和订阅波波微课频道，我们下节课再见。
