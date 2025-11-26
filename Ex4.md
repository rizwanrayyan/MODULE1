# Ex.No:4
# Ex.Name: Write a program in C++ to compute quotient and remainder using class methods(define methods outside class)
## Date: 07/08/2025
## Aim:
To write a C++ program to compute the quotient and remainder using class methods defined outside the class.

## Algorithm:
1. Start the program.
2. Define a class Division with two member functions:
  -computeQuotient(int a, int b)
  -computeRemainder(int a, int b)
3. Declare these functions inside the class but define them outside using scope resolution ::.
4. In the main() function, read two integers from the user (dividend and divisor).
5. Call the methods using the class object to compute quotient and remainder.
6. Display the results.
7. End the program.

## Program:
```cpp
#include <iostream>
using namespace std;
class view{
    public:
    void remain(int a,int b);
};
void view::remain(int a,int b)
{
    cout<<"The quotient of the division is:"<<a/b<<endl;
    cout<<"The remainder of the division is:"<<a%b;
}
int main()
{
    int a,b;
    cin>>a>>b;
    view v;
    v.remain(a,b);
}
```


## Output:
<img width="621" height="252" alt="image" src="https://github.com/user-attachments/assets/698ab1a7-a886-4110-942b-1ed200160b84" />


## Result:
The program successfully computes the quotient and remainder using class methods defined outside the class in C++.
