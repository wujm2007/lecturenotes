## What Is Software Design?

- Find solution to a problem
- Map problem domain cencepts to programming concepts
  - Date structures
  - Interface
  - Program logic
- Dealing with complexity: abstraction/modularization
- Dealing with changes



- This is not an algorithm class
- This is not a programing language class



## Prerequisites

- Solid programming skill
  - We do not teach inheritance, encapsulation and polymorphism
  - We will teach how and when to use them
- Java programming
  - We are not supposed to debug your program
- Datebase, file processing
- UML modeling
  - We will review it in class, but not teach it in detail
- Eclipse



## Topics: Software Design Fundamentals

- Design principles
- Experiences (Patterns)
- Communications (representations, UML)
- Object-oriented programing



## Reference Books

- Design patterns: elements of reusable object-oriented software


- Design patterns explained


- Head first design pattern



## Grades

- Main content
  - 4 labs (40%)
  - homework (2 parts) (40%)
  - final (20%)


- Participation (-10%)
  - arrive on time
  - no cell phone
  - no chatting
  - participate in activities.



## Software Design - Find a Solution

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

### The Essence of OO Design

1. Shift in Responsibility
2. Abstraction
   1. abstract class/concrete class
   2. inheritance/realization
3. Modularization/Information Hiding
   1. date encapsulation
   2. polymorphism
   3. coupling/cohesion

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



## The UML Diagrams

### Class Diagram

