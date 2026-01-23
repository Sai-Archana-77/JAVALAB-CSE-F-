## Experiment 3

## TITLE: Implementing the palindrome using java

---

## Source Code:

```

import java.util.Scanner;

class palindrome {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a String:");
        String str= sc.nextLine();
        int start = 0;
        int end = str.length() - 1;
        while (start < end) {
            if (str.charAt(start) != str.charAt(end)) {
                System.out.println(str+" is not a palindrome");
                return;
            }

            start++;
            end--;
        }
        System.out.println(str+" is a palindrome");
    }
}

```

## OUTPUT:
<img width="1366" height="768" alt="AddExp3" src="https://github.com/user-attachments/assets/23de4afe-e565-4536-978a-5a5024fe19a1" />
