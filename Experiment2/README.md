#Experiment 2
##TITLE: 2a.)Display the student
```
class student {
int id;
String name;
void setData(int i,String n){
id = i;
name = n;
}
void display(){
System.out.println("student ID:"+id);
System.out.println("student Name:"+name);
}
public static void main(String[] args){
student s1 = new student();
s1.setData(101,"sai");
s1.display();
}
}

```
>#output

<img width="1366" height="768" alt="Exp2a" src="https://github.com/user-attachments/assets/eb4044d5-a306-46d4-a132-87120e416382" />

##TITLE: 2b.)Display the methodoverloading
```
class Methodoverloading {
int add(int a, int b){
return a+b;
}
int add(int a,int b,int c){
return a+b+c;
}
double add(double a, double b){
return a+b;
}
public static void main(String[] args){
Methodoverloading obj = new Methodoverloading();
System.out.println("Addition of two integers: " + obj.add(10, 20));
System.out.println("Addition of three integers: " + obj.add(5, 10, 15));
System.out.println("Addtion of doubles: " + obj.add(2.5, 3.5));
}
}

```
>#output

<img width="1366" height="768" alt="Exp2b" src="https://github.com/user-attachments/assets/aea2ed91-ab64-4210-a059-43bab440c855" />
