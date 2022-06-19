The content in [[LectureList#Lecture-5 Systems Modelling|Lecture-5]]

UML 主要由两个部分组成，一个是 Structure，另一个是 Behavior
Structure 由闭合图形表示，包括 Class、Component、Object、Package 等
Behavior 由带箭头或其他符号的线表示，包括 Sequence、Communication、Activity、Use Case 等

## Structural Perspective

UML 类图表示的是系统组织的静态关系
主要有以下几种成分，
Structure：Class、Abstract Class、Interface
Behavior：Generalization、Association、Dependency、Realization、Composition、Aggregation

![image-20220619162501704](https://raw.githubusercontent.com/Anxiu0101/PicgoImg/master/202206191626062.png)

### Structure

### Behavior

#### Generalization

Generalization represents an “is-a” relationship. In this example, it can be read as a Manager is a type of User; a Developer is a type of User. The children class (Manager and Developer) automatically inherits the properties of their parent class. 
泛化表示“is-a”关系。 在本例中，可以将 Manager 理解为 User 的一种类型； 开发人员是一种用户。 子类（Manager 和 Developer）自动继承其父类的属性。

```puml
class User {
	id uint
	name string
}

class 
```

#### Association
#### Dependency
#### Realization
#### Composition
#### Aggregation
