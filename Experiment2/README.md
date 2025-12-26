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
