# 抽象工厂模式
+ 定义：它提供了一个创建一系列相关或依赖对象的接口，而无需指定创建对象的具体类。
+ 优点：
  + 抽象工厂模式可以使代码更易于维护和扩展。
  + 抽象工厂模式可以隐藏创建对象的细节，使代码更易于理解。
  + 抽象工厂模式可以使代码更易于扩展，因为每次添加一个新的产品族时，只需要修改相应的工厂类即可。
+ 缺点：
  + 抽象工厂模式可能会导致代码过于分散，难以管理。

# 工厂方法模式
+ 定义：它定义了一个创建对象的接口，但由子类决定要创建哪种对象。
+ 优点：
  + 工厂方法模式可以使代码更易于维护和扩展。
  + 工厂方法模式可以隐藏创建对象的细节，使代码更易于理解。
  + 工厂方法模式可以使代码更易于扩展，因为每次添加一个新的产品类时，只需要修改相应的子类即可。
+ 缺点：
  + 工厂方法模式可能会导致代码过于分散，难以管理。

# 区别
+ 抽象工厂模式提供了一个创建一系列相关或依赖对象的接口，而工厂方法模式只提供了一个创建对象的接口。
+ 抽象工厂模式由子类来创建对象，而工厂方法模式由工厂类来创建对象。
+ 抽象工厂模式可以使代码更易于维护和扩展，而工厂方法模式可以使代码更易于理解和扩展。