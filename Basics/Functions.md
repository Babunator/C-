# Defining a Function
- Syntax for defining a function in C++:
```
return_type function_name( parameter list ) {
body of the function
}
```
Where:

- ``return_type`` specifies the type of value being returned by that function. 
- ``function_name`` specifies the name of the function and needs to be unique. 
- ``parameter list`` allows you to pass more than one value to your function, along with their data types. 
- ``body of the function`` specifies the set of instructions to accomplish a task. 

For example:
```cpp
#include <iostream>

int max(int num1, int num2) { // declaring the function max with parameters num1 and num2
    int result;
    
    if (num1 > num2)
    result = num1;
    else
    result = num2;
    
    return result;
}

```

# Calling a function
To call a function, write the function's name followed by two parentheses () and a semicolon;
```cpp
#include <iostream>

int max(int num1, int num2) { // declaring the function max with parameters num1 and num2
    int result;
    
    if (num1 > num2)
    result = num1;
    else
    result = num2;
    
    return result;
}

int main () {
    int a = 100;
    int b = 200;
    int ret;
    
    ret = max(a, b); //calling on function max()
    std::cout << "Max value is : " << ret << std::endl;
    
    return 0;
}
```
