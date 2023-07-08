## Java HashMap Examples

### Example 1: Creating a HashMap and adding key-value pairs

```java
import java.util.HashMap;

public class Example1 {
    public static void main(String[] args) {
        HashMap<String, String> Employee = new HashMap<>();
        Employee.put("Tom", "London");
        Employee.put("Neo", "Berlin");
        Employee.put("Frank", "Oslo");
        Employee.put("Drake", "Washington DC");
        System.out.println(Employee);
    }
}
```

##### Output:
```
{Tom=London, Neo=Berlin, Frank=Oslo, Drake=Washington DC}
```

### Example 2: Retrieving a value from a HashMap using key

```java
import java.util.HashMap;

public class Example2 {
    public static void main(String[] args) {
        HashMap<String, String> Employee = new HashMap<>();
        Employee.put("Tom", "London");
        Employee.put("Neo", "Berlin");
        Employee.put("Frank", "Oslo");
        Employee.put("Drake", "Washington DC");
        System.out.println(Employee.get("Frank"));
    }
}
```

##### Output:
```
Oslo
```

### Example 3: Removing a key-value pair from a HashMap

```java
import java.util.HashMap;

public class Example3 {
    public static void main(String[] args) {
        HashMap<String, String> Employee = new HashMap<>();
        Employee.put("Tom", "London");
        Employee.put("Neo", "Berlin");
        Employee.put("Frank", "Oslo");
        Employee.put("Drake", "Washington DC");
        Employee.remove("Neo");
        System.out.println(Employee);
    }
}
```

##### Output:
```
{Tom=London, Frank=Oslo, Drake=Washington DC}
```

### Example 4: Clearing a HashMap

```java
import java.util.HashMap;

public class Example4 {
    public static void main(String[] args) {
        HashMap<String, String> Employee = new HashMap<>();
        Employee.put("Tom", "London");
        Employee.put("Neo", "Berlin");
        Employee.put("Frank", "Mumbai");
        Employee.put("Drake", "Washington DC");
        Employee.clear();
        System.out.println(Employee);
    }
}
```

##### Output:
```
{}
```

### Example 5: Getting the size of a HashMap

```java
import java.util.HashMap;

public class Example5 {
    public static void main(String[] args) {
        HashMap<String, String> Employee = new HashMap<>();
        Employee.put("Tom", "London");
        Employee.put("Neo", "Berlin");
        Employee.put("Frank", "Mumbai");
        Employee.put("Drake", "Washington DC");
        System.out.println(Employee.size());
    }
}
```

##### Output:
```
4
```

### Example 6: Iterating over a HashMap using keySet()

```java
import java.util.HashMap;

public class Example6 {
    public static void main(String[] args) {
        HashMap<String, String> Employee = new HashMap<>();
        Employee.put("Tom", "London");
        Employee.put("Neo", "Berlin");
        Employee.put("Frank", "Mumbai");
        Employee.put("Drake", "Washington DC");
        for (String i : Employee.keySet()) {
            System.out.println("key: " + i + " value: " + Employee.get(i));
        }
    }
}
```

##### Output:
```
key: Tom value: London
key: Neo value: Berlin
key: Frank value: Mumbai
key: Drake value: Washington DC
```

### Example 7: Iterating over a HashMap using entrySet()

```java
import java.util.HashMap;
import java.util.Map;

public class Example7 {
    public static void main(String[] args) {
        HashMap<String, Integer> people = new HashMap<>();
        people.put("Tom", 25);
        people.put("Neo", 20);
        people.put("Frank", 23);

        for (Map.Entry<String, Integer> entry : people.entrySet()) {
            System.out.println("Name: " + entry.getKey() + " Age: " + entry.getValue());
        }
    }
}
```

##### Output:
```
Name: Tom Age: 25
Name: Neo Age: 20
Name: Frank Age: 23
```

### Example 8: Retrieving values from a HashMap using get()

```java
import java.util.HashMap;

public class Example8 {
    public static void main(String[] args) {
        HashMap<Integer, String> hm = new HashMap<>();
        hm.put(25, "Tom");
        hm.put(20, "Neo");
        hm.put(28, "Frank");
        hm.put(21, "Drake");
        String s = hm.get(20);
        System.out.println(s);
        s = hm.get(21);
        System.out.println(s);
    }
}
```

