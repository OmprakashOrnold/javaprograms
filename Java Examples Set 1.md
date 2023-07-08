## Example 1: Finding Square Root

```java
import java.util.Scanner;

public class SquareRoot {

   public static void main(String[] args) {

      // declare variables
      double number = 0;
      double squareRoot = 0;

      // read input from console
      Scanner scan = new Scanner(System.in);
      System.out.print("Enter a number: ");
      number = scan.nextDouble();

      // find sqrt() value
      squareRoot = Math.sqrt(number);

      // display result
      System.out.println("Square root "
		+ "value = "+ squareRoot);

      // close Scanner class object
      scan.close();
   }
}
```

### Output
```
Enter a number: 25
Square root value = 5.0
```

##  Example 2: Displaying Numbers using Recursion

```java
public class KnowProgram {
  public static void main(String[] args) {

    // variable
    int n = 10;

    // method call
    System.out.println("Displaying from 1 to 100: ");
    display(n);
  }

  // recursive method
  public static void display(int n) {
     if(n > 1)
       display(n-1);
     System.out.print(n+" ");
  }

}
```

### Output
```
Displaying from 1 to 100: 
1 2 3 4 5 6 7 8 9 10 
```

##  Example 3: Basic Calculator
```java
import java.util.Scanner;

public class BasicCalculator {

   public static void main(String[] args) {

      // Declare variables
      double num1=0.0, num2=0.0;
      char operator='\0';

      // create Scanner class object to
      // read inputs
      Scanner scan = new Scanner(System.in);
      System.out.print("Enter two numbers: ");
      num1 = scan.nextDouble();
      num2 = scan.nextDouble();

      // read operator
      System.out.println("Available Operators"
		+ "are::  (+ - * / % ^)");
      System.out.print("Enter operator: ");
      operator = scan.next().charAt(0);

      // switch-case statements
      switch(operator) {

         case '+':
            System.out.println("Result = "+ (num1+num2));
		break;

	 case '-':
	    System.out.println("Result = "+ (num1-num2));
		break;

	 case '*':
	    System.out.println("Result = "+ (num1*num2));
		break;

	 case '/':
	    System.out.println("Result = "+ (num1/num2));
		break;

	 case '%':
	    System.out.println("Result = "+ (num1%num2));
		break;

	 case '^':
	    System.out.println("Result = "+
                               Math.pow(num1,num2));
		break;

	 default:
	    System.out.println("Invalid operator");
      } // end of switch-case

      // close Scanner class object
      scan.close();

   }
}
```

### Output
```
Enter two numbers: 10 20
Available Operatorsare:: (+ – * / % ^)
Enter operator: +
Result = 30.0
```

##  Example 4: Generating Fibonacci Series
```java
import java.util.Scanner;

public class FibonacciSeries {
   public static int fibonacci(int n) {
      return (n<=1) ? n :
	  (fibonacci(n-1) + fibonacci(n-2) );
   }

   public static void main(String[] args) {
      int term; // range value

      // Read range value
      Scanner scan = new Scanner(System.in);
      System.out.print("Enter the term: ");
      term = scan.nextInt();

      // display fibonacci series
      System.out.println("First "+term+" terms of "
		+ "Fibonacci series are: ");

      for(int i=1; i<term; i++)
         System.out.print(fibonacci(i)+"\t");

       // close Scanner class object
      scan.close();
   }
}
```

### Output
```
Enter the term: 7
First 7 terms of Fibonacci series are:
1	1	2	3	5	8	
```

##  Example 5: Finding Sum of Natural Numbers

```java
import java.util.Scanner;

public class SumOfNaturalNumbers {
   public static void main(String[] args) {
      int num, sum = 0;

      // Read input from console
      Scanner scan = new Scanner(System.in);
      System.out.print("Enter a number: ");
      num = scan.nextInt();

      // Calculate sum of natural numbers
      for(int i=1; i<=num; i++) {
         sum += i;
      }

      // Display result
      System.out.println("Sum of first " + num
		+ " natural numbers is: " + sum);

      // Close Scanner class object
      scan.close();
   }
}
```

### Output
```
Enter a number: 5
Sum of first 5 natural numbers is: 15
```

