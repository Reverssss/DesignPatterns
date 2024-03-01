# 定义
+ 享元模式（Flyweight Pattern）
+ 通过共享对象来减少创建对象的个数，从而提高性能。
+ 享元模式适用于那些可以共享相同状态的对象。

# 优点
+ 减少内存使用： 享元模式可以减少内存使用，因为共享对象可以被多个客户端使用。
+ 提高性能： 享元模式可以提高性能，因为创建对象通常比查找和使用共享对象要耗时。
+ 简化代码： 享元模式可以简化代码，因为你不需要为每个对象都创建和管理一个单独的实例。

# 缺点
+ 潜在的性能损失： 享元模式可能会导致潜在的性能损失，因为你需要在每次使用共享对象时都进行查找。
+ 增加复杂性： 享元模式可能会增加代码的复杂性，尤其是当共享对象的状态很复杂时

# 使用情形
+ Singleton
+ 通过这种方式，Spring实现了类似Flyweight模式的共享机制，有效地减少了同一类型的对象创建的数量