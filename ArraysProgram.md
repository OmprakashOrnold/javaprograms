
## Find the sum of all elements in an array
```java
public static int findSum(int[] arr) {
    int sum = 0;
    for (int num : arr) {
        sum += num;
    }
    return sum;
}

```
## Calculate the average of elements in an array.
```java
public static double findAverage(int[] arr) {
    int sum = findSum(arr);
    return (double) sum / arr.length;
}

```
## Find the largest element in an array.
```java
public static int findLargestElement(int[] arr) {
    int max = arr[0];
    for (int i = 1; i < arr.length; i++) {
        if (arr[i] > max) {
            max = arr[i];
        }
    }
    return max;
}

```
## Find the second largest element in an array.
```java
public static int findSecondLargestElement(int[] arr) {
    int max = arr[0];
    int secondMax = Integer.MIN_VALUE;

    for (int i = 1; i < arr.length; i++) {
        if (arr[i] > max) {
            secondMax = max;
            max = arr[i];
        } else if (arr[i] > secondMax && arr[i] != max) {
            secondMax = arr[i];
        }
    }
    return secondMax;
}

```
## Find the smallest element in an array.
```java
public static int findSmallestElement(int[] arr) {
    int min = arr[0];
    for (int i = 1; i < arr.length; i++) {
        if (arr[i] < min) {
            min = arr[i];
        }
    }
    return min;
}

```
## Find the second smallest element in an array.
```java
public static int findSecondSmallestElement(int[] arr) {
    int min = arr[0];
    int secondMin = Integer.MAX_VALUE;

    for (int i = 1; i < arr.length; i++) {
        if (arr[i] < min) {
            secondMin = min;
            min = arr[i];
        } else if (arr[i] < secondMin && arr[i] != min) {
            secondMin = arr[i];
        }
    }
    return secondMin;
}

```
## 
```java
```
## 
```java
```
## 

## 
## 