## Example 6: Calculate the sum of a series

```java
public class Series {
  public static void main(String[] args) {

    int n = 5;
    int sum = 0;

    // calculate the sum of series
    sum = n*(n-1)/2;

    // display result
    System.out.println("Sum = " + sum);
  }
}
```
##### Output:
```
Sum = 10
```

## Example 7: Calculate the sum of another series

```java
public class Series {
  public static void main(String[] args) {

    int n = 5;
    int sum = 0;

    // calculate the sum of series
    sum = n*(n+1)*(2*n+1)/6;

    // display result
    System.out.println("Sum = " + sum);
  }
}
```

##### Output:
```
Sum = 55
```

## Example 8: Find the length of an array

```java
public class ArrayLength {
  public static void main(String[] args) {

    // declare and initialize an array
    int arr[] = {10, 20, 30, 40, 50};

    // display array length
    System.out.print("The length of the given array = ");
      System.out.println(arr.length);
  }
}
```

##### Output:
```
The length of the given array = 5
```

## Example 9: Display size and elements of an array

```java
class TestArray{
  public static void main(String[] args) {

    // defining array
    int[] a = {10,20,30,40,50};

    // display size of array
    System.out.println("Size = "+ a.length);

    // display array using length property
    System.out.println("Array elements:");
    for(int i=0; i < a.length; i++){
      System.out.print(a[i]+"\t");
    }

  }
}
```

##### Output:
```
Size = 5
Array elements:
10 20 30 40 50
```

## Example 10: Display elements of an array using for loop

```java
public class DisplayArray {
  public static void main(String[] args) {

    // declare and initialize an array
    int arr[] = {10, 20, 30, 40, 50};

    // display the array using for loop
    for(int i=0; i<arr.length; i++) {
      System.out.print(arr[i] + " ");
    }
  }

}
```

##### Output:
```
10 20 30 40 50
```


## Example 11: Display 2D array

```java
public class Display2DArray {
  public static void main(String[] args) {

    // declare and initialize an array
    int arr[][] = {{50,60},{70,80},{90,100}};

    // display 2D array using for-each loop
    for(int[] i : arr) {
      for(int j : i) {
        System.out.print(j + " ");
      }
    }
  }
}
```

##### Output:
```
50 60 70 80 90 100
```

## Example 12: Calculate the sum of an array

```java
public class ArraySum {
  public static void main(String[] args) {

    // declare array and
    // initialize it with values
    int array[] = {10, 20, 30, 40, 50};

    // initialize sum variable with 0
    int sum = 0;

    // add array elements
    for (int i=0; i<array.length; i++) {
      sum += array[i]; // sum = sum + array[i];
    }

    // display the result
    System.out.println("Sum of array elements= " + sum);

  }
}
```

##### Output:
```
Sum of array elements= 150
```

## Example 13: Calculate the sum of a list

```java
import java.util.List;
import java.util.ArrayList;
public class ArraySum {
  public static void main(String[] args) {

    // declare list
    List<Integer> list = new ArrayList<Integer>();

    // add elements to the list
    // you can take input from the end-user
    list.add(10);
    list.add(20);
    list.add(30);
    list.add(40);
    list.add(50);

    // initialize sum variable with 0
    int sum = 0;

    // add array elements to sum
    for (int i : list) {
      sum += i;
    }

    // display the result
    System.out.println("Sum = " + sum);

  }
}
```

##### Output:
```
Sum = 150
```

## Example 14: Calculate the average of an array

```java
public class ArrayAverage {
  public static void main(String[] args) {

    double array[] = {10, 20, 30, 40, 50};
    // declare sum variable, & initialize with 0
    double sum = 0.0;
    // declare average variable
    double avg = 0.0;

    // loop to iterate the array
    for (int i=0; i<array.length; i++) {
      // add numbers
      sum = sum + array[i];
    }

    // calculate the average value
    avg = sum/array.length;

    // display result
    System.out.println("Average: " + avg );
  }
}
```

##### Output:
```
Average: 30.0
```

## Example 15: Copy an array

