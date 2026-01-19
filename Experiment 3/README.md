## Experiment 3

## Experiment 3a

### TITLE:
Implement constructor overloading in JAVA.

---

### Source code:
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

Main java

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

#output
<img width="1366" height="768" alt="3A" src="https://github.com/user-attachments/assets/3db80b65-9b2d-4381-99b6-e37b3d97fd6b" />





## Experiment 3b

## Title: 
Implementing Binary Search Algorithm

---

## source code:
BinarySearch.java

```java
import java.util.Scanner;
class BinarySearch {

	int list[];
	int key;
	int size;

	BinarySearch(int size) {

		list= new int[size];
		key = -1;
		this.size=size;

 	}
 
 	void setList() {

			Scanner sc = new Scanner(System.in);
			System.out.println("Enter the list items in Ascending Order.");


			for( int i = 0; i < size; i++) {
	
				System.out.print("Enter the value of " + (i + 1) + " item: ");
				list[i] = sc.nextInt();
			}
			sc.close();

	}

	void getList() {

		for(int i = 0; i < size; i++) 
		System.out.print(list[i] + ", "); System.out.println("\b\b.");

	}

	int binarySearch(int key) {

		int low = 0; int high = list.length; int mid = 0;

		while(low < high) {

			mid = (low + high) / 2;

			if(list[mid] == key) {
				break;
			}

			else if(list[mid] < key) {

				low = mid + 1;
			}

			else
				high = mid + 1;

		}

		return list[mid]==key ? mid : -1 ;

	}

}

```

## Main.java

import java.util.Scanner;
class Main {

	public static void main(String args[]) {

		
		BinarySearch bs = new BinarySearch(10);
		bs.setList();
		bs.getList();


	int index = bs.binarySearch(10);		
	if(index == -1 )
			System.out.println("Key item does not exit");

		else
			System.out.println("key item exist at index: " + index);

	}

}

```

## output
<img width="1366" height="768" alt="3B" src="https://github.com/user-attachments/assets/5586203c-29ec-441b-b478-91d89a2442f4" />



