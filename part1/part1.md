## Part 1
### 1a)
1. Output: "values added: 20"
2. Output: "final result: 20"
3. Output: "values added: 20"
4. No output; Code will return an error because result is not defined outside of the function, it is only defined in the scope of the "if (add)" block.
5. No output; Code will return an error because you are trying to assign a new value to the const variable 'result'.
6. (same as 5) No output; Code will return an error because you are trying to assign a new  value to the const variable 'result'.

### 1b)
1. The console will output "3" because we have finished looping across the input array 'prices', so the i variable will be = 3 (and can be output by console because i is in function scope because it is type 'var').
2. The console will output "150" because 'discountedPrice' will hold the last discounted price, which is 300 * (1-.5) = 150 (type 'var', so can be accessed in function scope)
3. The console will ouptut "150" because 'discountedPrice' holds the last discounted price 150, and that is used to round: Math.round(150*100)/100 = 150.
4. The function returns the array [50, 100, 150] because this function calculates the discounted price of each item, rounded to the nearest integer, and stores them into the array 'discounted'.
5. The code will error because 'i' is declared as 'let', so 'i' only exists within the scope of the for loop. 'i' is not defined in function scope.
6. The code will error because 'discountedPrice' is declared as 'let', so 'discountedPrice' only exists within the scope of the for loop. 'discountedPrice' is not defined in function scope.
7. The console will output "150" because although 'finalPrice' is declared by 'let', the log function is within the same scope in which finalPrice is defined.
8. The function returns the array [50, 100, 150] because this function calculates the discounted price of each item, rounded to the nearest integer, and stores them into the array 'discounted'. 'discounted' is declared within the same scope as the return line, so there are no issues.
9. The code will error before outputting anything because at line 8, you are trying to change the array 'discounted' by adding an element to it when the array is const and not allowed to be modified.
10. (same as 9) The code will error before outputting anything because at line 8, you are trying to change the array 'discounted' by adding an element to it when the array is const and not allowed to be modified.
11. The function cannot return anything because it will error for the same reason as 9 and 10. It errors because at line 8, you are trying to change the array 'discounted' by adding an element to it when the array is const and not allowed to be modified.
12. A) `student.name`  
    B) `student['Grad Year']`  
    C) `student.greeting()`   
    D) `student['Favorite Teacher'].name`  
    E) `student.courseLoad[0]`  
13. A) '3' + 2 = '32'; integer 2 maps to its string representation  
    B) '3' - 2 = 1; subtraction has no meaning with strings, so string 3 maps to its integer representation and subtraction is performed  
    C) 3 + null = 3; null maps to integer 0  
    D) '3' + null = '3null'; null should be converted to string representation because we are adding to a string  
    E) true + 3 = 4; true maps to integer 1  
    F) false + null = 0; doing math which doesn't make sense on booleans and null, so false is converted to integer 0, null converted to integer 0.  
    G) '3' + undefined = '3undefined'; undefined should be converted to string representation because we are adding to a string  
    H) '3' - undefined = NaN; subtraction has no meaning with strings, so numeric conversion is attempted, but undefined maps to NaN, so result must be NaN.  
14. A) '2' > 1 = true; converting 2 to integer representation for numeric comparison  
    B) '2' < '12' = false; string comparison, comparing '2' and '12' by lexicographical order - '1' comes earlier than '2', so '12' < '2'  
    C) 2 == '2' = true; converting '2' to integer representation for numeric comparison  
    D) 2 === '2' = false; using strict equality, so no conversions are done - int and string are not the same  
    E) true == 2 = false; converting true to integer 1, 1 != 2  
    F) true == Boolean(2) = true; Boolean(2) explicitly casts 2 to true (because it is non-zero), so true == true
15. '==' cannot differentiate between values if, when converted automatically, they are the same value. '===' is strict equality, so if the left and right side do not match types, it immediately returns false (no conversion).  
16. (question16 is js file)
17. Result: modifyArray will return the array [2,4,6].  
    when modifyArray is called, the callback function to be used is `doSomething(num)`. modifyArray creates a new array 'newArr', and pushes to it the return value of the callback function on each element of 'array', `doSomething(array[i])` in this case. So really, the elements pushed onto 'newArr' are the elements of 'array', doubled.  
18. (question18 is js file)
19. The output is '1', then '3', then 1 second later, '2'.