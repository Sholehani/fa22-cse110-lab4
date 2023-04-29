1. 3: `var i = 0` in the `for` loop can be accessed outside the loop and even outside the function. This means `i` keeps the last value it obtained within the `for` loop. Therefore, line 12, which accesses `i` outside the `for` loop, returns this last value.
2. 150: In line 7, `var = discountedPrice` can be accessed outside the `for` loop it's in and outisde the function. Therefore, `discountedPrice` outside the for loop (like in line 13) keeps the last value it changed to within the `for` loop.
3. 150: `finalPrice` was initalized as a `var`, meaning it scopes anywhere in the function. Therefore, `finalPrice` keeps the last value it changed to within the `for` loop and returns this value when called in line 14;
4. [50, 100, 150]: In line 9, the function pushes `finalPrice` onto `var = discounted = []`, which updates `discounted` to an array carrying the updated prices of the original `prices` array. Since `discounted` is a `var`, it is accessible within the `for` loop and keeps the updated values after the loop. So, line 13 returns the `discounted` array with the updated prices.
5. error: `let i = 0;` in the `for` loop sets `i`'s scope to only the loop, making it inaccessible in line 12, which is outside the loop.
6. error: `let discountedPrice` in the `for` loop sets `discountedPrice`'s scope to only the loop, making it inaccessible in line 13, which is outside the loop.
7. 150: Since `let finalPrice` was declared at the beginning of the function, it is accessible throughout the entire function, but not outside of it. This means the `finalPrice` used inside the `for` loop in line 8 is updated and keeps its final value when used outside the loop. Therefore, `finalPrice` value is 150 by line 14.
8. [50, 100, 150]: The `let` used in line 3 initializes `discounted` to be accessible throughout the entire function, meaning it is accessed inside the `for` loop in line 9 and is properly updated. `discounted` then holds the updated prices after the `for` loop. Therefore, the function returns this list of prices in since line 16 returns `discounted` after the loop and within the function.
9. error: `let i = 0;` in the `for` loop sets `i`'s scope to only the loop, making it inaccessible in line 11, which is outside the loop.
10. 3: `length` is initialized in line 4, and is never changed throughout the function. So, `const length = price.length` sets `length` equal to the `price` array's length, which is 3. Therefore, line 12 returns 3.
11. [50, 100, 150]: Line 3 declares `discounted` as a `const` array. This means `discounted` can be manipulated, but not reassigned to a new array. Line 8 pushes new values into `discounted`, which does not reassind the array. This means line 8 is valid in changing the contents of `discounted` to the list of discounted price of each `prices` value. Therefore, the function returns the discounted price of `prices` values.
12. 
    A.  student.name
    B.  student['Grand Year']
    C.  student.greeting();
    D.  student['Favorite Teacher'].name
    E.  student.courseLoad[0]
13. 
    A.  32: 2 converts to string '2' and appends  '3'
    B.  1: '3' converts to number 3; 3 - 2 = 1
    C.  3: `null` converts to number 0; 3 + 0 = 3
    D.  3null: `null` converts to string 'null' and appends '3'
    E.  4: true converts to number 1; 1 + 3 = 4
    F.  0; fale and `null` bother convert to number 0; 0 + 0 = 0
    G.  3undefined: `undefined` converts to string 'undefined' and appends '3'
    H.  NaN: `undefined`  converts to its numeric value `NaN`
14. 
    A.  true: '2' converts to number 2; 2 > 1 is true
    B.  true: both strings convert to their corresponding numbers; 2 > 12 is true
    C.  true: '2' converts to number 2; 2 == 2 is true
    D.  false: 2 and '2' are different types
    E.  false: true converts to number 1; 1 == 2 is false
    F.  true: `Boolean(2)` evaluates to true and becomes a boolean value; true === true is true
15. `==` operators allow type conversion. `===` operators do not allow type conversions and will return false is operands of different types. 
16. [refer to `part2-question16.js`]
17. [2, 4, 6]: The `callback` parameter in `modifyArray` uses the `doSomething` function on each `array` element in line 4. According to `doSomething`, the elements of `array` are each multiplied by 2. These values are pushed onto `newArr`, which is returned by the end of the function.
18. [refer to `part2-question18.js`]
19. 1
    4
    3
    2
20. 