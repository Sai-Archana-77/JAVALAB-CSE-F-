## Additional Experiments

## Experiment 2

## TITLE:
2.)Display the Fibonacciseries

---

## SOURCE CODE:
Fibonacciseries

```java

import java.util.Scanner;
class Fibonacciseries{
int sum;
int n;
int FirstNumber;
int SecondNumber;
int ThirdNumber;
Fibonacciseries(int number){
n=number;
FirstNumber=0;
SecondNumber=1;
ThirdNumber=0;
sum=0;
}
void generate(){
if(n>0)
System.out.print("Fibonacci series:");
while(n>0){
if(n==1){
System.out.print(FirstNumber+".");
sum=sum+FirstNumber;
}else{
System.out.print(FirstNumber+",");
sum=sum+FirstNumber;
}
ThirdNumber = FirstNumber+SecondNumber;
FirstNumber=SecondNumber;
SecondNumber=ThirdNumber;
n--;
}
System.out.println("sum of Fibonacci series="+sum);
}
public static void main(String[] args){
Scanner sc = new Scanner(System.in);
System.out.println("Enter the value of n:");
int number = sc.nextInt();
Fibonacciseries f = new Fibonacciseries(number);
f.generate();
}
}

```

## output
<img width="1366" height="768" alt="AddExp2" src="https://github.com/user-attachments/assets/4e7358a2-9d5e-4def-9aa6-8642b9e56bb3" />

