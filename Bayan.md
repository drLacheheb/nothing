
Exam 1:

Section 1: Define Java Terms (10 marks)

1. Define the terms class and object in Java.

2. Explain the concept of inheritance in Java.

3. What is the purpose of the keyword "this" in Java?

Section 2: Code or Function Result Prediction (15 marks)

1. Given the following code snippet, what is the output?

   ```java

   int x = 5;

   System.out.println(x++);

   System.out.println(++x);

   ```

2. What will be the value of the variable "result" after executing the following code?

   ```java

   int result = 10;

   result += 5 * 3 % 2;

   ```

3. What will be the output of the following code?

   ```java

   String str1 = "Java";

   String str2 = new String("Java");

   System.out.println(str1 == str2);

   ```

Section 3: Code Completion or Debugging (25 marks)

1. Complete the following code snippet to calculate the sum of all elements in an array:

   ```java

   int[] numbers = {1, 2, 3, 4, 5};

   int sum = 0;

   for (int i = 0; i < numbers.length; i++) {

       // TODO: Complete the code here

   }

   System.out.println("Sum: " + sum);

   ```

2. Identify and fix the error in the following code that prevents it from compiling:

   ```java

   public class Person {

       private String name;

       public Person(String n) {

           name = n;

       }

       public void printName() {

           System.out.println(name);

       }

   }

   ```

Exam 2 (Building on Exam 1):

Section 1: Define Java Terms (15 marks)

1. Explain the concept of abstraction in Java.

2. Define the terms interface and abstract class in Java.

3. What is method overloading in Java?

Section 2: Code or Function Result Prediction (20 marks)

1. What will be the output of the following code?

   ```java

   public class A {

       public void print() {

           System.out.println("A");

       }

   }

   public class B extends A {

       public void print() {

           System.out.println("B");

       }

   }

   public class Main {

       public static void main(String[] args) {

           A obj = new B();

           obj.print();

       }

   }

   ```

2. Given the following code snippet, what is the value of "result"?

   ```java

   int result = 10;

   result = result++ + ++result - result--;

   ```

Section 3: Code Completion or Debugging (30 marks)

1. Complete the following code snippet to implement a basic calculator using OOP principles:

   ```java

   public class Calculator {

       // TODO: Add instance variables and constructor here

       public int add(int a, int b) {

           // TODO: Complete the method here

       }

       public int subtract(int a, int b) {

           // TODO: Complete the method here

       }

       // TODO: Add other arithmetic operations here

   }

   ```
