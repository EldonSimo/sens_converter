#include <iostream>
#include <conio.h>
using namespace std;

int main() {
    cout << "\n==================================== Sens Converter Based on Feeling ====================================\n";
    
    double num1;
    cout << "Enter your CSGO sens: ";
    cin >> num1;
    
    double num2;
    cout << "Enter your DPI (400, 800, 1200): ";
    cin >> num2;
    
    if (num2 == 400) {
        double newValue = num1 - 0.002;
        cout << "Your sens in CS2: " << newValue << endl;
    } 
    else if (num2 == 800) {
        double newValue = num1 - 0.0002;
        cout << "Your sens in CS2: " << newValue << endl;
    } 
    else if (num2 == 1200) {
        double newValue = num1 - 0.00002;
        cout << "Your sens in CS2: " << newValue << endl;
    } 
    else {
        cout << "Invalid DPI" << endl;
    }


    char enterKey = '\n';
    cout << "Press any key to exit..." << endl;
    _getch();
    
    return 0;
}
