大家好，欢迎回到我们的《100 个 Python 编程练习题》系列课程。今天我们要解决的是第 14 题，也是一个二级难度的题目。

问题是这样的：编写一个程序，接受一个句子，并计算大写字母和小写字母的数量。假设我们输入的是 "Hello world!"，那么输出应该是：大写字母 1 个，小写字母 9 个。

下面我们开始来编写解决这个问题的 Python 代码。

```python
# 定义一个函数，接受一个句子，并计算大写字母和小写字母的数量
def count_letters(sentence):
    # 初始化大写字母和小写字母的数量
    upper_case = 0
    lower_case = 0
    # 遍历句子中的每一个字符
    for char in sentence:
        # 如果字符是大写字母，大写字母的数量加1
        if char.isupper():
            upper_case += 1
        # 如果字符是小写字母，小写字母的数量加1
        elif char.islower():
            lower_case += 1
    # 返回大写字母和小写字母的数量
    return upper_case, lower_case

# 输入一个句子
sample_sentence = "Hello world!"
# 调用函数，计算大写字母和小写字母的数量
upper_case_result, lower_case_result = count_letters(sample_sentence)
# 打印结果
print("UPPER CASE", upper_case_result)
print("LOWER CASE", lower_case_result)
```

在这段代码中，我们首先定义了一个函数`count_letters`，它接受一个句子，并计算大写字母和小写字母的数量。然后我们初始化大写字母和小写字母的数量为 0，再遍历句子中的每一个字符，如果字符是大写字母，那么大写字母的数量加 1，如果字符是小写字母，那么小写字母的数量加 1。最后，我们返回大写字母和小写字母的数量。

我们用题目中给出的例子来测试一下我们的代码：预期的输出是大写字母 1 个，小写字母 9 个。

```python
# 测试
# 预期输出：大写字母1个，小写字母9个
```

这个问题主要涉及到 Python 的字符串处理，主要是`isupper`和`islower`两个方法。

记住，编程需要不断的学习和练习。

感谢观看，记得点赞和订阅波波微课频道，我们下节课再见。
