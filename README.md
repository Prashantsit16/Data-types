# Data-types
Aim:
To understand and demonstrate the use of storage classes in C++, and to find the sizes of different data types using the sizeof operator. This involves exploring the characteristics of various storage classes and determining the memory allocated for different data types.

Theory:
Storage classes in C++ define the scope, visibility, and lifetime of variables and functions. The primary storage classes are:

auto: The default storage class for local variables.
static: Preserves the value of a variable across function calls.
extern: Defines a variable that is shared across multiple files.
register: Suggests that a variable be stored in a CPU register for faster access (though this is a suggestion, not a guarantee).

.The sizeof operator is used to determine the size in bytes of a data type or variable, providing insights into memory allocation.

Procedure:
Include Required Headers:

cpp
#include <iostream>
using namespace std;
Define Main Function:

Declare variable
int main() {
    Variable declarations
    int a = 10;
    static int b = 20;
    extern int c; // Assume 'c' is defined elsewhere
    register int d = 30;

    Displaying the data types :
    cout << "Size of int: " << sizeof(int) << " bytes" << endl;
    cout << "Size of char: " << sizeof(char) << " bytes" << endl;
    cout << "Size of float: " << sizeof(float) << " bytes" << endl;
    cout << "Size of double: " << sizeof(double) << " bytes" << endl;

    // Display storage class usage (values of variables)
    cout << "Value of auto variable a: " << a << endl;
    cout << "Value of static variable b: " << b << endl;
    cout << "Value of register variable d: " << d << endl;

    return 0;
OUTPUT:
1.Size of data types
![Screenshot 2024-09-05 153032](https://github.com/user-attachments/assets/26453ab5-bdf4-4a3c-ae07-aaaca3afcd4c)

2.Storage class:
![Screenshot 2024-09-05 153040](https://github.com/user-attachments/assets/eb451f52-9708-408e-849d-e572b88e5086)

Conclusion:
Understanding storage classes and the sizeof operator in C++ provides crucial insights into variable management and memory allocation. Storage classes control variable scope and lifetime, while sizeof helps in determining memory usage for different data types. This knowledge is fundamental for efficient programming and memory management. The example illustrates practical applications and reinforces these core concepts effectively.
