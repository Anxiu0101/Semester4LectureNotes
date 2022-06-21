## Q1

Consider the following specification text: “A client company that sells oil burners needs a specific editorial content management system to manage product manuals that are written for customers. Engineers write and submit drafts of product manuals. Reviewers check these manuals for their technical accuracy and the quality of writing (so that customers can understand them). There is a list of reviewers (an audit committee) who can review and evaluate the submitted manuals. The chief editor will distribute the manuals to relevant reviewers (those that have the necessary technical knowledge). The reviewers then submit their reviews/comments and a score to the system. The chief editor will make the decision about accepting the manual to be published online or to reject the manual and return it to the engineer. The chief editor then notifies the engineers about the status of their submission.”
1. Given the above specification text, draw two data flow diagrams (DFD): First a high-level (Level 0) DFD followed by a more detailed level (Level 1) DFD. [20 marks]
2. Represent the following text as an entity relationship (ER) diagram: ‘Staff registers a client at a branch’. [5 marks]


## Q2

Consider the following text that describes Dublin airport: For this example, we only consider Passengers, Tour guides, Minor Passengers (children), Passengers with Special Needs (e.g. with disabilities). Furthermore, consider Dublin airport as a business, similar to a system. Some of the essential things passengers typically do at Dublin airport are individual check-in, group check-in (for groups of tourists) and security screening – all of these represent important business functions or processes that take place at Dublin airport and serve the needs of passengers. Check-in can be performed at the counter or at the kiosk. Because passengers might have no luggage, luggage check-in is optional.
Draw the use-case diagram for this description.

> [[Use Case]]

```puml
skinparam actorStyle awesome
left to right direction
package DublinAirportSystem {
	usecase "check in" as uc1
	usecase "group check in" as uc2
	usecase "security screening" as uc3
}

:User: --> uc1
:User: --> uc2
:User: --> uc3
```


## Q3

You are being asked to design a software system for DriveWell Ltd., a school of motoring. The owner of the driving school has previously been interviewed by a colleague and you get the following description of their business activities:
“Our school has many highly-qualified instructors that we keep on record with their instructor number, their name, address, mobile phone, and driving qualification. A new client must first attend an interview with an instructor to discuss an appropriate plan of learning. Such interviews are booked with a specific date and time and, as a result, determine a learning plan. During this interview the client provides some personal information (his/her provisional driving license number, mobile phone number and address). Each client is uniquely identified with a client number. A client may request individual lessons or book a block of five, however all lessons cost the same. A lesson takes an hour and is with a particular instructor in a particular car at a given date and time. After each lesson, the instructor records the progress made by the client and notes the mileage used during the lesson. The school has a pool of cars which are adapted for the purpose of teaching. Each instructor has a sole use of a particular car. We record the registration plate, the make and the model of each car in our records.”
Draw the UML class diagram for this description and explain its specifics in
detail, if needed.


## Q4

1. What is the observer design pattern? Describe a scenario, based on a concrete example, where the observer design pattern is needed.[8 marks]
2. Using a washing machine as an example, describe three functional requirements and two non-functional requirements. [5 marks]
3. Describe the different types of relationship between classes in an UML Class Diagram and create an example for each in UML (association, aggregation, composition, unary). [12 marks]

### Q4.1

> [[Design Patterns#Observer Pattern|Observer Pattern]]

### Q4.2

> [[Functional Requirements and Non-functional Requirements]]

### Q4.3

> [[UML Class Diagram#Association Aggregation and Composition]]  
> Unary 课件上好像·没有