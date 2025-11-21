# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:
Write a Java program to create a class called Smartphone with private instance variables brand, model, and storageCapacity. Provide public getter and setter methods to access and modify these variables. Add a method called increaseStorage() that takes an integer value and increases the storageCapacity by that value.

## AIM:
To implement access specifiers in Java using private variables and public getter and setter methods.


## ALGORITHM :
1. Start the program.
2. Import the necessary package java.util.
3. Create a class Smartphone with private variables.
4. Create public getter and setter methods to access private data members.
5. Create a method increaseStorage(int value) to increase storage.
6. In the main method, get user input.
7. Create an object of Smartphone and call the methods.
8. Display updated details.
9. End the program.
    
## PROGRAM:
 ```
Program to implement a Access Specifiers using Java
Developed by: Sudharsanam R K
RegisterNumber: 212222040163
```

## SOURCE CODE:
```java
import java.util.Scanner;

class prog {
    private String brand;
    private String model;
    private int storageCapacity;
 
    public String getBrand() {
        return brand;
    }

    public String getModel() {
        return model;
    }

    public int getStorageCapacity() {
        return storageCapacity;
    }

    public void setBrand(String brand) {
        this.brand = brand;
    }

    public void setModel(String model) {
        this.model = model;
    }

    public void setStorageCapacity(int storageCapacity) {
        this.storageCapacity = storageCapacity;
    }

    public void increaseStorage(int value) {
        if (value > 0) {
            this.storageCapacity += value;
        }
    }
    
    public void display() {
        System.out.println("Brand: " + brand);
        System.out.println("Model: " + model);
        System.out.println("Updated Storage Capacity: " + storageCapacity + " GB");
        System.out.println("------------------------------");
    }

    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        String brand=sc.nextLine();
        String Model=sc.nextLine();
        int storageCapacity=sc.nextInt();
        int increaseValue=sc.nextInt();
        prog obj=new prog();
        obj.setBrand(brand);
        obj.setModel(Model);
        obj.setStorageCapacity(storageCapacity);
        obj.getBrand();
        obj.getModel();
        obj.getStorageCapacity();
        obj.increaseStorage(increaseValue);
        obj.display();
    }
}
```

## OUTPUT:
<img width="923" height="441" alt="image" src="https://github.com/user-attachments/assets/f8826765-e461-4b4a-9c00-732059268d21" />

## RESULT:
The program successfully implemented access specifiers using private instance variables and public getter and setter methods in Java.
