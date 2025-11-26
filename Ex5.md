# Ex.No:5
# Ex.Name: Write a C++ program to find the minimum of two and three numbers using construction overloading, pass values during compile time.
## Date: 07/08/2025
## Aim:
To write a C++ program that finds the minimum of two and three numbers using constructor overloading, where values are passed during compile time.


## Algorithm:
1. Start the program.
2. Define a class Minimum with overloaded constructors:
  -One constructor to find the minimum of two numbers.
  -Another constructor to find the minimum of three numbers.
3. In each constructor, compute and display the minimum value.
4. In main(), create objects of the class with values passed directly during object creation (compile time).
5. Display the results.
6. End the program.

## Program:
```cpp
#include<iostream>
using namespace std;
class sam
{
    public:
    sam(int a,int b)
    {
        if(a<b)
        cout<<a<<" is lesser\n";
        else
        cout<<b<<" is lesser\n";
    }
    sam(int a,int b,int c)
    {
        if(a<b)
        {
            if (a<c)
            cout<<a<<" is lesser\n";
        }
        if(b<c)
        cout<<b<<" is lesser\n";
        else
        cout<<c<<" is lesser";
    }
};
int main()
{
    sam s(95,64);
    sam s1(22,28,21);
}
```

## Output:
<img width="370" height="180" alt="image" src="https://github.com/user-attachments/assets/af1e9a78-60f1-4dca-8bcf-3c515919e614" />

## Result:
The program successfully finds the minimum of two and three numbers using constructor overloading, with values passed at compile time.
