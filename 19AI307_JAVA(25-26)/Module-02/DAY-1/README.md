# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
Create a class Car with attributes brand, model, year. Create 2 objects and print their details.

## AIM:
To write a Java program to implement Classes and Objects using a Car class and display details of two car objects.

## ALGORITHM :
1. Start the program.
2. Import the necessary package java.util (if required).
3. Create a class named Car.
4. Declare data members: brand, model, year.
5. Create a parameterized constructor to initialize values.
6. In the main function, create two objects of class Car.
7. Print the details of both objects.
8. End the program.

## PROGRAM:
```txt
Program to implement a Class and Objects using Java
Developed by: Shreyas S
RegisterNumber: 212222040155
```

## SOURCE CODE:
```java
class Car{
    String brand;
    String model;
    int year;
}
public class prog {
    public static void main(String[] args) {
        Car car1 = new Car();
        car1.brand = "Toyota";
        car1.model = "Innova";
        car1.year = 2022;

        Car car2 = new Car();
        car2.brand = "Hyundai";
        car2.model = "i20";
        car2.year = 2021;

        System.out.println("Car 1: " + car1.brand + " " + car1.model + " " + car1.year);
        System.out.println("Car 2: " + car2.brand + " " + car2.model + " " + car2.year);
    }
}
```

## OUTPUT:
<img width="575" height="170" alt="image" src="https://github.com/user-attachments/assets/550c3dcd-4916-43bd-b806-a691318c2a2e" />

## RESULT:
The program to implement a class and objects using Java was successfully executed and the details of two car objects were displayed.

