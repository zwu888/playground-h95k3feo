#description: 
 variables with static storage duration are zero initialized.  Note that x has static storage duration even though the static keyword is not used.  According to the standard: "All objects which do not have dynamic storage duration, do not have thread storage duration, and are not local have static storage duration"
```C++ runnable

#include <iostream>

int x;

int main()
{
    int y;
    std::cout << x << std::endl;
    std::cout << y << std::endl;
    return 0;
} 
