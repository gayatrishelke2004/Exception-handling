#include <iostream>
using namespace std;
class Exp_handling {
private:
    int age, vehicle;
    long double income;
    string city;
public:
    void getdata() {
        cout << "\nEnter the age: ";
        cin >> age;
        cout << "\nEnter total no. of vehicle wheels: ";
        cin >> vehicle;
        cout << "\nEnter the income: ";
        cin >> income;
        cout << "\nEnter the city: ";
        cin >> city;
    }
    void check() {
        
    }
 friend void display(const Exp_handling&); // Declaration of friend function
};
void display(const Exp_handling& obj) {
    cout << "\nAge: " << obj.age;
    cout << "\nVehicle wheels: " << obj.vehicle;
    cout << "\nIncome: " << obj.income;
    cout << "\nCity: " << obj.city;
}

int main() {
    Exp_handling a;
    a.getdata();
    a.check();
    display(a);
   return 0;
}# Exception-handling
