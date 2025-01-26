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
