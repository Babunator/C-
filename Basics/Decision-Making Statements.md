# If Statement
It instructs the compiler to execute the block of code only if the condition holds true. 
- Syntax:
```
if (expression)
{ //code}
```
- Example: 
```cpp
#include <iostream>

int main () {
int b;
std::cout << "Type a number: ";
std::cin >> b; 
if( b < 20 ) {    //If statement to check if entered number is less than 20
std::cout << "Your number is less than 20;" << std::endl;
}
std::cout << "Value of your number is : " << b << std::endl;

return 0;
}
```

# If...Else Statement
This is an extension of the ‘if’ statement. It instructs the compiler to execute the ‘if’ block only if the specified condition is true. Otherwise, it executes the ‘else’
block. 
- Syntax:
```
if (expression)
{//code}
else
{//code}
```
- Example: 
```cpp
#include <iostream>

int main () {
int b;
std::cout << "Type a number: ";
std::cin >> b; 
if( b < 20 ) {    //If statement to check if entered number is less than 20
std::cout << "Your number is less than 20;" << std::endl;
}
else {            //Else statement if the number is more than 20
    std::cout << "Your number is more than 20;" << std::endl;
}
std::cout << "Value of your number is : " << b << std::endl;

return 0;
}
```
# Switch Statement
When you need to execute conditions against various values, you can use switch statements.
- Syntax:
```
switch(expression) {
case constant-expression :
statement(s);
break; //optional
case constant-expression :
statement(s);
break; //optional

default : //Optional
statement(s);
}
```
- Example: 
```cpp
#include <iostream>

int main () {

char grade; // local variable declaration:

std::cout << "Type your grade(A,B,C,D,F): ";
std::cin >> grade; 

switch(grade) {
case'A' :
std::cout << "Outstanding!" << std::endl;
break;
case'B' :
case'C' :
std::cout << "Well done" << std::endl;
break;
case'D' :
std::cout << "Pass" << std::endl;
break;
case'F' :
std::cout << "Try again" << std::endl;
break;
default :
std::cout << "Invalid grade" << std::endl;
}
std::cout << "Your grade is " << grade << std::endl;

return 0;
}
```
