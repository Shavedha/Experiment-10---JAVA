# Experiment-10---JAVA
## AIM
To create a Java program to print the below
```
Create a class named 'Member' having the following members:
Data members:
1 - Name
2 - Age
3 - Phone number
4 - Address
5 - Salary

It also has a method named 'printSalary' which prints the salary of the members.
Two classes 'Employee' and 'Manager' inherits the 'Member' class. The 'Employee' and 
'Manager' classes have data members 'specialization' and 'department' respectively. 
Now, assign name, age, phone number, address and salary to an employee and
a manager by making an object of both of these classes and print the same.
```
## ALGORITHM
1. Create a member class to print the name,age,phone number,Address and salary.
2. Create a employee class to print the specialization.
3. Create a manager class to print the department.
4. In the main class add the values for both employee and Manager and print the same.
5. End the program.
## PROGRAM
### Member.java
```
public class Member {
    String name,phonenum,Address;

    public void name(String name){
        System.out.println("Name: "+name);
    }
    public void age(int age){
        System.out.println("Age: "+age);
    }
    public void phonenum(String phonenum){

        System.out.println("Phone Number: "+phonenum);
    }
    public void add(String address){

        System.out.println("Address: "+address);
    }
    public void printSalary(int salary){

        System.out.println("Salary: "+salary);
    }
}

```
### Main.java
```
public class Main{
    public static void main(String[] args){
        Employee emp1=new Employee();
        System.out.println("EMPLOYEE");
        emp1.name("Morgan");
        emp1.age(26);
        emp1.phonenum("6758490675");
        emp1.add("76th WallsStreet");
        emp1.printSalary(756000);
        emp1.spec("Analyst");

        Manager mg1=new Manager();
        System.out.println("MANAGER");
        mg1.name("Chloe");
        mg1.age(34);
        mg1.phonenum("6453789067");
        mg1.add("64th Ravenclaw");
        mg1.printSalary(956700);
        mg1.Deps("Research and Development");


    }
}
```
### Employee.java
```
public class Employee extends Member {
    String specialization;
    void spec(String specialization){

        System.out.println("Specilization :  "+specialization);
    }
}

```
### Manager.java
```
public class Manager extends Member {
    String Departmentt;
    void Deps(String Department){

        System.out.println("Department: "+Department);
    }
}

```
## OUTPUT
<img width="482" alt="image" src="https://github.com/Shavedha/Experiment-10---JAVA/assets/93427376/afc3e20c-706b-4d41-84df-cbd862d79bc9">

## RESULT
Thus a Java program is created to implement the above code.
