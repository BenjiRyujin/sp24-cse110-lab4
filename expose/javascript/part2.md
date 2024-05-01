1. The console will return 3, as var i remains in the function scope of discountPrices. It returns 3 because that is the length of the prices array that the for loop is iterating through.
2. The console will return 150, as discountedPrice var was declared in the same function scope as when it is called again. The most recent assignment of a value to discountedPrice was in the last iteration of the for loop, in which the price was 300, then cut it in half to 150 after applying the discount.
3. Similar to the previous question, line 14 will return 150, as the finalPrice is simply the discountedPrice but rounded, which is still 150. 
4. This function will return [50,100,150], the array that was declared in the function scope. The array contains the finalPrices after the discount is added to the initial price array. It is a modification of the initial parameter array [100,200,300].
5. Line 12 will cause an error as 'i' is declared with 'let' which means it is in the scope of the for loop. Line 12 calls 'i' outside of the scope in which it was declared, which causes a reference error.
6. Similar to the last question, line 13 will cause an error as 'discountedPrice' is declared with 'let' in the scope of the for loop, which means it is out of scope outside of the for loop, where it is called in line 13.
7. Line 14 will output 150 into the console, as it is declared with 'let' in the scope of the function, rather than the for loop. 
8. The function will return [50,100,150], as discounted was declared in the function scope with 'let', so it is still able to be referenced when called at the end of the function. It is returning the modified array of the input array of prices, [100,200,300], after applying the discount. 
9. Line 11 will cause an error as it is trying to reference 'i', which is declared in the scope of the for loop, and it is called out of scope in line 11.
10. Line 12 will return the length of the prices array, which is 3. 'length' is declared with 'const' in the scope of the function, which allows it to be called later on in the same function. 
11. This function will return [50,100,150], even though it was declared with 'const'. Although 'discounted' cannot be reassigned to a different array or value, it doesn't mean that the contents of the array it is assigned to is immutable. In this case, the for loop is simply pushing into the array, or changing the contents, not reassining the variable to another array. 
12.  
    A. student.name
    B. student['Grad Year']
    C. student.greeting()
    D. student['Favorite Teacher][name]
    E. student.courseLoad[0]
13.  
    A. '32'; integers map to string representation when performing concatenation
    B. 1; string is converted to number to perform subtraction
    C. 3; null is converted to number 0 due to addition
    D. '3null'; null is converted to string due to concatenation
    E. 4; true is converted to 1 due to addition
    F. 0; false and null converted to 0 due to addition
    G. '3undefined'; undefined is converted to string due to concatenation
    H. NaN; undefined is converted to NaN due to subtraction
14.  
    A. true; '2' is converted to number for comparison
    B. false; strings are compared as they are both strings and the first character, '2', is greater than the first character of the second string '1'
    C. true; string is convertd to number before comparison
    D. false; === performs comparison before any typecasting, 2 is not same type as '2', so false
    E. false; true is converted to 1 as a number, not 2
    F. true; despite no typecasting, Boolean(2) is a boolean as any number greater than 0 is true as a boolean
15. == performs type conversion before comparison, while === checks the equality strictly without type conversion.
17. The result will be the array [2,4,6], as the input array [1,2,3] is iterated through and at each index, the value is multiplied by 2 through the doSomething function and then pushed to the new array, which is returned after the loop finishes.
19. 1 4 3 2