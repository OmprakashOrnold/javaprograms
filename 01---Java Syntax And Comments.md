## Java Syntax And Comments Examples

### Example 1 - Print a variable

```java
class A{
    public static void main(String[] args) {
        int A = 10; //here A is a variable - comment
        System.out.println(A);
    }
}
```

Output:

```
10
```

### Example 2 - Print a variable with multiline comment

```java
class A {
    public static void main(String[] args) {
        /* Multiline Comment :
        Let's declare and
        print variable in java. */
        int A = 10;
        System.out.println(A);
    }
}
```

Output:

```
10
```

### Example 3 - Print a simple string

```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Hello Java");
    }
}
```

Output:

```
Hello Java
```

### Example 4 - Print a single line comment

```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Single Line Comments");
        //Single Line Comments
    }
}
```

Output:

```
Single Line Comments
```

### Example 5 - Print a multiline comment

```java
public class Main {
    public static void main(String[] args) {
        /*the code below will print multiline comment
        to the Screen
        Happy Learning.
        Thank you
         */
        System.out.println("Multiline Comments");
    }
}
```

Output:

```
Multiline Comments
```

### Example 6 - Print a string variable

```java
public class Main {
    public static void main(String[] args) {
        String name = "Focus";
        System.out.println(name);
    }
}
```

Output:

```
Focus
```

### Example 7 - Print an integer variable

```java
public class Main {
    public static void main(String[] args) {
        int myAge = 25;
        System.out.println(myAge);
    }
}
```

Output:

```
25
```

### Example 8 - Print an integer variable declared and initialized separately

```java
public class Main {
    public static void main(String[] args) {
        int myAge;
        myAge = 25;
        System.out.println(myAge);
    }
}
```

Output:

```
25
```

### Example 9 - Print an integer variable with updated value

```java
public class Main {
    public static void main(String[] args) {
        int myAge = 20;
        myAge = 25;
        System.out.println(myAge);
    }
}
```

Output:

```
25
```

### Example 10 - Print a final integer variable

```java
public class Main {
    public static void main(String[] args) {
        final int myAge = 20;
        myAge = 25; //will Generate an Error
        System.out.println(myAge);
    }
}
```

Output:

```
Error: cannot assign a value to final variable myAge
```

### Example 11 - Concatenating strings

```java
public class Main {
    public static void main(String[] args) {
        String title = "Practice";
        System.out.println(title + " Java Example ");
    }
}
```

Output:

```
Practice Java Example 
```

### Example 12 - Concatenating strings to form a full name

```java
public class Main {
    public static void main(String[] args) {
        String firstName = "Tom";
        String secondName = " Hank";
        String fullName = firstName + secondName;
        System.out.println(fullName);
    }
}
```

Output:

```
Tom Hank
```

### Example 13 - Sum of integers

```java
public class Main {
    public static void main(String[] args) {
        int x = 10, y = 20, z = 30;
        System.out.println(x + y + z);
    }
}
```

Output:

```
60
```

### Example 14 - Declaring variables

```java
class Example {
   public static void main(String args[]) { 
        byte b;
        short s;
        int i;
        float f;   
        char c;	   
        double d; 
        boolean boo; 
        long l;  
           
        System.out.println("Variable Example created successfully");
   }
}
```

Output:

```
Variable Example created successfully
```

### Example 15 - Storing data

```java
class Example {
   public static void main(String args[]) { 
        int i=5;
        float f=5.5f;
        char c=  'a';
        double d=123456.789; 
        boolean b=true;
        System.out.println("Data stored");
  }
}
```

Output:

```
Data stored
```

### Example 16 - Declaring multiple variables

```java
class Example {
   public static void main(String args[]) { 
        int i1, i2, i3, i4;
        float f1, f2, f3, f4;
        char c1, c2, c3, c4;	   
        double d1, d2, d3, d4;   
        boolean b1, b2, b3, b4;  

        System.out.println("More than one variable created successfully");
   }
}
```

Output:

```
More than one variable created successfully
```

### Example 17 - Declaring variables with different names

