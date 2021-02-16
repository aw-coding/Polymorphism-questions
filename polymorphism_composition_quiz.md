# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?

Many shapes, or many forms.


2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

It means one object can take the place of another. for instance, we could have a Cheese class which would inherit the properties and methods of its Food parent class, but still be treated as the Food class for other purposes. In creating the Cheese class it would be written:

public class Cheese extends Food{}



3. What can we use to implement polymorphism in Java?

Inheritance and Interfaces


4. How many 'forms' can an object take when using polymorphism?

There is no limit. A class can only have one parent class, but can have an unlimited amount of Interfaces.



5. Give an example of when you could use polymorphism.

You could be writing software for managing employees. There might be some features (methods and attributes) which would be common to all employees (such as hiring and firing), which would be in the abstract Employee class. 
However, you could add extra features to the child classes of that (such as a budgetControlled attribute to a SeniorManager class) which would be only in those respective child classes.



# Composition and Aggregation

6. What do we mean by 'composition' in reference to object-oriented programming?

It refers to an object which is composed of other objects.


7. When would you use composition? Provide a simple example in Java.

It is used when you want the existence of one object to be dependent on the other. For instance a Petal object might be dependent on a Flower object to which it is attached.
public Flower(){
    this.petal = new Petal()
}


8. Give a difference between composition and aggregation?

The difference is that although objects are tied together in both cases, they can only exist independently of each other in aggregation.


9. What is/are the advantage(s) of using composition/aggregation?

Using composition can be less error-prone than aggregation, since objects which are linked are destroyed and are not still existing (leaving unwanted functionality and scope for unforseen complications).
However, an advantage of aggregation is that in some cases we might want objects and their behaviours to remain, even after what they were linked to was destroyed. For example, a Team class might be made up of Employee objects, which would still remain even after a Team was disbanded (and deleted from the software).



10. When using composition, when an object is destroyed, what happens to all the objects it is composed of?

They are also destroyed.


11. When using aggregation, when an object is destroyed, what happens to all the objects it is composed of?

They are not destroyed.