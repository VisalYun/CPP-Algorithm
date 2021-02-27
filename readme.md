### Basic Syntax
```
#include <iostream>
using namespace std;

int main() {
  cout << "Hello World!";
  return 0;
}
```
### Printing the output
```
cout << "Hello World!";
```
**Adding the new line**
```
cout << "Hello World! \n";
// OR
cout << "Hello World!" << endl;
cout << "I am learning C++";
```
### Variable
**Declaring Variable**
```
// data_type variable_name = value;
int age = 18;
```
Data type:
- int - stores integers (whole numbers), without decimals, such as 123 or -123
- float - stores floating point numbers, with decimals, such as 19.99 or -19.99. Sufficient for storing 7 decimal digits
- double - stores floating point numbers, with decimals, such as 19.99 or -19.99. Sufficient for storing 15 decimal digits
- char - stores single characters, such as 'a' or 'B'. Char values are surrounded by single quotes
- string - stores text, such as "Hello World". String values are surrounded by double quotes
- bool - stores values with two states: true or false
**const**
make the variable unchangeable and read-only.
```
const int myNum = 15;  // myNum will always be 15
myNum = 10;  // error: assignment of read-only variable 'myNum'
```
**Printing variable**
```
cout << "I am " << << myAge << " years old.";
```
### Getting user input
```
int x;
cout << "Type a number: "; // Type a number and press enter
cin >> x; // Get user input from the keyboard
cout << "Your number is: " << x;
```
### Operator
**Arithmetic Operators**
- **+**	    Addition	Adds together two values
- **-**	    Subtraction	Subtracts one value from another
- *	        Multiplication	Multiplies two values
- **/**	    Division	Divides one value by another
- **%**	    Modulus	Returns the division remainder
- **++**    Increment	Increases the value of a variable by 1
- **--**    Decrement	Decreases the value of a variable by 1
**Note**:   Different between ++x and x++
```
// Prefix increment
let prefix = 1;
console.log(++prefix); // 2
console.log(prefix); // 2

// Postfix increment
let postfix = 1;
console.log(postfix++); // 1
console.log(postfix); // 2
```
**Assignment Operator**
we use the assignment operator (=) to assign the value to the variable
**Logical Operator**
- && 	Logical and	Returns true if both statements are true
- || 	Logical or	Returns true if one of the statements is true
- !	    Logical not	Reverse the result, returns false if the result is true
### String
Don't forget to add **#include <string>** as the header file.
**Operation**
- Concatenate: *str1 + str2*
- Check length: *str.length()*
- User Input Strings
```
#include <iostream>
#include <string>
using namespace std;

int main() {
  string fullName;
  cout << "Type your full name: ";
  getline (cin, fullName);
  cout << "Your name is: " << fullName;
  return 0;
}
```
### Condition
```
if (condition1) {
    //do sth..
} else if (condition2) {
    //do sth..
} else {
    //do sth..
  }
```
**Shorthand**
```
variable = (condition) ? expressionTrue : expressionFalse;
```
### Loop
**while loop**
```
while (condition) {
  // code block to be executed
}
```
**do-while loop**
```
do {
  // code block to be executed
}
while (condition);
```
**for loop**
```
for (statement 1; statement 2; statement 3) {
  // code block to be executed
}
```
- Statement 1 is executed (one time) before the execution of the code block.
- Statement 2 defines the condition for executing the code block.
- Statement 3 is executed (every time) after the code block has been executed.
### Array
**Declaring array**
```
string cars[4];
int myNum[3] = {10, 20, 30};
```
**Loop through array**
```
string cars[4] = {"Volvo", "BMW", "Ford", "Mazda"};
for(int i = 0; i < 4; i++) {
  cout << cars[i] << "\n";
}
```
**Omit Elements on Declaration**
```
string cars[5];
cars[0] = "Volvo";
cars[1] = "BMW";
...
```