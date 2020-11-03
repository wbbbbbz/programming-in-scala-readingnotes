# 1 一门可伸缩的语言

> The name Scala stands for "scalable language." The language is so named because it was designed to grow with the demands of its users.
>设计目标随着用户的需求一起成长

- Scala中的Map，BigInt，akka框架下的receive方法等，都不是Scala语言本身提供的。只是库中的方法。所以Scala可以被培育使用与各类场景。

## 1.2 是什么让Scala 能屈能伸？

> 在Scala 中，函数值就是对象，而函数的类型是可被子类集成的类。
- 函数式编程语言例子：
  - Lisp，Scheme，SML，Erlang，Haske ll，OCaml，F#
- 函数式编程两大核心理念
  - 函数式一等(first-class)的值，类似于整数和字符串。
  - 程序中的操作应该将输入值映射成输出值，而不是当场（in place）修改数据。不可变数据结构是函数式编程的基石之一。
    - 这个核心理念的另一种表述是方法不应该有副作用（side effect）。方法只能通过接收入参和返回结果这两种方式与外部环境通信。像这样的方法被认为是“指称透明的” （referential transparent），意思是对于任何给定的输入，该方法调用都可以被其结果替换，同时不会影响程序的语义。
    - 函数式编程鼓励不可变数据结构和指称透明的方法。

## 1.3 为什么要用Scala?
> 兼容性、精简性、高级抽象和静态类型。

- 兼容性
  - 与Java的无缝互调。编译成JVM字节码，性能与Java程序相当
  - 对Java原生的类型进行再包装。通过隐式转换(implicit conversion)
- 精简性
  - 避免了Java 程序中常见的一些样板（boilerplate）代码。
  - 类型推断
  - 强大类库
- 高级抽象
  - Scala 的函数字面量非常轻，因此经常被使用
- 静态类型
  - 很好地解决了静态类型的两个常见的痛点：通过类型推断规避了过于唠唆的问题，通过模式匹配以及其他编写和组合类型的新方式避免了死板
  - 可验证性质：静态类型系统可以证明某类运行期错误不可能发生
  - 安全的重构：静态类型系统提供了一个安全网，让你有十足的信心和把握对代码库进行修改。
  - 文档：静态类型是程序化的文档，编译器会检查其正确性。
