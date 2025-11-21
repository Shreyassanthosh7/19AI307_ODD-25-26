# Ex.No:3(D)    INTERFACE 

## QUESTION:
You are programming bots that analyze weather data. Each bot must implement a common interface and give a prediction.
-  Bot Types:
- SunBot: Predicts "HOT" if temperature > 30, else "MODERATE".
- RainBot: Predicts "COLD" if temperature < 20, else "WARM".
- Input:
   temperature
- botType (1 for SunBot, 2 for RainBot)Output:
- Prediction as a string.
- For example:

| Input        | Result   |
|--------------|----------|
| 35 1  | HOT  |

## AIM:
To write a Java program that demonstrates polymorphism using interfaces, where different weather prediction behaviors are implemented by SunBot and ColdBot based on temperature input.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read the temperature and bot type (1 for SunBot, else ColdBot) from the user.
5. Declare a reference variable of the WeatherBot interface.
6. Based on the input, create an object of either SunBot or ColdBot and assign it to the interface reference.
7. Call the Predict() method using the interface reference to get the weather prediction.
8. Display the weather prediction to the user.

## PROGRAM:
```txt
Program to implement a Interface using Java
Developed by: Sudharsanam R K
RegisterNumber:212222040163
```

## SOURCE CODE:
```java
import java.util.*;
interface WeatherBot {
    String Predict(int temp);
}

class SunBot implements WeatherBot {
    public String Predict(int temp) {
        if(temp>30)
        return "HOT";
        else
        return "MODERATE";
    }
}

class ColdBot implements WeatherBot {
    public String Predict(int temp) {
        if(temp<20)
        return "COLD";
        else
        return "WARM";
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner input=new Scanner(System.in);
        int temp=input.nextInt();
        int type=input.nextInt();
        WeatherBot weather;
        if(type==1)
        weather=new SunBot();
        else
        weather=new ColdBot();
        
        System.out.print(weather.Predict(temp));
    }
}
```

## OUTPUT:
<img width="401" height="186" alt="image" src="https://github.com/user-attachments/assets/0cdf1d67-b2e0-4e32-ab8e-cae04f591eed" />


## RESULT:
The program successfully demonstrates interface-based polymorphism. Depending on the selected bot type, the appropriate implementation of the Predict() method is invoked, and the weather condition is displayed based on the given temperature.