```java
import java.util.Arrays;

public class CopyArray {

   public static void main(String[] args) {
      // original array
      int arr[] = { 10, 20, 30, 40, 50 };

      // copy array using clone()
      int[] newArr = arr.clone();

      // display array (Before Modification)
      System.out.println("Before Modification,");
      System.out.println("Original Array = " + Arrays.toString(arr));
      System.out.println("Copied Array = " + Arrays.toString(newArr));

      // modifying content of original array
      arr[0] = 555;
      arr[3] = 777;

      // display array (After Modification)
      System.out.println("\nAfter Modification,");
      System.out.println("Original Array = " + Arrays.toString(arr));
      System.out.println("Copied Array = " + Arrays.toString(newArr));
   }

}
```

##### Output:
```
Before Modification,
Original Array = [10, 20, 30, 40, 50]
Copied Array = [10, 20, 30, 40, 50]

After Modification,
Original Array = [555, 20, 30, 777, 50]
Copied Array = [10, 20, 30, 40, 50]
```


## Example 16 - Merging two arrays in Java

```java
import java.util.Arrays;

public class CopyArray {

   public static void main(String[] args) {

      // array which should be merged
      String src1[] = {"Java", "Python", "C++"};
      String src2[] = {"HTML", "CSS", "JavaScript"};

      // create new array
      String newArray[] = new String[src1.length + src2.length];

      // Copy first to new array from 0 to src1.length
      System.arraycopy(src1, 0, newArray, 0, src1.length);

      // copy second array to new array
      System.arraycopy(src2, 0, newArray, src1.length, src2.length);

      // display all array
      System.out.println("Array1 = " + Arrays.toString(src1));
      System.out.println("Array2 = " + Arrays.toString(src2));
      System.out.println("Merged Array = " + Arrays.toString(newArray));
   }
}
```

Output:
```
Array1 = [Java, Python, C++]
Array2 = [HTML, CSS, JavaScript]
Merged Array = [Java, Python, C++, HTML, CSS, JavaScript]
```

## Example 17 - Finding the largest number in an array in Java

```java
import java.util.Scanner;

public class ArrayProgram {

  // Java method to find largest number in array
  public static int largest(int[] array) {

    // declare a variable max
    // assign first element to max
    int max = array[0];

    // compare with remaining elements
    // loop
    for (int i = 1; i < array.length; i++) {
      if (max < array[i])
        max = array[i];
    }

    return max;
  }

  // main method
  public static void main(String[] args) {
    // create Scanner class object to read input
    Scanner scan = new Scanner(System.in);

    // declare variables
    int size = 0;
    int arr[] = null;

    // take length of the array
    System.out.print("Enter length of the array: ");
    size = scan.nextInt();

    // create array
    arr = new int[size];

    // take array inputs
    System.out.println("Enter array elements: ");
    for (int i = 0; i < arr.length; i++) {
      arr[i] = scan.nextInt();
    }

    // method call
    System.out.println("Largest element = " + largest(arr));

    // close Scanner
    scan.close();
  }
}
```

Output:
```
Enter length of the array: 5
Enter array elements:
10 5 -15 20 -30
Largest element = 20
```

## Example 18 - Searching for an element in a sorted array in Java

```java
import java.util.Arrays;
import java.util.Scanner;

public class Search {
  public static void main(String[] args) {

    // unsorted array of String
    String arr[] = {"Java", "HTML", "C++", "Python", "CSS"};

    // display initial array
    System.out.println("Initial array = " + Arrays.toString(arr));

    // sort the array
    Arrays.sort(arr);

    // display array after sorting
    System.out.println("Initial array = " + Arrays.toString(arr));

    // Scanner class object to read input
    Scanner scan = new Scanner(System.in);

    // read character
    System.out.print("Enter a string to search: ");
    String str = scan.next();

    // search character
    int index = Arrays.binarySearch(arr, str);

    // display result
    if(index != -1)
      System.out.println(str + " found at index = " + index);
    else
      System.out.println(str+" not found.");

    // close Scanner
    scan.close();
  }
}
```

Output:
```
Initial array = [Java, HTML, C++, Python, CSS]
Initial array = [C++, CSS, HTML, Java, Python]
Enter a string to search: Java
Java found at index = 3
```

## Example 19 - Removing duplicates from a sorted array in Java

