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

	}

}
