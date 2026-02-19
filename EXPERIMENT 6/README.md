# EXPERIMENT 6

## EXPERIMENT 6A

### TITLE: Expection handling mechanism.

#### SOURCE CODE:

```

import java.util.Scanner;

public class Solution {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        // Read size of array
        System.out.print("Enter size of array: ");
        int n = sc.nextInt();

        // Create array
        int[] arr = new int[n];

        // Read array elements
        System.out.println("Enter " + n + " elements:");
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        // Ask user for index
        System.out.print("Enter index to access: ");
        int index = sc.nextInt();

        // Exception handling
        try {
            System.out.println("Element at index " + index + " is: " + arr[index]);
        } 
        catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("Invalid index! Please enter index between 0 and " + (n - 1));
        }

        sc.close();
    }
}

```

## OUTPUT
<img width="1366" height="768" alt="EXP6A" src="https://github.com/user-attachments/assets/72ac180c-b359-431b-94ff-8fa5a3f4f200" />



## EXPERIMENT 6B

### TITLE: Multiple catch clauses

#### SOURCE CODE:

```

import java.util.Scanner;
import java.util.InputMismatchException;

public class MultipleCatchExample {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        // Creating an integer array
        int arr[] = {10, 20, 30, 40, 50};

        try {
            // Taking two numbers from user
            System.out.print("Enter first number: ");
            int a = sc.nextInt();

            System.out.print("Enter second number: ");
            int b = sc.nextInt();

            // Division operation
            int result = a / b;
            System.out.println("Result of division: " + result);

            // Accessing array element
            System.out.print("Enter index to access array element: ");
            int index = sc.nextInt();

            System.out.println("Element at index " + index + " = " + arr[index]);
        }

        catch (ArithmeticException e) {
            System.out.println("Error: Division by zero is not allowed.");
        }

        catch (InputMismatchException e) {
            System.out.println("Error: Please enter numeric values only.");
        }

        catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("Error: Invalid array index.");
        }

        catch (Exception e) {
            System.out.println("Some other error occurred.");
        }

        finally {
            System.out.println("Program continues...");
            sc.close();
        }
    }
}

```

## OUTPUT
<img width="1366" height="768" alt="EXP6B" src="https://github.com/user-attachments/assets/02db40c3-4e45-450a-b6e0-2d70f96e4e1c" />




## EXPERIMENT 6C

### TITLE: Creation of java Bulit-in-Expection.

#### SOURCE CODE:

```

import java.util.Scanner;

public class Solution {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        try {
            // ArithmeticException (Divide by zero)
            System.out.print("Enter an integer to divide 100: ");
            int n = sc.nextInt();
            int result = 100 / n;
            System.out.println("Result: " + result);

            // ArrayIndexOutOfBoundsException
            int[] arr = new int[3];
            System.out.println("Accessing element at index 5:");
            System.out.println(arr[5]);

            // NumberFormatException
            System.out.print("Enter a number as text: ");
            String s = sc.next();
            int num = Integer.parseInt(s);
            System.out.println("Converted number: " + num);
        }

        catch (ArithmeticException e) {
            System.out.println("ArithmeticException: Division by zero.");
        }

        catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("ArrayIndexOutOfBoundsException: Invalid index.");
        }

        catch (NumberFormatException e) {
            System.out.println("NumberFormatException: Invalid numeric format.");
        }

        catch (Exception e) {   // Optional general exception
            System.out.println("Some other exception occurred.");
        }

        System.out.println("Program continues...");
        sc.close();
    }
}

```

## OUTPUT
<img width="1366" height="768" alt="EXP6C" src="https://github.com/user-attachments/assets/2e3dd931-3518-48e8-8ea4-1a990ebf661a" />
