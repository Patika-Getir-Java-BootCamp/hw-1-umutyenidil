1. As humans, we tend to solve problems by making them more concrete, because dealing with something tangible 
is easier than dealing with something abstract. Programming, which is inherently based on abstract concepts, 
becomes more memorable and easier to understand when we reinforce it with real-life examples. 
For instance, when we talking about OOP concepts, we often refer to entities like cars or animals, focusing on their properties and behaviors.
From a technical perspective, OOP provides benefits such as modularity, improved code readability, data encapsulation, easier maintenance, and flexibility.
Some of the major OOP programming languages include: Java, Python, Dart, and Swift.

2. These two approaches make inheritance easier in OOP. An interface defines what an object should do, but not how it should do it. 
On the other hand, an abstract class can define both what should be done and how it can be done.
In essence, interfaces can be seen as protocols, while abstract classes serve as templates that contain shared properties or behaviors.

3. These two methods are overridden and used to check whether created objects are equal or not. 
Reference types cannot be compared using simple equality operators like primitive types can, 
because while primitive types like int, boolean hold actual values but reference types hold references to objects created from classes.
For example, two Insan class instances with the name property as "Umut" are not considered equal by default, 
because they are stored at different memory locations.
By overriding hashCode(), a numeric value is generated based on specific properties of the instance. 
Then, by overriding equals(), we compare whether the properties used in hashCode() are the same in both instances, 
allowing us to define meaningful equality between objects.

4. The diamond problem is an inheritance conflict that occurs in languages that support multiple inheritance. 
If a class has two superclasses that both define the same method, the compiler cannot determine which method of the superclasses to use. 
This creates confusion and can prevent the program from running properly.
To avoid this issue, Java does not allow multiple inheritance with classes. 
Instead, it allows multiple interfaces to be implemented. Even if those interfaces contain methods with the same signature, 
Java requires the subclass to explicitly define which version of the method should be used, thus resolving the conflict.

5. The Garbage Collector is a built-in feature necessary for programs to run efficiently and to prevent memory leaks. 
It cleans up memory areas that were allocated during the lifecycle of the program but are no longer in use.
For example, suppose we create an object and hold it with a reference. 
Later, we create a new object and assign it to the same reference. 
As a result, the previous object is no longer accessible but still occupies space in memory. 
In such cases, the JVM periodically checks for these unreachable objects, triggers the garbage collection process, and removes them from memory.
Although the Garbage Collector runs automatically under the JVM, we can also request it manually using the System.gc().

6. The static keyword is used to define class-level properties. Static methods and properties are shared and can be accessed 
by all instances created from the same class. In addition to being used for defining methods and properties, static can also be used
to create static code blocks that execute as soon as the class is loaded. 
These blocks are useful for initializing or configuring static methods and variables when the class is first used.

7. Immutability is used to define instances that cannot be changed after they are created. 
In instances with this characteristic, you cannot modify the object directly.
Instead, you can make changes by creating a new instance based on the existing one and assigning it to a different reference.
This approach is especially useful for preventing issues like deadlocks in asynchronous operations.
Classes like String, LocalDate are examples of immutable classes in Java.

8. Composition and Aggregation are two concepts in OOP that describe relationships between objects.
In Composition, the relationship represents a whole-part structure. For example, a House class and a Room class have a composition relationship. Rooms can't exist without a house, and a house can't exist without rooms.
On the other hand, Aggregation represents more of a group or collection type of relationship. For instance, a Class and Student classes have an aggregation relationship. A Class can exist without Students, and a Student doesn’t necessarily have to belong to a Class.

9. Cohesion and coupling are two concepts essential for writing good code. 
Cohesion refers to how closely related the methods in a class or module are in terms of what they do. 
High cohesion means that the class or module is focused on a single purpose. 
Coupling indicates the level of dependency between different classes or modules. 
Low coupling means that classes or modules function independently, while high coupling means they are dependent on each other. 
Good code should be defined by high cohesion and low coupling.

10. Heap and Stack are two different areas of RAM with distinct characteristics. The Stack stores method calls, local variables, 
primitive values, and references. It is faster compared to the heap and operates based on the Last in firs tout principle.
The Heap, on the other hand, holds objects until they are cleared by the garbage collector. It has a larger capacity than the Stack but is generally slower in terms of access speed.

11. Exceptions are unexpected errors that occur during the flow of a program. 
These errors can disrupt the normal execution, so it is important to handle them properly.
There are errors that occur at compile time and runtime. Compile time errors are easier to detect and handle since they are caught by the compiler before the program runs. 
However, runtime errors are harder to identify, as they only occur during the actual execution of the program.

12. In my opinion, clean code is a standard. This standard, established by one or more developers during the construction of a program, makes the code easier to read and maintain.

13. Method hiding is an unusual case that occurs when static methods are seemingly overridden. 
It refers to the situation where a subclass defines a static method with the same signature as one in its superclass.
In such cases, the static method that gets called is determined by the reference type, not the object type.

14. Abstraction and polymorphism are two concepts in OOP that serve different purposes.
In abstraction, the goal is to show what an object does while hiding how it does it, providing a simplified interface.
Polymorphism, on the other hand, aims to allow objects to exhibit different behaviors in different forms, enabling flexibility in how actions are performed.
