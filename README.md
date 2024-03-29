# 设计模式

+ 优点
  + 解耦： 降低代码之间的耦合度，使之更容易维护和扩展。
  + 灵活性
  + 可扩展性

+ 缺点
  + 可能会导致潜在的性能损失
  + 增加复杂性

> 单例模式优缺点相反

# 创建型
+ Builder:
  + 当你需要创建一个复杂对象，它有许多属性，并且希望有一个清晰的方法一步步构建此对象时，可以选择Builder模式。这对于提高代码的可读性和易用性很有帮助。

  + 构建复杂对象时，特别是当对象包含多个属性，有些属性可能是可选的，不需要全部设置。
  + 当创建对象的过程需要分步骤进行，且每个步骤都需要清晰地定义。

+ Abstract Factory:
  + 当你需要提供一个接口用于创建一系列相关或相互依赖的对象，而无需指定它们具体的类时，可以选择Abstract Factory模式。这有助于代码解耦和扩展性。

  + 当有一组相互关联的对象需要一起使用，并且希望确保客户端不与具体类耦合。
  + 当有多个产品系列，并且系统只应在配置时或运行时一次性地使用其中一个系列。

+ Factory Method:
  + 当要提供一个用于创建对象的接口，让子类决定实例化哪一个类时，可以选择Factory Method模式。这有助于将对象的创建延迟到子类进行。

  + 当一个类无法预料它所需创建对象的类别，以及希望其子类来指定所创建的对象。
  + 当类想由其子类来指定创建的对象时。
  > 和 Abstract Factory 的区别是创建一个对象而不是一系列对象

+ Prototype:
  + 当需要复制或克隆对象，而不是每次都创建新实例时，可以选择Prototype模式。这可以加快创建对象的速度，尤其是对于复杂对象的实例化非常耗时时。

  + 当需要避免创建一个与产品层次平行的工厂层次时。
  + 当一个类的实例只有几个不同状态的组合中的一种，建立相应数目的原型并克隆它们可能比每次用适当的状态手动实例化该类更方便。

+ Singleton:
  + 当要确保一个类只有一个实例，并且提供一个全局访问点时，可以选择Singleton模式。

  + 当确切地知道只需要一个实例，并且需要一个全局访问点以外的额外功能。
  + 当单个实例应该是可扩展的，并且客户应能够使用一个扩展的实例而不必修改代码。

# 结构型
+  Adapter *
  + 当想要使现有的类与其他的接口兼容，或者提供一个统一的接口以供不同的实现类使用时，使用Adapter模式。

  + 需要使用现有类的功能，而这些类的接口不符合当前系统的接口标准。
  + 需要创建一个可以透明地与多个不同的客户端或离散系统互操作的重用类。

+ Bridge
  + 当希望将抽象与其实现分离, 以便两者可以独立变化时，使用Bridge模式。

  + 不希望在抽象和实现二者之间有固定的绑定关系，如实现可能在运行时切换。
  + 类的抽象以及其实现都应该可以通过生成子类的方式独立地扩展。

+ Composite
  + 当需要表示对象的部分-整体层次结构时，使用Composite模式。它可以使你对单个对象和组合对象的操作具有一致性。

  + 希望客户端可以忽略组合对象与单个对象的差异。
  + 在有树形结构的场合，用以表示整体与部分的关系。

+ Decorator
  + 当不通过子类化的方式来扩充对象的功能，而是希望在运行时添加职责时，使用Decorator模式。

  + 当系统需要新功能时，为避免使用大量子类来扩展对象功能。
  + 当需要动态地给一个对象添加功能，这些功能可以再动态地撤销。

+ Facade
  + 当需要提供一个简单的界面以隐藏复杂的系统，如一组不相关的类、一个复杂的类库或框架时，使用Facade模式。

  + 提供一个简单的或层次化的入口点去访问子系统。
  + 当需要解耦一个复杂系统以增加子系统的独立性和可移植性。

+ Flyweight
  + 当有大量相似对象，想要减少存储开销，进行内存共享时，使用Flyweight模式。

  + 当程序需要大量对象，这些对象有许多共同的特性，从而引入许多细粒度的对象来表示。
  + 当由于使用了大量的对象，造成很大的存储开销时。

+ Proxy *
  + 当需要一个替身或占位符来代表一个真实对象进行访问或控制时，使用Proxy模式。

  + 当需要为一个对象提供一个替代者或占位符以访问它，例如远程代理（Remote Proxies）、虚拟代理（Virtual Proxies）或保护代理（Protection Proxies）。
  + 当需要添加一些管理操作，但不想改变真实对象的类。

# 行为型