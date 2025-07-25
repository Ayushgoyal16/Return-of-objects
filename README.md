# Return-of-objects
#include <iostream>
using namespace std;

class sample
 {
    int x;
public:
    void getdata(int a) 
    {
        x = a;
    }

    void display() 
    {
        cout << "x = " << x << endl;
    }

    sample sum(sample b)
     {
        sample c;
        c.x = x + b.x;
        return c;
    }
};

int main() 
{
    sample obj1, obj2, obj3;

    int a, b;
    cout << "Enter first number: ";
    cin >> a;
    cout << "Enter second number: ";
    cin >> b;

    obj1.getdata(a);
    obj2.getdata(b);

    obj3 = obj1.sum(obj2);

    cout << "Sum is: ";
    obj3.display();

    return 0;
}





