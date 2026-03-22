# EXPERIMENT 5

# Experiment 5A

## TITLE : Implement the Interface java.

## SOURCE CODE:

---

### source code of Sortable java:

```

public interface Sortable {
    void sort(int[] arr);
}

```

### source code of Bubble Sort java:

```

class BubbleSort implements Sortable {

    public void sort(int[] arr) {
        int n = arr.length;

        for (int i = 0; i < n - 1; i++) {
            for (int j = 0; j < n - i - 1; j++) {

                if (arr[j] > arr[j + 1]) {
                    // swap
                    int temp = arr[j];
                    arr[j] = arr[j + 1];
                    arr[j + 1] = temp;
                }
            }
        }
    }
}

```

### source code of Selection Sort java:

```

class SelectionSort implements Sortable {

    public void sort(int[] arr) {
        int n = arr.length;

        for (int i = 0; i < n - 1; i++) {

            int minIndex = i;

            for (int j = i + 1; j < n; j++) {
                if (arr[j] < arr[minIndex]) {
                    minIndex = j;
                }
            }

            // swap
            int temp = arr[minIndex];
            arr[minIndex] = arr[i];
            arr[i] = temp;
        }
    }
}

```

### source code of Main Class of TestSort java :

```

public class TestSort {

    public static void main(String[] args) {

        int[] arr1 = {5, 2, 9, 1, 3};

        Sortable ref;

        ref = new BubbleSort();
        ref.sort(arr1);

        System.out.println("Array sorted using BubbleSort:");
        display(arr1);

        int[] arr2 = {8, 4, 7, 6, 2};

        ref = new SelectionSort();
        ref.sort(arr2);

        System.out.println("Array sorted using SelectionSort:");
        display(arr2);
    }

    static void display(int[] arr) {
        for (int num : arr) {
            System.out.print(num + " ");
        }
        System.out.println();
    }
}

```

# OUTPUT :
<img width="1366" height="768" alt="EXP5A" src="https://github.com/user-attachments/assets/e4c22f16-81ab-449d-b5ad-633498d81831" />



# EXPERIMENT 5B

## TITLE : Implement the Runtime Polymorphism.

## SOURCE CODE :

---

### source code of the Vehicle :

```

class vehicle {

    void run() {
        System.out.println("vehicle is running");
    }
}

```

### source code of the Car java:

```

class car extends vehicle {

    @Override
    void run() {
        System.out.println("car is running on four wheels");
    }
}

```

###  source code of the Bike java:


```

class bike extends vehicle {

    @Override
    void run() {
        System.out.println("bike is running on two wheels");
    }
}

```

### source code of  the Testehicle :

```

public class testvehicle {

    public static void main(String[] args) {

        vehicle v;   // base class reference

        v = new car();
        v.run();     // calls car's run()

        v = new bike();
        v.run();     // calls bike's run()

        v = new vehicle();
        v.run();     // calls vehicle's run()
    }
}

```

# OUTPUT :
<img width="1366" height="768" alt="EXP5B" src="https://github.com/user-attachments/assets/b9e5242b-28e2-46a2-9ecf-ac3347690f4d" />


# EXPERIMENT 5C

## TITLE : String Buffer Delete Demo.

## SOURCE CODE: 

```

public class StringBufferDeleteDemo {

    public static void main(String[] args) {

        // Create StringBuffer object
        StringBuffer sb = new StringBuffer("Java Programming");

        // Display original string
        System.out.println("Original String: " + sb);

        // Delete a single character at index 4
        sb.deleteCharAt(4);
        System.out.println("After deleting character at index 4: " + sb);

        // Delete a range of characters from index 0 to 4
        sb.delete(0, 4);
        System.out.println("After deleting characters from index 0 to 4: " + sb);
    }
}

```

# OUTPUT :
<img width="1366" height="768" alt="EXP5C" src="https://github.com/user-attachments/assets/cf9f5c03-40ca-4e00-a64b-a534a102f8e6" />

