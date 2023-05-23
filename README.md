## Object-Oriented Programming (OOP) in Java 

Object-Oriented Programming (OOP) is a programming paradigm that revolves around the concept of objects, which are instances of classes. Java is a popular programming language that fully supports OOP principles. In this summary, we'll explore the core concepts of OOP in Java and provide examples to illustrate each concept.  ### Classes and Objects  In Java, a class is a blueprint or template that defines the structure and behavior of objects. An object is an instance of a class, representing a specific entity. For example, we can define a class called "Car" with attributes like color, model, and speed. We can then create multiple car objects based on this class.  

```java

class Car {

    String color;

    String model;

    int speed;

    void accelerate() {

        // Code to increase the car's speed

    }

}

// Creating objects of the Car class

Car car1 = new Car();

Car car2 = new Car();`

```

### Encapsulation

Encapsulation ensures that data (variables) and methods (functions) that operate on the data are bundled together within a class, and access to them is controlled through methods. This provides data hiding and protects the integrity of the data.

```java

class BankAccount {

    private double balance;

    public void deposit(double amount) {

        // Code to deposit the given amount into the account

    }

    public double getBalance() {

        // Code to retrieve the account balance 

    }

}

BankAccount account = new BankAccount();

account.deposit(100.0);

double balance = account.getBalance();

```

### Inheritance

Inheritance allows classes to inherit properties and methods from other classes, creating a hierarchical relationship between classes. The class that is inherited from is called the superclass (or parent class), and the class that inherits is called the subclass (or child class).

```java

class Animal {

    void eat() {

        // Code for eating

    }

}  

class Cat extends Animal {

    void meow() {

        // Code for meowing

    }

}

Cat cat = new Cat(); cat.eat();

// Inherited method

cat.meow(); // Method specific to the Cat class

```

### Polymorphism

Polymorphism allows objects of different classes to be treated as objects of a common superclass, enabling methods to be invoked dynamically at runtime. Polymorphism is achieved through method overriding and method overloading.

```java

class Animal {

    void makeSound() {

        // Code to make a generic animal sound

    }

}

class Dog extends Animal {

    void makeSound() {

        // Code to make a dog-specific sound

    }

}

class Cat extends Animal {

    void makeSound() {

        // Code to make a cat-specific sound

    }

}

Animal animal1 = new Dog(); Animal animal2 = new Cat(); animal1.makeSound();  // Executes the Dog class's makeSound() method

animal2.makeSound();  // Executes the Cat class's makeSound() method`

```

### Abstraction

Abstraction focuses on providing simplified interfaces for complex systems by hiding unnecessary implementation details. Abstract classes and interfaces are used to define abstract types, which cannot be instantiated but can be extended or implemented by other classes.

```java

abstract class Shape {

    abstract void draw();

}

class Circle extends Shape {

    void draw() {

        // Code to draw a circle

    }

}

class Rectangle extends Shape {

    void draw() {

        // Code to draw a rectangle

    }

}

Shape shape1 = new Circle(); 

Shape shape2 = new Rectangle();

shape1.draw();  // Draws a circle shape2.draw();  // Draws a rectangle`

```

These are the fundamental concepts of OOP in Java.

## Abstract Classes and Interfaces

Abstract classes and interfaces are key components of object-oriented programming in Java that facilitate abstraction and provide a way to define common behaviors and contracts for classes.

### Abstract Classes

An abstract class in Java is a class that cannot be instantiated directly and is typically used as a base class for other classes. It serves as a blueprint for its subclasses by defining common attributes and methods. An abstract class can have both abstract and non-abstract methods.

```java

abstract class Animal {

    String name;

    public Animal(String name) {

        this.name = name;

    }

    abstract void sound(); // Abstract method

    void sleep() {

        System.out.println("The animal is sleeping.");

    }

}

class Dog extends Animal {

    public Dog(String name) {

        super(name);

    }

    void sound() {

        System.out.println("The dog barks.");

    }

}

Animal dog = new Dog("Buddy"); dog.sound(); // Output: "The dog barks." 

dog.sleep(); // Output: "The animal is sleeping."`

```

### Interfaces

An interface in Java defines a contract that specifies a set of methods that implementing classes must adhere to. It represents a collection of abstract methods and constant (static final) variables. In essence, an interface defines what a class should do, without specifying how it should be done.

```java

interface Shape {

    double getArea(); // Abstract method

    double getPerimeter(); // Abstract method

}

class Circle implements Shape {

    double radius;

    public Circle(double radius) {

        this.radius = radius;

    }

    public double getArea() {

        return Math.PI * radius * radius;

    }

    public double getPerimeter() {

        return 2 * Math.PI * radius;

    }

}

Shape circle = new Circle(5.0);

System.out.println("Area: " + circle.getArea()); // Output: "Area: 78.53981633974483" 

System.out.println("Perimeter: " + circle.getPerimeter()); // Output: "Perimeter: 31.41592653589793"

```

Interfaces provide a way to achieve abstraction, promote code reusability, and allow classes to be loosely coupled by programming to interfaces rather than concrete implementations.

### Inheritance and Overrides

Inheritance allows a class to inherit properties and behaviors from its superclass. The `super()` keyword is used to call the constructor of the superclass. Method overriding allows a subclass to provide its own implementation of a method that is already defined in its superclass.

```java

class Vehicle {

    protected String brand;

    public Vehicle(String brand) {

        this.brand = brand;

    }

    public void start() {

        System.out.println("Starting the vehicle.");

    }

}  

class Car extends Vehicle {

    private int numberOfDoors;

    public Car(String brand, int numberOfDoors) {

        super(brand); // Calling the superclass constructor

        this.numberOfDoors = numberOfDoors;

    }

    public void drive() {

        System.out.println("Driving the car.");

    }

}

Car myCar = new Car("Toyota", 4); myCar.start(); // Output: "Starting the vehicle." 

myCar.drive(); // Output: "Driving the car."  

class Animal {

    public void makeSound() {

        System.out.println("The animal makes a sound.");

    }

}

class Cat extends Animal {

    @Override

    public void makeSound() {

        System.out.println("The cat meows.");

    }

}

Cat myCat = new Cat(); myCat.makeSound(); // Output: "The cat meows."

```

Inheritance and method overriding allow subclasses to extend or modify the behavior inherited from the superclass, providing flexibility and customization in the code.

This covers the summary of inheritance, abstract classes, interfaces, and related concepts in Java.
