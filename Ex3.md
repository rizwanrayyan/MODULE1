# Ex.No:3
# Ex.Name: Write a C++ program to convert Celsius into Fahrenheit using inline function  
## Date: 07/08/2025
## Aim:
To write a C++ program that converts a temperature from Celsius to Fahrenheit using an inline function.

## Algorithm:
1. Start the program.
2. Define an inline function celsiusToFahrenheit(float c) that takes Celsius as input and returns Fahrenheit using the formula:
𝐹=(𝐶×95)+32
3. In the main() function, take Celsius temperature as input from the user.
4. Call the inline function to convert Celsius into Fahrenheit.
5. Display the result.
6. End the program.

## Program:
```cpp
#include <iostream>
inline double celsiusToFahrenheit(double celsius) {
    return (celsius * 9.0 / 5.0) + 32.0;
}

int main() {
    double celsius;
    std::cin >> celsius;
    double fahrenheit = celsiusToFahrenheit(celsius);
    std::cout << "temperature in Fahrenheit:" << fahrenheit << std::endl;

    return 0;
}
```


## Output:
<img width="760" height="221" alt="image" src="https://github.com/user-attachments/assets/75013410-2ca9-4b77-a6ba-583441efd8f1" />



## Result
The program successfully converts Celsius into Fahrenheit using an inline function in C++.
