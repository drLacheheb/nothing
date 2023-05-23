Here are three more exams, each increasing in difficulty, focusing on Object-Oriented Programming (OOP) concepts in Java:

Exam 3:

Section 1: Define Java Terms (15 marks)

1. What is the purpose of the "super" keyword in Java? Give an example.

2. Explain the concept of method overriding in Java.

3. Define the terms "static" and "final" in Java.

Section 2: Code or Function Result Prediction (20 marks)

1. What will be the output of the following code?

   ```java

   public class A {

       public void method() {

           System.out.println("A");

       }

   }

   public class B extends A {

       public void method() {

           super.method();

           System.out.println("B");

       }

   }

   public class Main {

       public static void main(String[] args) {

           A obj = new B();

           obj.method();

       }

   }

   ```

2. Given the following code snippet, what will be the value of "result"?

   ```java

   int result = 10;

   result = result++ * ++result - result--;

   ```

Section 3: Code Completion or Debugging (30 marks)

1. Complete the following code snippet to implement a class hierarchy representing different shapes:

   ```java

   public abstract class Shape {

       // TODO: Define necessary instance variables and methods here

   }

   

   public class Circle extends Shape {

       // TODO: Implement necessary methods and constructors here

   }

   

   public class Rectangle extends Shape {

       // TODO: Implement necessary methods and constructors here

   }

   ```

Exam 4 (Building on Exam 3):

Section 1: Define Java Terms (20 marks)

1. Explain the concept of interface inheritance in Java.

2. Define the terms "polymorphism" and "dynamic binding" in Java.

3. What is the purpose of the "final" keyword when applied to a class in Java?

Section 2: Code or Function Result Prediction (25 marks)

1. What will be the output of the following code?

   ```java

   public interface Printable {

       void print();

   }

   

   public class A implements Printable {

       public void print() {

           System.out.println("A");

       }

   }

   

   public class B implements Printable {

       public void print() {

           System.out.println("B");

       }

   }

   

   public class Main {

       public static void main(String[] args) {

           Printable obj = new B();

           obj.print();

       }

   }

   ```

2. Given the following code snippet, what will be the value of "result"?

   ```java

   int result = 10;

   result = ++result * (result-- + result++);

   ```

Section 3: Code Completion or Debugging (35 marks)

1. Complete the following code snippet to implement a simple banking system using OOP principles:

   ```java

   public abstract class Account {

       // TODO: Define necessary instance variables and methods here

   }

   

   public class SavingsAccount extends Account {

       // TODO: Implement necessary methods and constructors here

   }

   

   public class CheckingAccount extends Account {

       // TODO: Implement necessary methods and constructors here

   }

   

   public class Bank {

       private List<Account> accounts;

   

       // TODO: Implement necessary methods to manage accounts here

   }

   ```

Exam 5 (Building on Exam 4):

Section 1: Define Java Terms (25 marks)

1. Explain the concept of an abstract class in Java. Provide an example.

2. Define the terms "constructor" and "method overloading" in Java.

3. What is the purpose

 of the "protected" access modifier in Java?

Section 2: Code or Function Result Prediction (30 marks)

1. What will be the output of the following code?

   ```java

   public abstract class A {

       public abstract void methodA();

       public void methodB() {

           System.out.println("B");

       }

   }

   

   public class B extends A {

       public void methodA() {

           System.out.println("A");

       }

   }

   

   public class Main {

       public static void main(String[] args) {

           A obj = new B();

           obj.methodA();

           obj.methodB();

       }

   }

   ```

2. Given the following code snippet, what will be the value of "result"?

   ```java

   int result = 10;

   result = (result++ + result--) * ++result;

   ```

Section 3: Code Completion or Debugging (40 marks)

1. Complete the following code snippet to implement a basic game using inheritance and polymorphism:

   ```java

   public abstract class Game {

       // TODO: Define necessary instance variables and methods here

   }

   

   public class TicTacToe extends Game {

       // TODO: Implement necessary methods and constructors here

   }

   

   public class Chess extends Game {

       // TODO: Implement necessary methods and constructors here

   }

   

   public class Main {

       public static void main(String[] args) {

           Game game1 = new TicTacToe();

           Game game2 = new Chess();

           // TODO: Simulate the game and print the winner

       }

   }

   ```
