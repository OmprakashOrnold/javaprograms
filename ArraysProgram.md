
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
## Reverse an array in-place (without using additional arrays).
```java
public static void reverseArray(int[] arr) {
    int start = 0;
    int end = arr.length - 1;

    while (start < end) {
        int temp = arr[start];
        arr[start] = arr[end];
        arr[end] = temp;
        start++;
        end--;
    }
}

```
## Check if an array is palindrome (reads the same forwards and backward
```java
public static boolean isPalindrome(int[] arr) {
    int start = 0;
    int end = arr.length - 1;

    while (start < end) {
        if (arr[start] != arr[end]) {
            return false;
        }
        start++;
        end--;
    }
    return true;
}

```
## Find the common elements between two arrays.
```java
public static List<Integer> findCommonElements(int[] arr1, int[] arr2) {
    List<Integer> commonElements = new ArrayList<>();
    Set<Integer> set = new HashSet<>();

    for (int num : arr1) {
        set.add(num);
    }

    for (int num : arr2) {
        if (set.contains(num)) {
            commonElements.add(num);
        }
    }
    return commonElements;
}

```

## Find the intersection of two arrays
```java
public static int[] findIntersection(int[] arr1, int[] arr2) {
    Set<Integer> set1 = new HashSet<>();
    Set<Integer> intersection = new HashSet<>();

    for (int num : arr1) {
        set1.add(num);
    }

    for (int num : arr2) {
        if (set1.contains(num)) {
            intersection.add(num);
        }
    }

    int[] result = new int[intersection.size()];
    int index = 0;
    for (int num : intersection) {
        result[index++] = num;
    }
    return result;
}

```

## Merge two sorted arrays into a single sorted array.

```java
public static int[] mergeSortedArrays(int[] arr1, int[] arr2) {
    int[] mergedArray = new int[arr1.length + arr2.length];
    int i = 0, j = 0, k = 0;

    while (i < arr1.length && j < arr2.length) {
        if (arr1[i] < arr2[j]) {
            mergedArray[k++] = arr1[i++];
        } else {
            mergedArray[k++] = arr2[j++];
        }
    }

    while (i < arr1.length) {
        mergedArray[k++] = arr1[i++];
    }

    while (j < arr2.length) {
        mergedArray[k++] = arr2[j++];
    }

    return mergedArray;
}

```
## Rotate an array to the right by a given number of steps
```java
public static void rotateArrayRight(int[] arr, int steps) {
    int n = arr.length;
    steps = steps % n;

    reverseArray(arr, 0, n - 1);
    reverseArray(arr, 0, steps - 1);
    reverseArray(arr, steps, n - 1);
}

private static void reverseArray(int[] arr, int start, int end) {
    while (start < end) {
        int temp = arr[start];
        arr[start] = arr[end];
        arr[end] = temp;
        start++;
        end--;
    }
}

```
## Find the missing number in a given range of an array
```java
public static int findMissingNumber(int[] arr, int n) {
    int sum = (n * (n + 1)) / 2;
    for (int num : arr) {
        sum -= num;
    }
    return sum;
}

```
## Move all zeros to the end of the array while maintaining the relative order of other elements.
```java
public static void moveZerosToEnd(int[] arr) {
    int index = 0;
    for (int num : arr) {
        if (num != 0) {
            arr[index++] = num;
        }
    }

    while (index < arr.length) {
        arr[index++] = 0;
    }
}

```
## Given an array, find the subarray with the maximum sum (Kadane's algorithm).
```java
public static int findMaxSubarraySum(int[] arr) {
    int maxSum = arr[0];
    int currentSum = arr[0];

    for (int i = 1; i < arr.length; i++) {
        currentSum = Math.max(arr[i], currentSum + arr[i]);
        maxSum = Math.max(maxSum, currentSum);
    }
    return maxSum;
}

```
## Find the equilibrium index of an array (the point where the sum of elements on the left equals the sum of elements on the right
```java
public static int findEquilibriumIndex(int[] arr) {
    int totalSum = findSum(arr);
    int leftSum = 0;

    for (int i = 0; i < arr.length; i++) {
        totalSum -= arr[i];
        if (leftSum == totalSum) {
            return i;
        }
        leftSum += arr[i];
    }
    return -1; // Equilibrium index not found
}

```
## Remove duplicates from a sorted array (modify the array in-place)
```java
public static int removeDuplicates(int[] arr) {
    int n = arr.length;
    if (n == 0 || n == 1) {
        return n;
    }

    int j = 0;
    for (int i = 0; i < n - 1; i++) {
        if (arr[i] != arr[i + 1]) {
            arr[j++] = arr[i];
        }
    }
    arr[j++] = arr[n - 1];
    return j;
}

```
## 
```java
```
## 
```java
```
