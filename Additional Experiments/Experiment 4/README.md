## Experiment 4

## TITLE: Implementing the Perfect Number using java

---

## Source Code:

```

import java.util.Scanner;

class perfectnumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int num = sc.nextInt();

        int sum = 0;

        for (int i = 1; i < num; i++) {
            if (num % i == 0) {
                sum += i;
            }
        }

        if (sum == num)
            System.out.println(num + "num is a perfect number.");
        else
            System.out.println(num + "num is not a perfect number.");
    }
}

```

## OUTPUT:
<img width="1366" height="768" alt="AddExp4" src="https://github.com/user-attachments/assets/42630714-f6a0-4536-8f11-4aa0c139781d" />
