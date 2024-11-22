## 长沙理工大学 Python 选修课计算器大作业

### 项目背景
随着编程教育的发展，Python作为一门简单易学的编程语言，被广泛应用于各个领域。为了帮助学生理解Python的基本语法和逻辑结构，长沙理工大学开设了Python选修课程。本次大作业旨在通过实现一个计算器，巩固学生的编程基础，提升解决实际问题的能力。

### 项目目标
1. **基本功能实现**：设计一个能够进行加、减、乘、除四则运算的计算器。
2. **用户交互**：实现简单的命令行界面，让用户能够输入计算表达式并获得结果。
3. **异常处理**：处理用户输入中的异常情况，如除以零、非法字符等，确保程序的鲁棒性。
4. **扩展功能**：允许用户添加额外功能，例如支持括号运算、幂运算等。

### 技术要求
- 使用Python 3.x进行开发。
- 遵循PEP 8编码规范，确保代码的可读性和可维护性。
- 需要编写基本的单元测试来验证计算器的功能。

### 项目模块
1. **主程序模块**：
   - 负责接受用户输入，并调用计算功能。
2. **计算核心模块**：
   - 实现各类运算的逻辑，包括基本的加减乘除和扩展的复杂运算。
3. **异常处理模块**：
   - 负责捕获并处理用户输入时可能出现的各种错误。
4. **测试模块**：
   - 包含单元测试，确保各个模块功能的正确性。

### 示例代码
下面是一个简单的结构示例，展示计算器的基本框架：

```python
def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y == 0:
        raise ValueError("Cannot divide by zero!")
    return x / y

def calculator():
    print("欢迎使用计算器！")
    while True:
        try:
            expression = input("请输入计算表达式 (或输入 'exit' 退出): ")
            if expression.lower() == 'exit':
                break
            # 在此处解析并计算表达式
            result = eval(expression)  # 注意：eval需谨慎使用。
            print(f"结果: {result}")
        except Exception as e:
            print(f"错误: {e}")

if __name__ == "__main__":
    calculator()
```

### 评估标准
- 功能实现（包括基本运算和扩展功能）。
- 代码的清晰度和规范性。
- 异常处理的有效性。
- 提交的项目文档，包括用户手册和开发文档。

### 项目时间表
- **项目启动**：2024年11月
- **项目提交**：2024年12月初

### 总结
本项目不仅是一次编程实践的机会，也是学生深入理解Python编程基础的重要步骤。通过完成计算器大作业，学生可以提升自己的逻辑思维能力和问题解决能力，为以后更复杂的项目打下坚实基础。

如需进一步讨论项目细节或有其他问题，请随时联系！