##### Output:
```
Neo
Drake
```

### Example 9: Checking if a key exists in a HashMap using containsKey()

```java
import java.util.HashMap;

public class Example9 {
    public static void main(String[] args) {
        HashMap<String, String> Employee = new HashMap<>();
        Employee.put("Tom", "London");
        Employee.put("Neo", "Berlin");
        Employee.put("Frank", "Oslo");
        Employee.put("Drake", "Washington DC");
        if (Employee.containsKey("Neo")) {
            System.out.println("Neo is an employee.");
        } else {
            System.out.println("Neo is not an employee.");
        }
        if (Employee.containsKey("Sam")) {
            System.out.println("Sam is an employee.");
        } else {
            System.out.println("Sam is not an employee.");
        }
    }
}
```

##### Output:
```
Neo is an employee.
Sam is not an employee.
```

### Example 10: Checking if a value exists in a HashMap using containsValue()

```java
import java.util.HashMap;

public class Example10 {
    public static void main(String[] args) {
        HashMap<String, String> Employee = new HashMap<>();
        Employee.put("Tom", "London");
        Employee.put("Neo", "Berlin");
        Employee.put("Frank", "Oslo");
        Employee.put("Drake", "Washington DC");
        if (Employee.containsValue("Berlin")) {
            System.out.println("There is an employee in Berlin.");
        } else {
            System.out.println("There is no employee in Berlin.");
        }
        if (Employee.containsValue("Mumbai")) {
            System.out.println("There is an employee in Mumbai.");
        } else {
            System.out.println("There is no employee in Mumbai.");
        }
    }
}
```

##### Output:
```
There is an employee in Berlin.
There is no employee in Mumbai.
```

## Example 11 - Retrieving values from a HashMap in Java

```java
import java.util.Collection;
import java.util.Iterator;
import java.util.HashMap;

class Check {
    public static void main(String[] arg) {
        HashMap<Integer, String> hm = new HashMap<Integer, String>();

        hm.put(17,"Tom");
        hm.put(57,"Neo");
        hm.put(50,"Drake");
        hm.put(33,"Taylor");
        hm.put(71,"Alex");
        hm.put(99,"Robert");
        hm.put(11,"John");

        Collection col = hm.values();

        Iterator trav = col.iterator();

        while(trav.hasNext()) {
            String value = (String)trav.next();  // will give next Value
            System.out.println(value);
        }
    }
}
```

##### Output:
```
Tom
Taylor
Drake
Robert
Alex
Neo
John
```

## Example 12 - Storing objects as values in a HashMap in Java

```java
import java.util.HashMap;
import java.util.Iterator;
import java.util.Map;

class Xyz {
    String name;
    String clg;
    String branch;
    double per;

    Xyz(String s1, String s2, String s3, double p) {
        name = s1;
        clg = s2;
        branch = s3;
        per = p;
    }
}

class Check {
    public static void main(String arg[]) {
        HashMap<Integer, Xyz> hm = new HashMap<Integer, Xyz>();

        Xyz x1 = new Xyz("Tom", "NIT", "cse", 68.5);
        Xyz x2 = new Xyz("Neo", "NIT", "ecm", 70);
        Xyz x3 = new Xyz("Frank", "NIT", "ecm", 75);
        Xyz x4 = new Xyz("Drake", "NIT", "ECM", 80);
        Xyz x5 = new Xyz("Napster", "NIT", "EEE", 85);

        hm.put(1, x1);
        hm.put(2, x2);
        hm.put(3, x3);
        hm.put(4, x4);
        hm.put(5, x5);

        Iterator trav = hm.entrySet().iterator();

        while (trav.hasNext()) {
            Map.Entry record = (Map.Entry) trav.next();  // will give next (Key, Value) pair
            Xyz j = (Xyz) record.getValue();
            System.out.println(record.getKey() + " " + j.name + " " + j.clg + " " + j.branch + " " + j.per);
        }
    }
}
```

##### Output:
```
1 Tom NIT cse 68.5
2 Neo NIT ecm 70.0
3 Frank NIT ecm 75.0
4 Drake NIT ECM 80.0
5 Napster NIT EEE 85.0
```
