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
