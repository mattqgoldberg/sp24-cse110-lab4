1. Line 12 prints out '3'. There is no error because i was declared using the var keyword, so it is still in scope because it lives for the duration of the entire function not just the for loop.

2. Similar to question 1, line 13 will print '150'. The variable is in scope still because it is defined with var. The value 150 comes from the code on line 7, and we are printing out the last value after the for loop, so discountedPrice is equal to 300 * (1 - 0.5) or 150.

3. Line 14 will print '150'. Similar to the other two examples, the variable is in scope since it was declared using var. 150 is simply the final value of discountedPrice multiplied by 100, rounded, then divided by 100 which does not change the value in this case.

4. The function returns an array, where each value in the array is the discounted price from the input array. The for loop goes through each value in the prices array, and calculates the new discount array, appending that discounted price the new output array.

5. Line 12 causes an error because i is not defined in the current scope. Declaring i with the let keyword means that its lifetime is only inside of the for loop, so trying to reference it after the for loop results in an error.

6. Line 13 will have the same error as the previous problem. discountedPrice was defined using the let keyword inside of the for loop, so it cannot be referenced outside the for loop.

7. Unlike the previous two questions, this will print '150' with no error. This is because finalPrice is declared at the top of the function using the let keyword, not inside of the for loop. This means that the variable can be accessed anywhere in the function with no scope issue.

8. This function will return an array with all of the values of discounted prices as intended. No scope issues occur.

9. Just like the previous examples, line 11 will error since i was defined inside of the for loop with the let keyword. It cannot be accessed outside of the for loop.

10. Line 12 will print out the length of the array which is 3. It is a constant which means it cannot be reassigned, but it can be passed into the console.log function with no issue.

11. The fucntion will return the array of discounted prices as intended. Using const in these cases causes not issues as the variable with const are never reassigned. The for loop correctly calculates the discount for each input and appends them to the output array.

12. 
 - A. student.name
 - B. student['Grad Year']
 - C. student.greeting()
 - D. student['Favorite Teacher'].name
 - E. student.courseLoad[0];

13. 

 - A. '3' + 2: Outputs 32, because the integer 2 is converted into a string and concatenated with the string '3'.
 - B. '3' - 2: Outputs 1, since the '-' operator is only for numbers, '3' is converted to a number.
 - C. 3 + null: Outputs 3, since null is converted to the number 0 and 3 + 0 = 3.
 - D. '3' + null: Outputs 3null, since null is converted the string 'null' and concatenated.
 - E. true + 3: Outputs 4, true is converted to the number 1, 1 + 3 = 4.
 - F. false + null: Outputs 0, since false converts to 0 and so does null.
 - G. '3' + undefined: Outputs 3undefined since undefined is converted to string 'undefined' and concatenated.
 - H. '3' - undefined: Since '-' is only numbers, converts both '3' and undefined to 3 and NaN. 3 - NaN = NaN.

14. 
 - A. '2' > 1: Outputs true, since '2' is converted the number 2 in comparisons.
 - B. '2' < '12': Outputs false, since both are strings, they are compared lexicographically, and 2 comes after 1 in the lexicon.
 - C. 2 == '2': Outputs true, since '2' is converted to the number 2 by the equality operator.
 - D. 2 === '2': Outputs false, since the strict equality operator does the check without converted the string into a number.
 - E. true == 2: Outputs false, since true is converted to the number 1.
 - F. true === Boolean(2): Outputs true, since Boolean(2) is converted to true, as it is a truthy value. Ex: Boolean(0) would be converted to false.
 
15. The difference between the == and === operators is the type conversion. The == operator will automatically convert values of different types into numbers before doing the comparison, while === will not do any type conversion.

16. See part2-question16.js

17. The result of the function would be a new output array [2, 4, 6]. This is because the code iterates through each value of the input array, then calls the callback function on this value. The callback function is doSomething() which doubles the value given. This doubled value is returned and then appended to the newArr, which gets returned at the end.

18. See part2.question18.js

19. The code prints 1, then 4, then 3, then 2. 