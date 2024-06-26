# 习题二

### 第一题
1. 创建一个泛型函数 `print_info`，它接受一个实现了 `Debug` 特征的参数，并打印出该参数的调试信息。这个函数应该能够处理任何实现了 `Debug` 特征的类型。
2. 创建一个泛型函数 `largest`，它接受一个任意类型的切片，并返回切片中最大的元素。要求这个函数只能用于元素类型实现了 `PartialOrd` 和 `Copy` 特征的情况。

### 第二题
1. 定义一个名为 `Drawable` 的特征，它包含一个名为 `draw` 的方法。然后定义两个结构体 `Circle` 和 `Square`，并为它们实现 `Drawable` 特征。
2. 创建一个名为 `display` 的函数，它接受一个实现了 `Drawable` 特征的参数。在这个函数内部，调用传入参数的 `draw` 方法。

### 第三题
用`Rust`写一个冒泡排序函数，要求支持范型，并支持指定按`升序`、`降序`排序。

### 第四题
1. 设计一个名为 `divide` 的函数，它接受两个`f64`类型的参数，返回类型为`Result<f64, String>` 。当除数为零时，函数应返回一个描述错误的字符串。
2. 设计一个名为`get_first`的函数，它接受一个 `Vec<i32>` 并返回一个 `Option<i32>`，如果向量为空，则返回 `None`。
3. 对于上面这个函数，编写代码示例，展示如何使用 `match`表达式来处理`divide`和`get_first`函数的返回值。进一步，展示如何使用`map、and_then、or_else`等组合操作符来优化处理`Option`和`Result`的代码。

### 第五题
编写一个函数，它尝试执行多个可能失败的操作，并返回一个错误类型为 `Box<dyn Error>`的`Result`。展示如何在一个函数中处理不同类型的错误，并返回统一的错误类型。
