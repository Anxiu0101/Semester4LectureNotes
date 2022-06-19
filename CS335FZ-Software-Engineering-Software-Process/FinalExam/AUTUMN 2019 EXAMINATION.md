## Q1
One essential and widely used model in software engineering is the Waterfall Model.
1. Outline each stage of the Waterfall model and discuss its advantages and drawbacks. [20 marks]
2. What kind of software projects are often organised based on the Waterfall model? [5 marks]

### Q1.1

> [[Waterfall Model]]

![image-20220618054810922](https://raw.githubusercontent.com/Anxiu0101/PicgoImg/master/202206180548571.png)

There are five stage of the Waterfall model, 

1. Requirements Definition
2. System & Software Design
3. Implementation & Unit Testing
4. Integration & System Testing
5. Operation & Maintenance

And the Advantages of the Waterfall model are, 

### Q1.2
![image-20220618055147982](https://raw.githubusercontent.com/Anxiu0101/PicgoImg/master/202206180551049.png)

## Q2
Consider the following specification text: ‘‘John is a computer user who wants to check his email using the Thunderbird email application. When he clicks on the ‘Get Messages’ button, the server will send any unsent emails. It then checks for new emails and the server returns a corresponding response. If there are new emails, these will then be downloaded and displayed.”
1. Draw a sequence diagram based on the specification above. [10 marks]
2. Draw a collaboration diagram based on the specification above [10 marks]
3. Highlight the main differences between a sequence and a collaboration diagram. You may reference your answers to a) and b) above. [5 marks]

### Q2.1
>  [[Sequence Diagram]]
```puml
skinparam sequenceMessageAlign center
autonumber
John -> Thunderbird: Get Messages
Thunderbird -> John: send unsent emails
Thunderbird -> Server: Checks for new emails
alt new emails
	Server -> Thunderbird: Downloaded and displayed
else no new email
	Server -> Thunderbird: A corresponding response
end
```

### Q2.2
> [[Collaboration Diagram]]


### Q2.3

The difference between sequence diagram and collaboration diagram is that, 



## Q3

1. Describe the different types of relationship between classes in a UML Class Diagram and create an example for each in UML (association, aggregation, composition, inheritance). [12 marks]
2. Using an ATM as an example, describe three functional requirements and two non-functional requirements. [5 marks]
3. Describe a scenario, based on a concrete example, where the adapter design pattern is needed. [8 marks]

### Q3.1

> [[UML Class Diagram#Association Aggregation and Composition|Relation]]  
> [[UML Class Diagram#Generalization|Inheritance]]  

### Q3.2

> [[Functional Requirements and Non-functional Requirements]]

Functional requirements: 
- User can take money form ATM
- User can store money on ATM
- User can check his balance in account

Non-functional requirements: 
- Server and database should open the session to keep if one step fail, the data can return to the original state.
- The system shall collect up to 15,000 even/sec from approximately 300 web servers.

### Q3.3

> [[Design Patterns#Adapter Pattern|Adapter Pattern]]

scenario: Multiple database accessors.
I'm using gorm on my development now. It's an ORM library, and you can use it connect to databases include mysql, postgresql, sqlite and so on.
But all the data send and return as a map type. And we should use the adapter to translate it to different format message and pass to different databases. In that case, we will use a same api to deal with different response from database.

## Q4

The table below shows activities, their duration, and activity interdependencies.

![image-20220619201351688](https://raw.githubusercontent.com/Anxiu0101/PicgoImg/master/202206192013813.png)

1. Given this information, draw the corresponding activity network. You can assume that the project start date is today. Clearly highlight the critical path in your diagram. [15 marks]
2. In relation to software project management, what is: 
	1. a milestone
	2. a deliverable
3. What is risk management and what typical activities does risk management involve? [5 marks]

### Q4.1

### Q4.2

> [[Project Management#Milestones and Deliverables|Milestones and Deliverables]]

A Milestones is that
- Points in the schedule which allow us to assess the progress; 时间表中允许我们评估进度的要点；
- An end-point of a process activity 过程活动的终点

A deliverable is Project results delivered to customers, e.g. a security report. 交付给客户的项目结果，例如 一份安全报告。

### Q4.3

> [[Project Management#Risk Management|Risk Management]]  
> [[Project Management#Risk management process|Risk Management Process]]

Risk Management is Identifying risks and drawing plans to minimize their negative effects 识别风险并制定计划以尽量减少其负面影响

- Risk identification of project/product/business risks 项目/产品/业务风险的风险识别
- Risk analysis assesses likelihood and consequences of risks 风险分析评估风险的可能性和后果
- Risk planning creates a plan to avoid the risk or minimise its effects 风险规划创建一个计划来避免风险或最小化其影响
- Risk monitoring checks risks regularly and plans for mitigation and revision (when e.g. more information is available) 风险监控定期检查风险并制定缓解和修订计划（例如，当有更多信息可用时）