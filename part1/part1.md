### Part 1a:
1. Line 9 prints "values added: 20"

2. Line 13 prints "final result: 20"

3. Line 9 prints "values added: 20"

4. Line 13 returns an error, because result in this case is undefined. *result* is not defined outside of the if block, as the let keyword only defines a variable in the block it is defined in.

5. Line 9 returns an error, because result is previously assigned as 0, and because it was defined as a const, result can't be reassigned to `num1 + num2`

6. Line 13 returns an error, because result is previously assigned as 0, and because it was defined as a const, result can't be reassigned to `num1 + num2`

### Part 1b:
1. At line 12, the console will print the final version of i, because i is defined as a var in the for loop, and because of this, i is accessible anywhere in the script. In this case, from the function call `discountPrices([100, 200, 300], 0.5)`, `console.log(i)` returns 2.

2. At line 13, discountedPrice is printed, as discountedPrice is defined as a var in line 7. Because of this declaration, discountedPrice is accessible anywhere in the script. In this case, from the function call `discountPrices([100, 200, 300], 0.5)`, `console.log(discountedPrice)` returns 150.

3. At line 14, finalPrice is printed, as finalPrice is declared at line 4 as a var. This means that finalPrice is accessible anywhere in the script, and can be reassigned any number of times. In this case, from the function call `discountPrices([100, 200, 300], 0.5)`, `console.log(finalPrice)` returns 150.

4. This function will return the *discounted* array, which is the original input array with its elements multiplied by the quantity (1-discount). In this case, the function call `discountPrices([100, 200, 300], 0.5)` will return the array [50, 100, 150].

5. At line 12, the code will cause an error, as i is not able to be accessed outside of the for loop block because it was declared with the *let* keyword.

6. At line 13, the code will cause an error, as discountedPrice is not able to be accessed outside of the for loop block because it was declared with the *let* keyword.

7. At line 14, the correct finalPrice is returned, as finalPrice is declared with the *let* keyword inside of the function. Because finalPrice is to be accessed within the same scope, it is accessible. In this case, from the function call `discountPrices([100, 200, 300], 0.5)`, `console.log(finalPrice)` will return 150.

8. This function returns the final *discounted* array, that contains the new prices with the input prices modified by the discount argument. This function multiplies all the input prices by the quantity (1-discount). From the call `discountPrices([100, 200, 300], 0.5)`, the array returned is [50, 100, 150]

9. At line 11, the code will cause an error, as i is not able to be accessed outside of the for loop block because it was declared with the *let* keyword.

10. At line 12, the code will return length, which is initially set to `prices.length`. If we were to run the function call `discountPrices([100, 200, 300], 0.5)`, then length would be set to the length of the prices input array, which would be 3. So, line 12 will output "12" to the console.

11. This function will return the *discounted* array, which is the original input array with its elements multiplied by the quantity (1-discount). In this case, with the function call `discountPrices([100, 200, 300], 0.5)`, the function returns the array [50, 100, 150].

12. A. `student.name`  
    B. `student["Grad Year"]`  
    C. `student.greeting()`  
    D. `student["Favorite Teacher"].name`  
    E. `student.courseload[0]`  

13. A. 32 - This happens because '3' is treated as a string, and we concatenate the following term 2 as a string to 3.  
    B. 1 - This happens because there is no valid subtraction for a string, and '3' is converted to a numeric 3. So, 3 - 2 = 1.  
    C. 3 - This happens because null is treated as a 0, and 3 + 0 = 0.  
    D. 3null - This happens because '3' is treated as a string, and we concatenate the following term 'null' as a string to it.  
    E. 4 - This happens because true is treated as a 1, and 1 + 3 = 4.  
    F. 0 - This happens because false is treated as a 0, and null is also treated as a 0. So, 0 + 0 = 0.  
    G. 3undefined - This happens because '3' is treated as a string, and we concatenate the following term 'undefined' as a string to it.  
    H. NaN - This happens because there is no valid subtraction for a string, and we convert 3 to a numeric value. However, undefined has no value assigned to it, so this line tries to subtract an undefined value from 3, for which can't be calculated - and returns NaN (Not a Number).  

14. A. true - This is because JavaScript converts the values to numbers when comparing different types. So, because 2 > 1, it returns true.  
    B. false - This is because JavaScript compares strings character by character. So, because '2' is not equal to '1', there is no need to proceed further into the strings, and checks if '2' is less than '1', which evaluates to false.  
    C. true - This happens because Javascript converts the values to numbers when comparing different types. So, because 2 is equal to 2, it returns true.  
    D. false - This happens because the strict equality operator `===` immediately returns false when comparing different typed values, where in this case '2' is a string, and 2 is a number.  
    E. false - This happens because Javascript converts the values to numbers when comparing different types. So, because true, when converted to a number, becomes 1, 1 is not equal to 2, so this returns false.  
    F. true - This happens because the Boolean(2) conversion evaluates to true, as 2 is not 0 or empty. By using the strict equality operator, it checks both boolean values, and returns true, as true is equal to true.  

15. `==` checks equality, but because of the way JavaScript converts variable types, it is possible that JavaScript fails to provide the correct answer. So, `===` checks equality without conversion, and only checks if they are equal if they are the same type.

16. *in part1b-question16.js*

17. In the function call `modifyArray([1,2,3], doSomething)`, the result is a returned array `[2,4,6]`. This is because we go into modifyArray, and input the parameters [1,2,3] and the function doSomething. We first define an empty newArr as const. We then iterate through the input array, and on each element of the input array, we push into newArr a modified value of the element in the input array using callback. In this case, our callback function was doSomething, which returns a doubled input value. So, the value pushed into newArr is double the input array's elements. We then return the newArr array which contains the doubled values.

18. *in part1b-question18.js*

19. This code outputs (in new lines) `1, 4, 3, 2`. This happens because setTimeout outputs the code after a set delay. Because `console.log(1)` and `console.log(4)` don't have setTimeout associated with them, they print first, but 3 prints after because it has a delay of 0, and 2 prints last because it is delayed by 1 second.