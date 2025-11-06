#include <iostream>
using namespace std;

int main() {
    // Declare and initialize an array
    double sales[] = {12.25, 32.50, 16.90, 23.00, 45.68};

    // Display all elements
    cout << "Sales values:" << endl;
    int size = sizeof(sales) / sizeof(sales[0]);
    for (int i = 0; i < size; i++) {
        cout << "sales[" << i << "] = " << sales[i] << endl;
    }

    // Calculate and display average
    double total = 0;
    for (int i = 0; i < size; i++) {
        total += sales[i];
    }

    double average = total / size;
    cout << "\nAverage sales = " << average << endl;

    return 0;
}
