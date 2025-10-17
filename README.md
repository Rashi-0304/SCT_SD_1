#include <iostream>
using namespace std;

int main() {
    double temp, converted;
    int choice;

    cout << "Temperature Conversion Program" << endl;
    cout << "1. Celsius to Fahrenheit" << endl;
    cout << "2. Celsius to Kelvin" << endl;
    cout << "3. Fahrenheit to Celsius" << endl;
    cout << "4. Fahrenheit to Kelvin" << endl;
    cout << "5. Kelvin to Celsius" << endl;
    cout << "6. Kelvin to Fahrenheit" << endl;

    cout << "Enter your choice (1-6): ";
    cin >> choice;

    cout << "Enter temperature value: ";
    cin >> temp;

    switch(choice) {
        case 1:
            converted = (temp * 9/5) + 32;
            cout << temp << " Celsius = " << converted << " Fahrenheit" << endl;
            break;
        case 2:
            converted = temp + 273.15;
            cout << temp << " Celsius = " << converted << " Kelvin" << endl;
            break;
        case 3:
            converted = (temp - 32) * 5/9;
            cout << temp << " Fahrenheit = " << converted << " Celsius" << endl;
            break;
        case 4:
            converted = ((temp - 32) * 5/9) + 273.15;
            cout << temp << " Fahrenheit = " << converted << " Kelvin" << endl;
            break;
        case 5:
            converted = temp - 273.15;
            cout << temp << " Kelvin = " << converted << " Celsius" << endl;
            break;
        case 6:
            converted = ((temp - 273.15) * 9/5) + 32;
            cout << temp << " Kelvin = " << converted << " Fahrenheit" << endl;
            break;
        default:
            cout << "Invalid choice! Please select between 1 and 6." << endl;
    }

    return 0;
}
