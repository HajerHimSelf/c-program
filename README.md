#include <iostream>
using namespace std;

int main() {
    const int SIZE = 10;
    int numbers[SIZE];

   cout << "Enter 10 numbers: ";
    for (int i = 0; i < SIZE; ++i) {
     cin >> numbers[i];
    }

    bool ordered = true;
    for (int i = 1; i < SIZE; ++i) {
        if (numbers[i] < numbers[i - 1]) {
            ordered = false;
            break;
        }
    }

    if (ordered) {
      cout << "Ordered ascendingly"<<"\n";
    } else {
   cout << "Unordered ascendingly"<<"\n";
    }

    return 0;
}
    
    
