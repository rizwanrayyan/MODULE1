# Ex.No2
# Ex.Name: Write a C++ Program to generate Fibonacci series using Class?
## Date: 07/08/2025

## Aim:
To write a C++ program that generates the Fibonacci series using a class.

## Algorithm:
1. Start the program.
2. Define a class Fibonacci with data members for the first two terms of the series.
3. Create a method generateSeries(int n) to generate and display the Fibonacci series up to n terms.
4. In the main function, take the number of terms as input from the user.
5. Create an object of the Fibonacci class and call the method to generate the series.
6. Display the output.
7. End the program.


## Program:
```cpp
#include<iostream>
using namespace std;
int main()
{
    int x,c;
    int a=0,b=1;
    cin>>x;
    cout<<"Fibonacci Series are:"<<a<<" "<<b<<" ";
    for(int i=0;i<x-2;i++)
    {
        c=a+b;
        a=b;
        b=c;
        cout<<c<<" ";
    }
}
```
## Output:
<img width="1418" height="227" alt="image" src="https://github.com/user-attachments/assets/ca514421-83ef-4cff-aed0-7f8dafbeb0ed" />



## Result:
The program successfully generates the Fibonacci series using a class in C++.
