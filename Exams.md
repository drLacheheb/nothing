## Exam 1

### Section 1: Define Java Terms

1. What is inheritance in Java? 

2. What is polymorphism in Java? 

3. What is an abstract class in Java? 

4. What is an interface in Java? 

### Section 2: Code or Function Result Prediction

1. What will be the output of the following code snippet? 

```java

public class Animal {

    public void makeSound() {

        System.out.println("The animal makes a sound");

    }

}

public class Cat extends Animal {

    public void makeSound() {

        System.out.println("The cat meows");

    }

}

public class Main {

    public static void main(String[] args) {

        Animal animal1 = new Animal();

        Animal animal2 = new Cat();

        animal1.makeSound();

        animal2.makeSound();

    }

}

```

2. What will be the output of the following code snippet? 

```java

public abstract class Shape {

    int x, y;

    public void moveTo(int newX, int newY) {

        x = newX;

        y = newY;

    }

    public abstract void draw();

}

public class Circle extends Shape {

    int radius;

    public void draw() {

        System.out.println("Drawing Circle");

    }

}

public class Main {

    public static void main(String[] args) {

        Circle circle = new Circle();

        circle.moveTo(3, 4);

        circle.draw();

    }

}

```

3. What will be the output of the following code snippet? 

```java

interface Animal {

    public void makeSound();

}

class Dog implements Animal {

    public void makeSound() {

        System.out.println("The dog barks");

    }

}

class Cat implements Animal {

    public void makeSound() {

        System.out.println("The cat meows");

    }

}

class Main {

    public static void main(String[] args) {

        Animal animal1 = new Dog();

        Animal animal2 = new Cat();

        animal1.makeSound();

        animal2.makeSound();

    }

}

```

### Section 3: Code Completion or Debugging

1. Complete the following code to create a subclass of `Shape` called `Rectangle` with a `width` and `height` attribute. The `draw()` method should print "Drawing Rectangle". 

```java

public class Shape {

    int x, y;

    public void moveTo(int newX, int newY) {

        x = newX;

        y = newY;

    }

    public void draw() {

        System.out.println("Drawing Shape");

    }

}

public class Rectangle extends Shape {

    int width, height;

    public void draw() {

        // TODO: add code to draw the rectangle

    }

}

```

2. Identify and fix the error in the following code snippet: 

```java

public abstract class Animal {

    public void makeSound() {

        System.out.println("The animal makes a sound");

    }

}

public class Cat extends Animal {

    public void makeSound() {

        System.out.println("The cat meows");

    }

}

public class Main {

    public static void main(String[] args) {

        Animal animal1 = new Animal();

        Animal animal2 = new Cat();

        animal1.makeSound();

        animal2.makeSound();

    }

}

```

3. Complete the following code to implement the `Drawable` interface and print "Drawing Triangle". 

```java

interface Drawable {

    public void draw();

}

class Triangle implements Drawable {

    // TODO: add code to draw the triangle

}

class Main {

    public static void main(String[] args) {

        Drawable triangle = new Triangle();

        triangle.draw();

    }

}

```

    
    
   





