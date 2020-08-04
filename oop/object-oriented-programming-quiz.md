Object-Oriented Programming (OOP) Assessment
-----------------

#### Q1. What is an example of dynamic binding?
- any method 
- method overloading
- **method overriding** <<-- correct
- compiling

#### Q2. For which case would the use of a static attribute be appropriate?
- the number of people in each house in a small neighborhood
- the lot size for each house in a small neighborhood
- the color of each house in a small neighborhood
- **the weather conditions for each house in a small neighborhood** <<-- correct

#### Q3. Why would you create an abstract class, if it can have no real instances?
- **to avoid redundant coding in children** << -- correct
- to explore a hypothetical class
- to prevent unwanted method implementation
- to reserve memory for an unspecified class type

#### Q4. When does static binding happen?
- only when you export
- both at compile time and runtime
- **at compile time** <<-- correct
- at runtime

#### Q5. What is the best reason to use a design pattern?
- **It will result in code that is more extensible and maintainable.** <<-- correct
- It will result in a more compact product.
- It will speed initial development.
- It will allow you to add that design pattern to your resume.

#### Q6. What is encapsulation?
- defining classes by focusing on what is important for a purpose 
- **hiding the data and implementation details within a class** <<-- correct
- making all methods private
- using words to define classes

#### Q7. What is an IS-A relationship?
- It implies encapsulation.
- A superclass object has an IS-A relationship with its subclass.
- It implies a virtual method.
- **A subclass object has an IS-A relationship with its superclass or interface** <<-- correct

#### Q8. You want a method with behavior similar to a virtual method--it is meant to be overridden --expect that it does not have a mthod body. It just has a method signature. What kind of method should you use?
- an abstract method
- **a public internal method** <<-- correct
- an internal method 
- a protected internal method

#### Q9. Which code creates a new object from the Employee class?
- Employee current Employee = Employee.Create();
- **Employee current Employee = new Employee();** <<-- correct
- Employee currentEmployee;
- Employee currentEmployee = Employee.New();

#### Q10. Which type of constructor cannot have a return type?
- default
- copy
- parameterized
- **Constructors do not have a return type** <<-- correct

#### Q11. When is a constructor executed?
- **when an object is created from a class using the new keyword** <<-- correct
- when an class is defined using the class keyword
- every time an object is referenced
- when an object is created from a class using the create keyword

#### Q12. If a local class is defined in a function, what is true for an object of that class?
- **The object can be accessed, declared, and used locally in that function.** <<-- correct
- The object must be declared inside any other function.
- The object is temporarily accessible outside the function.
- The object can call all the other class members anywhere in the program.

#### Q13. Which two blocks are used to handle and check errors?
- do and check
- catching and trying 
- **try and catch** <<-- correct
- do and while

#### Q14. Why would you implement composition using an id instead of a reference?
- It makes it easier to save the entity.
- **all of these answers** <<-- correct
- It can make the entity retrieval more efficient
- It minimizes coupling.

#### Q15. Which statement best describes the method of inheritance in OOP?
- **Inheritance describes the ability to create new classes based on an existing class.** <<-- correct
- Inheritance means that a group of related properties, methods, and other members are treated as a single unit or object.
- Inheritance forces a class to have a single repsonsibilitly from only one parent.
- Inheritance means that you will never have multiple classes that can be used interchangeably, even though each class implements the same properties or methods in different ways.

#### Q16 Which type of inheritance ,when done continuously, is similar to a tree structure?
- multilevel
- hierarchical and multiple
- hierarchical **<<--correct 
- multiple

#### Q17. Which statement is true?
- A default parameter's constructor is not equivalent to the default constructor
- A default constructor is inherited from a parent class
- A default constructor can be called explicitly
- **A default constructor cannot be defined by the coder** <<-- correct

#### Q18. Which of the following is NOT an advantage of using getters and setters?
- Getters and setters can speed up compilation.
- Getters and setters provide encapsulation of behavior.
- Getters and setters provide a debugging point for when a property changes at runtime. <<--- picked this one not sure if its correct!
- Getters and setters permit different access levels.

#### Q19. In context of OOP, what is association?
- Association is a relationship where all objects have their own life cycle and there is no owner. <<-- correct
- Association is the procecss where model elements cooperate to proide higher-level behavior.
Association is whole/part relationship where one object is composed of one or more other objects, each of which is considered a part of the whole. 
- Association is where all objects have their own life cycle, but there is ownerhip, and child objects can not belong to another parent object.

#### Q20. How are user stories different from use cases?
- **User Stories are shorter and less detailed.** <<-- correct
- User stories are more accurate.
- User stories are more detailed and structured.
- User storised are more anecdotal and personal.

#### Q21. Which type of inheritance must be used so that the resultant is hybrid?
- multiple
- any type of inheritance
- **multilevel**  <<--- picked this one, 
- hierarchical

#### Q22. A language that does not support polymorphism but supports classes is considered what?
- **an object-based language** <<--- picked this one
- a class-based language
- a procedure-oriented language
- if classes are supported, polymorphism will be supported

#### Q23. If two classes combine some private data members and provides public member functions to access and manipulate those data members. Where is abstraction used?
- Abstraction is using a private access specifier for data members
- **Abstraction is using public member functions to access and manipulate the data members** <<-- correct
- Abstraction is using the class concept with both data members and member functions
- There is insufficient information to decide where abstraction is being used.

#### Q24. What are the five Creational Design patterns by the Gang of Four ?
- Observer, State, Strategy, Template Method, and Visitor.
- Composite, Visitor, State, Prototype, and Singleton.
- Composite, Builder, Factory Method, Prototype, and Singleton.
- **Abstract Factory, Builder, Factory Method, Prototype, and Singleton.** <<-- correct

#### Q25. In multilevel inheritence, one class inherits how many classes?
- one class only <<-- correct
- two classes
- as many classes as required
- at least two classes 

#### Q26. if an object is passed by reference, the changes made in the function are reflected _______.
- to the main object of the caller function, too <<-- correct
- on the caller function object and also the called function object
- on the copy of the object that is made during the pass
- only in the local scope of the called function

#### Q27. What is a method? 
- a set of instructions designed to perform a frequently used operation within a program and return no values
- the exact same thing as a function and subroutine <<-- correct
- a set of variables that can change over time
- a procedure associated with data and behaviour 

### Q28. A mobile phone is made up of components such as a motherboard, camera, and sensors. The motherboard represents all the functions of a phone, the display shows the display only, and the phone is represented as a whole. Which of the following has the highest level of abstraction?
- camera
- display
- motherboard
- mobile phone <<-- correct
