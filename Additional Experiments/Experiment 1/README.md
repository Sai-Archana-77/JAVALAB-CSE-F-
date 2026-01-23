## Experiment 1

## TITLE: Implementing the substring

---

## Source Code

```

import java.util.Scanner;

class substring {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter the main string: ");
        String mainString = sc.nextLine();

        System.out.print("Enter the substring to insert: ");
        String subString = sc.nextLine();

        System.out.print("Enter the position: ");
        int position = sc.nextInt();

        if (position >= 0 && position <= mainString.length()) {
            String firstPart = mainString.substring(0, position);
            String secondPart = mainString.substring(position);

            String resultString = firstPart + subString + secondPart;
            System.out.println("Resulting string: " + resultString);
        } else {
            System.out.println("Invalid position");
        }
    }
}

```

## OUTPUT
<img width="1366" height="768" alt="AddExp1" src="https://github.com/user-attachments/assets/a519eaf7-7863-4607-8f0c-2c93afd65046" />


