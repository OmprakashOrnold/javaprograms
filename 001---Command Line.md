
##### Example : 1 - Without command line arguments 
```java
class A {
    public static void main(String[] args) {
        System.out.println("Hello java");
    }
}
```
OUTPUT:
     compilation:javac A.java
     execution:java A 
     output:hello world

##### Example :  2  - With command line arguments : 
```java
class A
{
  public static void main(String args[])
  {
   System.out.println(args[0]);
   System.out.println(args[1]);
  }
}
````
OUTPUT:
     compilation:javac A.java
     execution:java A 10 20
     Output : 10 20


##### Example : 3  - Another Example same as like 
Command Line arguments passing inputs :Java
```java
class A
{
  public static void main(String args[])
  {
 
   System.out.println(args[0]);
   System.out.println(args[1]); 
   System.out.println(args[2]);
   System.out.println(args[3]);
  }
}
```
OUTPUT:

   Compile   : javac A.java
   Execution : java A   10   2.5   a   helloworld
   Output    :    10 2.5 a helloworld


##### Example : 4  - (Sample Error Program )
```java
class A
{
  public static void main(String args[])
  {
 
   System.out.println(args[0]); 
   System.out.println(args[1]);
   System.out.println(args[2]);
   
  }
}
```
OUTPUT:

Compile : Javac A.java
execution:java A   10 20
Output : Exception occur called ArrayOutOfBoundException() because access args[2] is not valid and there is no data to acces after 10,20 
it gives exception // Error //


##### Example : 5 - ( Without Parse ) 

```java
class A
{
  public static void main(String args[])
  {
 
   System.out.println(args[0]+1);
   System.out.println(args[1]+1);
 
 
  }
}
```
OUTPUT:

Compile : Javac A.java
Execution : Java A  10 20
Output : 101 201

##### Example : 6 -  ( With Parse ) : 
```java
Program with parse :Java

class A
{
  public static void main(String args[])
  {
  int a=Integer.parseInt(args[1]);//"10" convert to 10 and it will store in a
  int b=Integer.parseInt(args[0]);//"20" convert to 20 and it will store in b
   System.out.println(a+1);
   System.out.println(b+1);

  }
}
```
OUTPUT:
Compile : Javac A.java
Execution : Java A 10 20 
Output : 11 21

##### Example :7  - Command-Line Arguments
```java
class Main {
  public static void main(String[] args) {
    System.out.println("Command-Line arguments are");

    // loop through all arguments
    for(String str: args) {
      System.out.println(str);
    }
  }
}
```
OUTPUT:
 To compile the code:
javac Main.java

To run the code:
java Main

java Main hello java world

Output:
Command-Line arguments are
hello
java
world

##### Example :8  - Numeric Command-Line Arguments #7
```java
class Main {
  public static void main(String[] args) {

    for(String str: args) {
      // convert into integer type
    int argument = Integer.parseInt(str);
    System.out.println("Argument in integer form: " + argument);
    }

  }
}
```
OUTPUT:

// compile the code
javac Main.java

// run the code
java Main 11 23

Arguments in integer form
11
23

##### Example :9  - Read a Line of Text Using Scanner
```java
import java.util.Scanner;

class Main {
  public static void main(String[] args) {

    // creates an object of Scanner
    Scanner input = new Scanner(System.in);

    System.out.print("Enter your name: ");

    // takes input from the keyboard
    String name = input.nextLine();

    // prints the name
    System.out.println("My name is " + name);

    // closes the scanner
    input.close();
  }
}
```

OUTPUT:

Enter your name: Tom
My name is Tom


##### Example : 10 - Java Scanner nextInt() 

```java
import java.util.Scanner;

class Main {

  public static void main(String[] args) {

    // creates a Scanner object
    Scanner input = new Scanner(System.in);

    System.out.println("Enter an integer: ");

    // reads an int value
    int data1 = input.nextInt();

    System.out.println("Using nextInt(): " + data1);

    input.close();
  }
}
```
OUTPUT:

Enter an integer:
123
Using nextInt(): 123

##### Example :11 -  Java Scanner nextDouble()

```java
import java.util.Scanner;

class Main {
  public static void main(String[] args) {

    // creates an object of Scanner
    Scanner input = new Scanner(System.in);
    System.out.print("Enter Double value: ");

    // reads the double value
    double value = input.nextDouble();
    System.out.println("Using nextDouble(): " + value);

    input.close();
  }
}
```
OUTPUT:

Enter Double value: 98.76
Using nextDouble(): 98.76


##### Example : 12  - Java Scanner next() 

```java
import java.util.Scanner;

class Main {
  public static void main(String[] args) {

    // creates an object of Scanner
    Scanner input = new Scanner(System.in);
    System.out.print("Enter your name: ");

    // reads the entire word
    String value = input.next();
    System.out.println("Using next(): " + value);

    input.close();
  }
}
```
OUTPUT:

Enter your name: Tom Hank
Using next(): Tom Hank


##### Example : 13 -  Java Scanner nextLine() 

```java
import java.util.Scanner;

class A {
    public static void main(String[] args) {

        // creates an object of Scanner
        Scanner input = new Scanner(System.in);
        System.out.print("Enter your name: ");

        // reads the entire line
        String value = input.nextLine();
        System.out.println("Using nextLine(): " + value);

        input.close();
    }
}
```
OUTPUT:

Enter your name: tom
Using nextLine(): tom


##### Example : 14 - Read BigInteger and BigDecimal 

```java
import java.math.BigDecimal;
import java.math.BigInteger;
import java.util.Scanner;

class A {
    public static void main(String[] args) {

        // creates an object of Scanner
        Scanner input = new Scanner(System.in);
        System.out.print("Enter a big integer: ");

        // reads the big integer
        BigInteger value1 = input.nextBigInteger();
        System.out.println("Using nextBigInteger(): " + value1);

        System.out.print("Enter a big decimal: ");

        // reads the big decimal
        BigDecimal value2 = input.nextBigDecimal();
        System.out.println("Using nextBigDecimal(): " + value2);

        input.close();
    }
}
```
OUTPUT:

Enter a big integer: 123456789
Using nextBigInteger(): 123456789
Enter a big decimal: 1.23456789
Using nextBigDecimal(): 1.23456789



