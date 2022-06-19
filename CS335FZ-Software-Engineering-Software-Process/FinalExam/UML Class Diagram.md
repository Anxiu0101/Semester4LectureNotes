The content in [[LectureList#Lecture-5 Systems Modelling|Lecture-5]]

UML 主要由两个部分组成，一个是 Structure，另一个是 Behavior
Structure 由闭合图形表示，包括 Class、Component、Object、Package 等
Behavior 由带箭头或其他符号的线表示，包括 Sequence、Communication、Activity、Use Case 等

## Structural Perspective

UML 类图表示的是系统组织的静态关系
主要有以下几种成分，
Structure：Class、Abstract Class、Interface
Behavior：[[#Generalization]]、[[#Dependency]]、[[#Realization]]、[[#Association Aggregation and Composition]]

![image-20220619162501704](https://raw.githubusercontent.com/Anxiu0101/PicgoImg/master/202206191626062.png)

### Structure

### Behavior

#### Generalization

Generalization represents an “is-a” relationship. In this example, it can be read as a Manager is a type of User; a Developer is a type of User. The children class (Manager and Developer) automatically inherits the properties of their parent class. 
泛化表示“is-a”关系。 在本例中，可以将 Manager 理解为 User 的一种类型； 开发人员是一种用户。 子类（Manager 和 Developer）自动继承其父类的属性。  
这种关系在 UML 中使用 空心三角箭头表示。

```puml
class User {
	+ id uint
	+ name string
	--Get Set Method--
	+ getName() string
}

class Manager {
	+ Authority int
	--Get Set Method--
	+ getAuthority() int
}

class Developer {
	+ Level int
	--Get Set Method--
	+ getLevel() int
}

Manager --|> User
Developer --|> User
```

#### Dependency

Dependency represents the relationship between entities in which if the changes to the definition of one entity may cause changes to the other entities. This can be `<<use>>, <<import>>, <<depend>>, <<refine>>, <<extend>>, <<include>>, <<access>>, <<instanceOf>>, <<bind>>, <<instantiate>>, etc.`  
依赖关系表示实体之间的关系，如果对一个实体的定义进行更改，可能会导致对其他实体的更改。  
```puml
class Main {
	+ main()
}

Main ..> java.util.Scanner: <<import>>
```

#### Realization

In a realization relationship, an `<<interface>>` stereotype is used to create an interface and to realize the particular interface.  
在实现关系中，`<<interface>>` 构造型用于创建接口并实现特定接口。

```puml
interface IRouter {
	+ GET(string, HandlerFunc) IRouter
	+ POST(string, HandlerFunc) IRouter
}

class GroupRouter {
}

GroupRouter ..|> IRouter
```

#### Association, Aggregation and Composition

$$Composition \subset Aggregation \subset Association$$

An Association relationship represents connections or associations between object in the system. 关联关系代表系统中对象之间的连接或关联。

```puml
class Teacher{}
class Student{}

Student "1..*"-"1..*" Teacher
```

An Aggregation is a subtype of an association relationship. It can be described as a ‘part of’ relationship. In Aggregation relationship, objects have separate lifetimes. 聚集是关联关系的子类型。 它可以被描述为“关系的一部分”。 在聚合关系中，对象具有单独的寿命。
例子中，轮子属于车子的一部分，但是不会因为车子的消失而消失，作为客观的一部分实体存在

```puml
class Car{}
class Wheel{}

Wheel --o Car
```

A Composition is a subtype of an aggregation relationship. It represents a ‘whole/part’ relationship. If a composite is removed, all its associated parts will also be removed with it. 组成是聚集关系的亚型。 它代表了“整体/部分”的关系。 如果删除了复合材料，则其所有相关零件也将使用它去除。

```puml
class Person{}
class Heart{}

Heart --* Person
```






