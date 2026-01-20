## Experiment 3

## Experiment 3A

### TITLE:
Implement constructor overloading in JAVA.

---

### SOURCE CODE
Student.java

```java

class Student {

	String name;
	int age;
	double marks;

	Student() {

	}

	Student(String name, int age, double marks) {

		this.name=name;
		this.age=age;
		this.marks=marks;

	}

	void display() {

		System.out.println("Name: "+name);
		System.out.println("Age: "+age);
		System.out.println("marks: "+marks);

	}

}

```

## Main.java

```

 class Main {

	public static void main(String args[]) {

		Student std = new Student();
		std.display();

		Student std1 = new Student("Hari", 40, 67.8);
		std1.display();

	}
}

```

## output
<img width="1366" height="768" alt="3A" src="https://github.com/user-attachments/assets/3db80b65-9b2d-4381-99b6-e37b3d97fd6b" />






## Experiment 3C

## TITLE:
Sorting Element using Bubble sort

---

## SOURCE CODE:
Bubble sort

```java

class BubbleSort {

	void bubbleSort(int arr[]) {

		int n = arr.length;
		int temp = 0;

		for(int i=0 ; i < n-1 ; i++) {

			for(int j=0; j<n-i-1; j++) {

				if(arr[j] > arr[j+1]) {

					temp = arr[j+1];
					arr[j+1] = arr[j];
					arr[j] = temp;

				}
			}
		}

	}

}

```

## Main.java

```

import java.util.Scanner;
 class Main {
	
	public static void main(String args[]) {


		System.out.print("Enter the size of array: ");
		Scanner sc = new Scanner(System.in);
		int size = sc.nextInt();

		int integer[] = new int[size];

		for(int i = 0; i < size; i++) {

			System.out.print("Enter the value of integer at index " + (i+1) + ":"); 
			integer[i] = sc.nextInt();
		}

		BubbleSort bs = new BubbleSort();
		bs.bubbleSort(integer);


		System.out.print("The Sorted integer: ");

		for(int i = 0; i < size; i++)
		System.out.print(integer[i] + ", ");

		System.out.println("\b\b.");

	}

}

```

## output
<img width="1366" height="768" alt="3c" src="https://github.com/user-attachments/assets/759461d9-dccd-409c-9aff-122abfba3c42" />