```java
import java.util.Arrays;

public class ArrayTest {

   // method to remove duplicates from sorted array
   public static int[] removeDuplicates(int[] arr) {

      int j = 0; // index without duplicates
      int lastIndex = arr.length - 1;

      // loop through array
      for (int i = 0; i < lastIndex; i++) {
         // if current element is not same as next element
         if (arr[i] != arr[i + 1]) {
            // copy current element to new array
            arr[j++] = arr[i];
         }
      }

      // copy last element to new array
      arr[j++] = arr[lastIndex];

      // create new array without duplicates
      int newArr[] = Arrays.copyOf(arr, j);

      return newArr;
   }

   public static void main(String[] args) {
      // sorted array
      int arr[] = {10, 10, 20, 30, 40, 40, 50};

      // remove duplicates
      int newArr[] = removeDuplicates(arr);

      // display both arrays
      System.out.println("Original array: " + Arrays.toString(arr));
      System.out.println("After removing duplicates: " + Arrays.toString(newArr));
   }
}

// Output: 
// Original array: [10, 10, 20, 30, 40, 40, 50]
// After removing duplicates: [10, 20, 30, 40, 50]
```

## Example 20 - Adding an element to an array at a specified position in Java

```java
import java.util.ArrayList;
import java.util.Arrays;
import java.util.List;

public class ArrayTest {

   // method to add element to array and return new array
   public static Integer[] addElement(Integer[] arr, int element, int position) {

      // create ArrayList
      List<Integer> list = new ArrayList<Integer>(Arrays.asList(arr));

      // add element at specified position
      list.add(position, element);

      // return array
      return list.toArray(arr);
   }

   public static void main(String[] args) {
      // original array
      Integer arr[] = {10, 20, 30, 40, 50};

      // new element to be added
      int element = 99;

      // position to be inserted
      // Assuming array starts from 1, not 0
      int position = 3;

      // display old array
      System.out.println("Original array: " + Arrays.toString(arr));

      // add element
      arr = addElement(arr, element, position);

      // display new array
      System.out.println("New array: " + Arrays.toString(arr));
   }
}

// Output:
// Original array: [10, 20, 30, 40, 50]
// New array: [10, 20, 30, 99, 40, 50]
```

## Example 21 - Converting int to char in Java

```java
class Main {
  public static void main(String[] args) {

    // create int variables
    int num1 = 80;
    int num2 = 81;

    // convert int to char
    // typecasting
    char a = (char)num1;
    char b = (char)num2;

    // print value
    System.out.println(a);    // P
    System.out.println(b);    // Q
  }
}

// Output:
// P
// Q
```

## Example 22 - Converting long to int in Java

```java
class Main {
  public static void main(String[] args) {

    // create long variables
    long a = 2322331L;
    long b = 52341241L;

    // convert long into int
    // using typecasting
    int c = (int)a;
    int d = (int)b;

    System.out.println(c);    // 2322331
    System.out.println(d);    // 52341241
  }
}

// Output:
// 2322331
// 52341241
```

## Example 23 - Converting int to string in Java

```java
class Main {
  public static void main(String[] args) {

    // create int variables
    int num1 = 476;
    int num2 = 78656;

    // convert int to string
    // using toString()
    String str1 = Integer.toString(num1);
    String str2 = Integer.toString(num2);

    // print string variables
    System.out.println(str1);    // 476
    System.out.println(str2);    // 78656
  }
}

// Output:
// 476
// 78656
```

## Example 24 - Using constructors in inheritance in Java

```java
// superclass
class Languages {

  // constructor of the superclass
  Languages(int version1, int version2) {

    if (version1 > version2) {
      System.out.println("The latest version is: " + version1);
    }

    else {
      System.out.println("The latest version is: " + version2);
    }

  }
}

// child class
class Main extends Languages {

  // constructor of the child class
  Main() {
    // calling the constructor of super class
    super(11, 8);
  }

  // main method
  public static void main(String[] args) {

    // call the first constructor
    Main obj = new Main();

  }
}

// Output:
// The latest version is: 11
```

## Example 25 - Private constructors in Java

