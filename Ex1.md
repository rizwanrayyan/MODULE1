# Ex.No:1
# Ex.Name: Write a C++ program to find the sum of GP series using friend function. formula:  Sn = a(rn - 1) / (r - 1)
## Date: 07/08/2025
## Aim:To write a C++ program that calculates the sum of a Geometric Progression (GP) series using a friend function, based on the formula

### Algorithm:
```
1. Start the program.
2. Input the first term (a), common ratio (r), and number of terms (n).
3. Define a class GP with private data members: a, r, and n.
4. Initialize the values using a constructor.
5. Declare a friend function sumGP(GP g) inside the class.
6. In the friend function:
If 
𝑟=1
r=1, compute:

𝑆=𝑎×𝑛
Otherwise, compute using:
 Sn = a(rn - 1) / (r - 1)
7. Return the computed sum.
8. In main(), create an object of GP and call the friend function.
9. Display the result.
10. End the program.
```
## Program:
```cpp
#include <iostream>
#include <cmath>
using namespace std;

class GPSeries {
private:
    float a, r;
    int n;

public:
    void getInput();
    friend float findSum(GPSeries obj);  
};

void GPSeries::getInput() {
    cin >> a >> r >> n;
}
float findSum(GPSeries obj) {
    float sum;
    if (obj.r == 1) {
        sum = obj.a * obj.n; 
    } else {
        sum = obj.a * (pow(obj.r, obj.n) - 1) / (obj.r - 1);
    }
    return sum;
}

int main() {
    GPSeries gp;
    gp.getInput();

    float sum = findSum(gp);  
    cout << "The sum of GP series is " << sum << endl;

    return 0;
}
```
## Output:
<img width="571" height="256" alt="image" src="https://github.com/user-attachments/assets/439d6b4c-0ccd-428a-ba77-3a75f907a2b1" />

## Result:
The C++ program was successfully executed.

