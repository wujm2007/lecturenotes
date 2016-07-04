## Class Information

### What Is Software Design?

- Find solution to a problem
- Map problem domain cencepts to programming concepts
  - Date structures
  - Interface
  - Program logic
- Dealing with complexity: abstraction/modularization
- Dealing with changes



- This is not an algorithm class
- This is not a programing language class


### Prerequisites

- Solid programming skill
  - We do not teach inheritance, encapsulation and polymorphism
  - We will teach how and when to use them
- Java programming
  - We are not supposed to debug your program
- Datebase, file processing
- UML modeling
  - We will review it in class, but not teach it in detail
- Eclipse


### Topics: Software Design Fundamentals

- Design principles
- Experiences (Patterns)
- Communications (representations, UML)
- Object-oriented programing





## OO Paradigm

### Software Design - Find a Solution

Consider the example of an instructor at a conference. Student in your class have another class to attend following yours, but don't know where it is located. You are responsible to make sure everyone knows how to get to the next class.

### A Nature Solution

Get a list of student in the class

For each student

1. Find the next class she or he is taking
2. Find the location of that class
3. Find the way to get from your classsroom to  the student's next class
4. Tell the student how to get to his or her next class

### A Procedrual Solution

To do this work require the following procedures:

1. A way of getting the list of people in the class.
2. A way of getting the schedule for each person in the class.
3. A program that gives someone directions from your calssroom to any other classroom.
4. A control program that works for each person in the class and does the required steps for each person.

#### Is that reality?

- Probably not.
- Second method:
  - You would post directions to go from this classroom to all other classrooms.
  - Tell everyone in the class what you did.
  - People use the directions to go to their next class.


- This is a philosophical difference. It's a shift in responsibility.

### The OO Approach to the Classroom problem

1. Start the control program
2. Instantiate the collection of sudents in the classroom
3. Tell the collection to have the students go to their next class.
4. The collection tells each student to go to his or her class.
5. Each student:
   - Finds where his next class is.
   - Determines how to get there.
   - Goes there.
6. Done.

### The Object-Oriented Paradigm

1. Shift in Responsibility

   - Centered on the concept of the object. 

   - What is an object?

     - Traditionally: data with method.
     - Better Definition: Things responsible for themselves.

   - Conceptual View of an Object:

     An object is a set of responsibilities.

   - Specification View of an Object:

     An object is a set of methods (behaviors) that can be invoked by other objects or itself.

   - Implementation View of an Object:

     An object is code and data and the computational interactions between them.

   - An object’s **interface** is it’s collection of methods.

   - A class has the following:

     - The data elements the object contains
     - The methods the object can do
     - The way these data elements and methods can be accessed

2. Abstraction

   - Three levels of accessibility:
     - Public – Anything can see it
     - Protected – Only objects of this class and derived classes can see it
     - Private – Only objects from this class can see it
   - Encapsulation is not just about data, it’s about any kind of hiding!
   - In our previous examples, the type of student is in essence hidden from the control program (in essence, because it has to instantiate it and thus know what type of object it is).
   - This encapsulation is known as **polymorphism**.
   - Polymorphism can be defined as the ability to refer to different derivation of a class in the same way, but getting the behavior appropriate to a subclass

### Why do programs fail in the “real world”? 

- Most of you should have had some co op experience and therefore a taste of the real world. 
- In academics the problem
  - you are solving is usually clearly laid out. 
  - Expectations are well defined. 
- This is not the case in the real world. 
- While a program can fail because:
  - Technological problems
  - Incompetent Programmers
  - Poor Management
  - Poor Development Tools
- **The #1 reason projects fail is poor requirements gathering.**

### The Reality

- Why are requirements poor?
  - Requirements are incomplete
  - Requirements are often wrong
  - Requirements (and users) are misleading
  - Requirements do not tell the whole story
- While one tries to document requirements completely and properly, the reality is, for many reasons you will not achieve a perfect set of requirements. 
- If you do not have good requirements, how can programmers possibly be expected to develop an application that meets the needs of the end user.
- The reality is, **requirements always change**.

### OO Elements - Classes/Objects

- Abstract classes define what other, related classes can do.
- These "other" classes are classes that represent a particular type of related behavior. Such a class is called a **concrete class**.
- Therefore, *UndergradSudent* and *GraduateStudent* would be concrete classes.

### OO Elements - Relations

- The realationship between an  *UndergradSudent* and a *Student* class is called **is-a relationship**.
- An is-a relationship is a form of **inheritance**.


- Abstract classes act as placeholders for other concrete classes.
- Abstract classes define the methods their derived classes **must** implement.

### Good OO design

- The most important promise of OO is improve modularization
  - that is, enhance mantainability
  - while still supporting functional decomposition (which is good for cohesion)
  - while also promoting re-use
- Good OO = high cohesion + low coupling
  - Cohesion refers to how “closely the operations in a routine are related.”
  - Coupling refers to “the strength of a connection between two routines.”




### The Essence of OO Design

1. Shift in Responsibility
2. Abstraction
   1. Abstract Class vs. Concrete Class
   2. Inheritance/Realization
3. Modularization/Information Hiding
   1. Data Encapsulation
   2. Polymorphism
   3. Coupling/Cohesion