```java
class Test {

  // create private constructor
  private Test () {
    System.out.println("This is a private constructor.");
  }

  // create a public static method
  public static void instanceMethod() {

    // create an instance of Test class
    Test obj = new Test();
  }

}

class Main {

  public static void main(String[] args) {

    // call the instanceMethod()
    Test.instanceMethod();
  }
}

// Output:
// This is a private constructor.
```


## Example 26 - Generating random string in Java

```java
import java.util.Random;

class Main {
  public static void main(String[] args) {

    // create a string of all characters
    String alphabet = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";

    // create random string builder
    StringBuilder sb = new StringBuilder();

    // create an object of Random class
    Random random = new Random();

    // specify length of random string
    int length = 7;

    for(int i = 0; i < length; i++) {

      // generate random index number
      int index = random.nextInt(alphabet.length());

      // get character specified by index
      // from the string
      char randomChar = alphabet.charAt(index);

      // append the character to string builder
      sb.append(randomChar);
    }

    String randomString = sb.toString();
    System.out.println("Random String is: " + randomString);

  }
}

// Output:
// Random String is: ABXZMQS
```

## Example 27 - Clearing a StringBuffer in Java

```java
class Main {
  public static void main(String[] args) {

    // create a string buffer
    StringBuffer str = new StringBuffer();

    // add string to string buffer
    str.append("Java");
    str.append(" is");
    str.append(" awesome.");
    System.out.println("StringBuffer: " + str);

    // clear the string
    // using setLength()
    str.setLength(0);
    System.out.println("Updated StringBuffer: " + str);
  }
}

// Output:
// StringBuffer: Java is awesome.
// Updated StringBuffer: 
```

## Example 28 - Accessing characters in a string in Java

```java
class Main {
  public static void main(String[] args) {

    // create a string
    String name = "Hello";

    System.out.println("Characters in " + name + " are:");

    // loop through each element
    for(int i = 0; i<name.length(); i++) {

      // access each character
      char a = name.charAt(i);
      System.out.print(a + ", ");
    }
  }
}

// Output:
// Characters in Hello are:
// H, e, l, l, o, 
```

## Example 29 - Accessing characters in a string using for-each loop in Java

```java
class Main {

  public static void main(String[] args) {

    // create a string
    String name = "Hello";

    System.out.println("Characters in string \"" + name + "\":");

    // loop through each element using for-each loop
    for(char c : name.toCharArray()) {

      // access each character
      System.out.print(c + ", ");
    }

  }
}

// Output:
// Characters in string "Hello":
// H, e, l, l, o, 
```

## Example 30 - Comparing strings in Java

```java
class Main {

  public static void main(String[] args) {

    String name1 = new String("Hello");
    String name2 = new String("hello");

    System.out.println("Check if two strings are equal");

    // check if two strings are equal
    // using == operator
    boolean result1 = (name1 == name2);
    System.out.println("Using == operator: " + result1);

    // using equals() method
    boolean result2 = name1.equals(name2);
    System.out.println("Using equals(): " + result2);
  }
}

// Output:
// Check if two strings are equal
// Using == operator: false
// Using equals(): false
```

## Example 31 - Calculating compound interest in Java

```java
import java.util.Scanner;

class Main {
  public static void main(String[] args) {

    // create an object of Scanner class
    Scanner input = new Scanner(System.in);

    // take input from users
    System.out.print("Enter the principal: ");
    double principal = input.nextDouble();

    System.out.print("Enter the rate: ");
    double rate = input.nextDouble();

    System.out.print("Enter the time: ");
    double time = input.nextDouble();

    System.out.print("Enter number of times interest is compounded: ");
    int number = input.nextInt();

    double interest = principal * (Math.pow((1 + rate/100), (time * number))) - principal;

    System.out.println("Principal: " + principal);
    System.out.println("Interest Rate: " + rate);
    System.out.println("Time Duration: " + time);
    System.out.println("Number of Time interest Compounded: " + number);
    System.out.println("Compound Interest: " + interest);

    input.close();
  }
}

// Output:
// Enter the principal: 10000
// Enter the rate: 8.5
// Enter the time: 5
// Enter number of times interest is compounded: 12
// Principal: ## Example 31 - Calculating compound interest in Java

