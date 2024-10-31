# Polymorphism 

 Polymorphisms refer to the occurrence of something in multiple forms. As part of polymorphism, a Python child class has methods with the same name as a parent class method.A single type of entity is used to represent a variety of types in different contexts (methods, operators, objects, etc.)

# Method Overriding:

Method overriding is an object-oriented programming technique that lets us change the function implementation of a parent class in the child class. Method overriding is basically a child class's ability to implement change in any method given by one of its parent classes.

# Condition of method Overriding:

* Inheritance: There should be inheritance. Within a class, function overriding is not possible, therefore a child class is derived from a parent class.

* Same Method Name: The method in the subclass must have the same name as the method in the superclass that it intends to override.

* Same Parameters:The method in the subclass must have the same signature (i.e., the same number and type of     parameters) as the method in the superclass.

# Comparision :

## Polymorphism:  A function that calls the fly() method on different objects (like Bird and Airplane).

        class Bird:
            def fly(self):
                return "Flies"
        class Airplane:
            def fly(self):
                return "Flies with engines"
            def let_it_fly(flyable):
                print(flyable.fly())
            let_it_fly(Bird())       # Output: Flies
            let_it_fly(Airplane())   # Output: Flies with engines


## Method Overriding:  A Dog class that overrides the speak() method from its Animal superclass to return "Bark".

        class Animal:
            def speak(self):
                return "Animal speaks"
        class Dog(Animal):
                def speak(self):
                return "Bark"
        class Cat(Animal):
            def speak(self):
                return "Meow"
            def animal_sound(animal):
            print(animal.speak())
            animal_sound(Dog())  # Output: Bark
            animal_sound(Cat())  # Output: Meow

# Comparison using table :

![alt text](/images/table.png)



