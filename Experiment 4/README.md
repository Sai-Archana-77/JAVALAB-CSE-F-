## Experiment 4

## Experiment 4A

## TITLE: Implement Single Inheritance.

## SOURCE CODE:

---

## Person:

```

class Person {
    String name;
    int age;

    Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    void displayPersonDetails() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
    }
}

```

## Employee:

```

class Employee extends Person {

    double annualSalary;
    int yearOfJoining;
    String nationalInsuranceNumber;

    Employee(String name, int age, double annualSalary, int yearOfJoining,
             String nationalInsuranceNumber) {

        super(name, age);
        this.annualSalary = annualSalary;
        this.yearOfJoining = yearOfJoining;
        this.nationalInsuranceNumber = nationalInsuranceNumber;
    }

    void displayEmployeeDetails() {
        displayPersonDetails();
        System.out.println("Annual Salary: " + annualSalary);
        System.out.println("Year of Joining: " + yearOfJoining);
        System.out.println("National Insurance Number: " + nationalInsuranceNumber);
    }
}

```

## TestEmployee:

```

class TestEmployee {
    public static void main(String args[]) {

        Employee emp1 = new Employee(
                "Narasimhulu",
                45,
                60000.95,
                2011,
                "2003-2004-2005-2006"
        );

        emp1.displayEmployeeDetails();
    }
}

```


## OUTPUT
<img width="1366" height="768" alt="Exp4a" src="https://github.com/user-attachments/assets/a3940a2d-3da6-4d27-8e97-1d90b769f279" />


## Experiment 4B

## TITLE: Implement multi-level inheritance.

##  SOURCE CODE:

---

## Bicycle:

```

class Bicycle {
    String pedalType;

    void showBicycleInfo() {
        System.out.println("Pedal Type: " + pedalType);
    }
}

```

## Motor Bikes:

```

class Motorbike extends Bicycle {
    int engineCapacity;

    void showMotorbikeInfo() {
        System.out.println("Engine Capacity: " + engineCapacity + " cc");
    }
}

```

## Eletric Bikes: 

```

class ElectricBike extends Motorbike {
    int batteryCapacity;

    void showElectricBikeInfo() {
        System.out.println("Battery Capacity: " + batteryCapacity + " W>
    }
}

```

## Test Vehicles:

```

public class TestVehicle {
    public static void main(String[] args) {

        ElectricBike eBike = new ElectricBike();

        eBike.pedalType = "Manual Pedals";
        eBike.engineCapacity = 250;
        eBike.batteryCapacity = 500;

        eBike.showBicycleInfo();
        eBike.showMotorbikeInfo();
        eBike.showElectricBikeInfo();
    }
}

```

## OUTPUT
<img width="1366" height="768" alt="Exp4b" src="https://github.com/user-attachments/assets/f6afb5a6-bbe1-484e-8554-db40a175e1ff" />


## Experiment 4C

## TITLE: Implement areas different shapes.

## SOURCE CODE:

---

## Figure:

```

abstract class Figure {
    double dim1;
    double dim2;

    Figure(double dim1, double dim2) {
        this.dim1 = dim1;
        this.dim2 = dim2;
    }

    abstract double area();
}

```

## Rectangle:

```

class Rectangle extends Figure {

    Rectangle(double length, double breadth) {
        super(length, breadth);
    }

    double area() {
        return dim1 * dim2;
    }
}

```

## Triangle:

```

class Triangle extends Figure {

    Triangle(double base, double height) {
        super(base, height);
    }

    double area() {
        return 0.5 * dim1 * dim2;
    }
}

```

## Test Figure:

```

public class TestFigure {
    public static void main(String[] args) {

        Figure f1 = new Rectangle(10, 5);
        System.out.println("Area of Rectangle = " + f1.area());

        Figure f2 = new Triangle(6, 4);
        System.out.println("Area of Triangle = " + f2.area());
    }
}

```

## OUTPUT
<img width="1366" height="768" alt="Exp4c" src="https://github.com/user-attachments/assets/8d71b12b-b11f-497f-88dc-f0922d0f8b79" />



