1. The bug was that the values of num1 and num2 were both strings. When adding them together, this caused the string to concatenate instead of being converted to numbers where they could be added properly.

2. By casting both num1 and num2 to Number types inside of the calculate sum function, the intended result of adding the two numbers is achieved.