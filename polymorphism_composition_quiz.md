# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?
    many forms

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.
    Polymorphism happens when methods are inherited from the parent class but changed to perform a different task.

    An Animal is a Parent class and has a talk method which returns a String - "I can talk". Horse is a child class of Animal and has a talk method but instead of "I can talk it" returns "Neigh". This is polymorphism as the same method is returning different strings.(method overriding)

3. What can we use to implement polymorphism in Java?
    method overriding or overloading

4. How many 'forms' can an object take when using polymorphism?
    many

5. Give an example of when you could use polymorphism.
    An Animal is a Parent class and has a talk method which returns a String - "I can talk". Horse is a child class of Animal and has a talk method but instead of "I can talk it" returns "Neigh". This is polymorphism as the same method is returning different strings.(method overriding)


# Composition and Aggregation

6. What do we mean by 'composition' in reference to object-oriented programming?
    composition is a class relationship where one class depends on another. Has-a relationship
7. When would you use composition? Provide a simple example in Java.
    You would use comosition if the relationship is a Has-a and not an is-a.
    if you have a Student class and an address class the Student HAS-a Address. Instead of using inheritance you can use composition by using instance variables that refer to other objects.

    public class Student {

    String name;
    int studentNumber;
    //composition has-a relationship
    Address address;
   
    public Student(String name, int studentNumber, Address address){
        this.name=name;
        this.studentName = studentName;
        this.address = address
    }

8. Give a difference between composition and aggregation?
    Aggregation and composition are both Has-a relationships but with composition the class belongs to the other class(house has a roof) where with aggregation the object can exist without the other class. e.g Car has a wheel. 
9. What is/are the advantage(s) of using composition/aggregation?
    classes achieve polymorphism and code resuse by composition
    can change class implementation at run-time by changing the object
    Can achieve multiple inheritance via composition

10. When using composition, when an object is destroyed, what happens to all the objects it is composed of?
    also destroyed

11. When using aggregation, when an object is destroyed, what happens to all the objects it is composed of?
    still exists