```java
class Example {
   public static void main(String args[]) { 
        int examples;
        int a;
        int A;
        int xyz;
        int abc;
        double a1;
        double ABc;
        char java;
        char c1;
        boolean C$_;
          
        System.out.println("Variables named using lower, uppercase, digits, and symbols ($, _) successfully");
   }
}
```

Output:

```
Variables named using lower, uppercase, digits, and symbols ($, _) successfully
```

### Example 18 - Declaring variables with different names

```java
class Example {
   public static void main(String args[]) { 
        int examples;
        int a;
        int A;
        int xyz;
        int abc;
        double a1;
        double ABc;
        char java;
        char c1;
        boolean C$_;
          
        System.out.println("Variables named using lower, uppercase, digits, and symbols ($, _) successfully");
   }
}
```

Output:

```
Variables named using lower, uppercase, digits, and symbols ($, _) successfully
```

### Example 19 - Declaring variables with different names

```java
class Example {
   public static void main(String args[]) { 
        int  a1; 
        int hello;
        int javaprogramshub;
        char object_oriented_programming;
        float qwertyuiopax;
        int abcdefghijklmnop123$_;
        double subject_is_more_important_than_marks; 
   }
}
```

Output:

No output

### Example 20 - Using an uninitialized variable

```java
class Example {
    public static void main(String args[]) {
        int a;
        System.out.println(a);// error: variable a might not have been initialized 
    }
}
```

Output:

```
error: variable a might not have been initialized 
```

### Example 21 - Declaring Variables with Keywords

```java
class Variables {
    public static void main(String args[]) {
        int char;           // error: char is a keyword
        int class;          // error: class is a keyword
        int int;            // error: int is a keyword
        int if;             // error: if is a keyword
        int while;          // error: while is a keyword
        int CHAR;           // no error, CHAR is not a keyword
    }
}
```

Output:

```
error: not a statement
        int char;           // error: char is a keyword
            ^
error: not a statement
        int class;          // error: class is a keyword
             ^
error: not a statement
        int int;            // error: int is a keyword
           ^
error: not a statement
        int if;             // error: if is a keyword
           ^
error: not a statement
        int while;          // error: while is a keyword
              ^
```

### Example 22 - Redeclaring Variables

```java
class Example {
    public static void main(String args[]) {
        int a;
        float a;  // error: a is already defined in method main(String[])
        int b;
        int b;   // error: b is already defined in method main(String[])
        float b;  // error: b is already defined in method main(String[])
    }
}
```

Output:

```
error: variable a is already defined in method main(String[])
        float a;  // error: a is already defined in method main(String[])
              ^
error: variable b is already defined in method main(String[])
        int b;   // error: b is already defined in method main(String[])
            ^
error: variable b is already defined in method main(String[])
        float b;  // error: b is already defined in method main(String[])
              ^
```

### Example 23 - Creating Variables Anywhere in the Program

```java
class A {
    public static void main(String args[]) {
        int a = 10;
        System.out.println(a);

        int b = 20;
        System.out.println(b);

        int c = a + b;
        System.out.println(c);

        int d = 40;
        System.out.println(d);

        int x = 22;
    }
}
```

Output:

```
10
20
30
40
```

### Example 24 - Using a Variable Outside its Scope

```java
class A {
    public static void main(String args[]) {
        for (int i = 1; i < 4; i++) {
            System.out.println(i);  // 1 2 3
        }
        System.out.println(i);  // error: cannot find symbol
    }
}
```

Output:

```
1
2
3
error: cannot find symbol
        System.out.println(i);
                           ^
  symbol:   variable i
  location: class A
```

### Example 25 - Creating Variables in a Method

```java
class A {
    public void age() {
        int age = 0;
        age = age + 9;
        System.out.println("Sohan age is : " + age);
    }

    public static void main(String args[]) {
        A test = new A();
        test.age();
    }
}
```

Output:

```
Sohan age is : 9
```

### Example 26 - Using Instance and Private Variables

```java
class Employee {
    public String name;     // this instance variable is visible for any child class.
    private double salary; // salary variable is visible in Employee class only.

    // The name variable is assigned in the constructor.
    public Employee(String empName) {
        name = empName;
    }

    // The salary variable is assigned a value.
    public void setSalary(double empSal) {
        salary = empSal;
    }

    // This method prints the employee details.
    public void printEmp() {
        System.out.println("Name of Employee : " + name);
        System.out.println("Total salary of " + name + " is " + salary);
    }

    public static void main(String args[]) {
        Employee empOne = new Employee("Tom");
        empOne.setSalary(150000);
        empOne.printEmp();
    }
}
```

