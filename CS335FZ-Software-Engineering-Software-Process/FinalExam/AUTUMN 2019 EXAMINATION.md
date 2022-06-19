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