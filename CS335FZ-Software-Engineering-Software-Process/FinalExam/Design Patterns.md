
## Singleton Pattern

## Factory Method Pattern

## Facade Pattern

## Adapter Pattern

Convert the interface of a class into another interface clients expect. Adapter lets classes work together that couldn't otherwise because of incompatible interfaces. 将一个类的接口转化成所需的另一个预期接口。适配器使得那些因为接口不兼容的类共同工作。

使用场景：
- Use an existing class, but its interface does not match the one you need. 
- Create a reusable class that cooperates with unrelated or unforeseen classes, that is, classes that don't necessarily have compatible interfaces.
- Use several existing subclasses, but it's impractical to adapt their interface by subclassing everyone. An object adapter can adapt the interface of its parent class.

其实理解起来不难，就像电源适配器一样，适配器的使用就是既能干一件事情，又能干另一件事情的存在。

具体案例：
- Multiple database accessors 
- Use toolkit classes that have incompatible interfaces
- Other generic issues related to bridge incompatible interfaces 
	- E.g., cell phone chargers & adapters, memory card adapters, electrical plugs and adapters, etc.

## Observer Pattern