Output:

```
Name of Employee : Tom
Total salary of Tom is 150000.0
```

### Example 27 - Using Static and Final Variables

```java
class Employee {
    private static double salary;   // salary variable is a private static variable
    public static final String DEPARTMENT = "IT";    // DEPARTMENT is a constant

    public static void main(String args[]) {
        salary = 10000;
        System.out.println(DEPARTMENT + " Average Salary: "10000.0");
    }
}
```

Output:

```
IT Average Salary: 10000.0
```

### Example 28 - Checking if an Object is an Instance of a Class

```java
class Main {
    public static void main(String[] args) {
        String str = "Welcome";
        boolean result;

        // checks if str is an instance of
        // the String class
        result = str instanceof String;
        System.out.println("Is str an object of String? " + result);
    }
}
```

Output:

```
Is str an object of String? true
```

### Example 29 - Using the Ternary Operator

```java
class Java {
    public static void main(String[] args) {
        int februaryDays = 29;
        String result;

        // ternary operator
        result = (februaryDays == 28) ? "Not a leap year" : "Leap year";
        System.out.println(result);
    }
}
```

Output:

```
Leap year
```

### Example 30 - Printing a Message

```java
class AssignmentOperator {
    public static void main(String[] args) {
        System.out.println("Java programming is interesting.");
    }
}
```

Output:

```
Java programming is interesting.
```

### Example 31: Printing Text on Console

```java
// Printing Text on Console

public class Output {
    public static void main(String[] args) {
        System.out.println("1. println ");
        System.out.println("2. println ");
        System.out.print("1. print ");
        System.out.print("2. print");
    }
}
```

Output:

```
1. println 
2. println 
1. print 2. print
```

### Example 32: Declaring and Printing Variables

```java
// Declaring and Printing Variables

public class Variables {
    public static void main(String[] args) {
        Double number = -19.2;
        System.out.println(3);
        System.out.println(number);
    }
}
```

Output:
```
3
-19.2
```

### Example 33: Printing Variables with Text

```java
// Printing Variables with Text

public class PrintVariables {
    public static void main(String[] args) {
        int number = 123654987;
        System.out.println("I am " + "Tom");
        System.out.println("Mobile Number = " + number);
    }
}
```

Output:
```
I am Tom
Mobile Number = 123654987
```

### Example 34: Getting Integer Input From the User

```java
import java.util.Scanner;

// Getting Integer Input From the User

public class Input {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.print("Enter an integer: ");
        int number = input.nextInt();
        System.out.println("You entered " + number);
        input.close();
    }
}
```

Output:

```
Enter an integer: 123
You entered 123
```

### Example 35: Getting float, double and String Input

```java
import java.util.Scanner;

// Getting float, double and String Input

public class Input {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.print("Enter float: ");
        float myFloat = input.nextFloat();
        System.out.println("Float entered = " + myFloat);
        System.out.print("Enter double: ");
        double myDouble = input.nextDouble();
        System.out.println("Double entered = " + myDouble);
        System.out.print("Enter text: ");
        String myString = input.next();
        System.out.println("Text entered = " + myString);
        input.close();
    }
}
```

Output:

```
Enter float: 1.23
Float entered = 1.23
Enter double: -12.3
Double entered = -12.3
Enter text: Java
Text entered = java
```

### Example 36: Using if statement

```java
// Using if statement

public class Main {
    public static void main(String[] args) {
        String band = "LK";
        if (band == "LK") {
            System.out.print("Hey ");
            System.out.print("Chester");
        }
    }
}
```

Output:

```
Hey Chester
```

### Example 37: Using if statement with block

```java
// Using if statement with block

public class Main {
    public static void main(String[] args) {
        if (10 > 5) {
            System.out.println("Block Statement");
        }
    }
}
```

Output:

```
Block Statement
```

### Example 38: Using block statement

