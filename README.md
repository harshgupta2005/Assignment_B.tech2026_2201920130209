# Assignment_B.tech2026_2201920130209
This is GLBITM CDC26 assignment repository

**Problem1 26-01-2025**
Problem Statement:
Define a class Rectangle with attributes length and width. Implement methods to calculate the area and perimeter of the rectangle. Also, include a method to display the rectangle's dimensions.
```
   #include <iostream>
using namespace std;

class Rectangle {
private:
    double length;
    double width;

public:
    
    Rectangle(double l, double w) {
        length = l;
        width = w;
    }
    double calculateArea() {
        return length * width;
    }
    double calculatePerimeter() {
        return 2 * (length + width);
    }
    void displayDimensions() {
        cout << "Length: " << length << ", Width: " << width << endl;
    }
};
int main() {
    Rectangle rect(10.5, 5.2);
    rect.displayDimensions();
    cout << "Area: " << rect.calculateArea() << endl;
    cout << "Perimeter: " << rect.calculatePerimeter() << endl;
    return 0;
}
  ```
**Problem2 27-01-2025**
Problem Statement:Create a class BankAccount with attributes accountNumber, accountHolderName, and balance. Implement methods to deposit an amount, withdraw an amount (with sufficient balance check), and display the account details.
```#include <iostream>
using namespace std;

class BankAccount {
private:
    int accountNumber;
    string accountHolderName;
    double balance;

public:
    BankAccount(int accNum, string accHolder, double bal) {
        accountNumber = accNum;
        accountHolderName = accHolder;
        balance = bal;
    }

    void deposit(double amount) {
        balance += amount;
    }

    bool withdraw(double amount) {
        if (amount > balance) {
            cout << "Insufficient balance" << endl;
            return false;
        }
        balance -= amount;
        return true;
    }

    void displayAccountDetails() {
        cout << "Account Number: " << accountNumber << endl;
        cout << "Account Holder: " << accountHolderName << endl;
        cout << "Balance: " << balance << endl;
    }
};

int main() {
    BankAccount account(12345, "John Doe", 5000.0);
    account.deposit(1500.0);
    account.withdraw(2000.0);
    account.displayAccountDetails();
    return 0;
}
```