```java
// Using block statement

public class Main {
    public static void main(String[] args) {
        {
            System.out.println("Hello");
            System.out.println("java");
            System.out.println("Programmer");
        }
    }
}
```

Output:

```
Hello
java
Programmer
```

### Example 39: Multi-line Comment

```java
/* This is an example of  multi-line comment.
 * The program prints "Hello, World!" to the standard output.
 */

public class HelloWorld {
    public static void main(String[] args) {    	
    {	
        System.out.println("Java Is Awesome");
    }
}
```

Output:

```
Java Is Awesome
```

### Example 40: Declaring and Printing a Final Variable

```java
// Declaring and Printing a Final Variable

public class A {
    public static void main(String args[]) {
        final int i;
        i = 1234;
        System.out.println(i);
    }
}
```

Output:

```
1234
```



### Example 41: Using Final with for-each Statement

```java
// Java program to demonstrate final 
// with for-each statement
 
class A {
 
    // Main driver method
    public static void main(String[] args)
    {
 
        // Declaring and initializing
        // custom integer array
        int arr[] = { 1, 2, 3 };
 
        // final with for-each statement
        // legal statement
        for (final int i : arr)
            System.out.print(i + " ");
    }
}
```

Output:

```
1 2 3
```

### Example 42: Printing Text on Console

```java
// Java program to print text on console
 
class Simple {
    public static void main(String args[]) {
        System.out.println("Hello Java");
    }
}
```

Output:

```
Hello Java
```

### Example 43: Performing Addition Operation

```java
// Java program to perform addition operation
 
class Calculation {
    public static void main(String[] args) {
        int a = 10;
        int b = 10;
        int c = a + b;
        System.out.println(c);
    }
}
```

Output:

```
20
```

### Example 44: Type Casting Integer to Float

```java
// Java program to demonstrate type casting of integer to float
 
class A {
    public static void main(String[] args) {
        int a = 5;
        float f = a;
        System.out.println(a);
        System.out.println(f);
    }
}
```

Output:

```
5
5.0
```

### Example 45: Type Casting Float to Integer

```java
// Java program to demonstrate type casting of float to integer
 
class A {

    public static void main(String[] args) {
        float f = 12.3f;
        //int a=f;//Compile time error
        int a = (int) f;
        System.out.println(f);
        System.out.println(a);
    }
}
```

Output:

```
12.3
12
```

### Example 46: Type Casting Integer to Byte (Overflow)

```java
// Java program to demonstrate type casting of integer to byte (Overflow)

class A {
    public static void main(String[] args) {
        //Overflow
        int a = 130;
        byte b = (byte) a;
        System.out.println(a);
        System.out.println(b);
    }
}
```

Output:

```
130
-126
```

### Example 47: Type Casting Byte to Byte

```java
// Java program to demonstrate type casting of byte to byte
 
class A {

    public static void main(String[] args) {
        byte a = 10;
        byte b = 10;
        //byte c=a+b;//Compile Time Error: because a+b=20 will be int
        byte c = (byte) (a + b);
        System.out.println(c);
    }
}
```

Output:

```
20
```

### Example 48: Increment and Decrement Operators

```java
// Java program to demonstrate increment and decrement operators
 
class Operator {
    public static void main(String[] args) {
        int x = 5;
        System.out.println(x++);
        System.out.println(++x);
        System.out.println(x--);
        System.out.println(--x);
    }
}
```

Output:

```
5
7
7
5
```

### Example 49: Combination of Increment and Addition Operators

```java
// Java program to demonstrate combination of increment and addition operators

class Operator {
    public static void main(String[] args) {
        int a = 10;
        int b = 10;
        System.out.println(a++ + ++a);//10+12=22
        System.out.println(b++ + b++);//10+11=21

    }
}
```

Output:

```
22
21
```

### Example 50: Bitwise and Logical Operators

```java
// Java program to demonstrate bitwise and logical operators
 
class Operator {
    public static void main(String[] args) {
        int a = 10;
        int b = -10;
        boolean c = true;
        boolean d = false;
        System.out.println(~a);
        System.out.println(~b);
        System.out.println(!c);//false (opposite of boolean value)
        System.out.println(!d);//true
    }
}
```

Output:

```
-11
9
false
true
```
