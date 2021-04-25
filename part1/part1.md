## Lab4 - part1

### Part 1a. A quick Introduction...

1. At line 9, it prints **values added: 20**. It won't cause error since var can be accessed anywhere inside sumValues function.

2. At line 13, it prints **final result: 20**. Even though declaration of the result variable is inside if condition, it still won't cause any error since the result variable is still inside sumValues function.

3. At line 9, it prints **values added: 20**. Since the commond is in the same block scope (still in the if condition) with the let declaration of the result variable, it won't cause any error.

4. The code returns an error at line 13. The command which calls the result variable is outside the if condition, so it is in the different scope with the let declaration. So it would cause an error.

5. At line 9, it prints **values added: 20**. Similar to let declaration, since the command is inside the if condition, which is the scope of const declaration, it would print normally.

6. The code returns an error at line 13. Similar to let declaration, the command which calls the result variable is outside the if condition, so it is in the different scope with the const declaration. So it would cause an error.

<hr>

### Part 1b. A Little More of a Challenge

1. It would print **3** at line 12. Since i is declared by var, it is valid inside the whole function. Since there is a for loop before line 12 which takes i from 0 to prices.length and since there are 3 elements in total, the value of i is 3 after the for loop.

2. It would print **150** at line 13. The value of discountedPrice is updated in each turn of the for loop and its final value should be decided by the last value in discounted array, which is `300 * (1 - 0.5) = 150`.

3. It would print **150** at line 14. Since finalPrice is declared by var, it is valid inside the whole function. The value of finalPrice is updated by discountedPrice. So it should be `Math.round(150 * 100) / 100 = 150`.

4. It would return **[50, 100, 150]**. discounted is declared as an empty array at line 3. For each turn in the for loop, we add finalPrice at the end of the discounted array.

5. The code causes an error at line 12. Since i is declared by let, its scope is restricted inside the for loop. Since the command which call i is outside the for loop, it would cause an error.

6. The code causes an error at line 13. Since discountedPrice is declared by let, its scope is restricted inside the for loop. Since the command which call discountedPrice is outside the for loop, it would cause an error.

7. It would print **150** at line 13. Since finalPrice is declared before for loop, its scope is the whole function, so it won't cause error when we call it in line 14 outside the for loop. The value of discountedPrice is updated in each turn of the for loop and its final value should be decided by the last value in discounted array, which is `300 * (1 - 0.5) = 150`.

8. It would return **[50, 100, 150]**. There are no commands which call variables outside their scopes, so it won't cause any error. discounted is declared as an empty array at line 3. For each turn in the for loop, we add finalPrice at the end of the discounted array.

9. The code causes an error at line 11. Since i is declared by let, its scope is restricted inside the for loop. Since the command which call i is outside the for loop, it would cause an error.

10. It would print **3** at line 12. Since length is declared outside the for loop, its scope is the whole function. Since the value of scope is the length of the prices array and there are 3 elements in the array, length is equal to 3.

11. It would return **[50, 100, 150]**. There are no commands which call variables outside their scopes, so it won't cause any error. discounted is declared as an empty array at line 3. For each turn in the for loop, we add finalPrice at the end of the discounted array.

<hr>

12. A) `student.name` <br>
    B) `student["Grad Year"]` <br>
    C) `student.greeting()` <br>
    D) `student["Favorite Teacher"].name` <br>
    E) `student.courseLoad[0]`

<hr>

13. A) '3' + 2 = **'32'**. Since '3' is a string, the plus sign adds two strings together. Integers map to their exact string representation. <br>
    B) '3' - 2 = **1**. Since we can't do substraction on strings, JS converts string to its number representation. <br>
    C) 3 + null = **3**. Since 3 is a number and null can be absence of any object value, the answer follows 3's representation. <br>
    D) '3' + null = **'3null'**. Since '3' is a string, the plus sign adds two strings together, so it inteprets null as the string "null" and put two components together. <br>
    E) true + 3 = **4**. Since we can't add two booleans, the plus sign follows 3 and inteprets true as a number, adding 1 and 3 together. <br>
    F) false + null = **0**. False maps to 0 and null maps to 0. The plus sign then adds two numbers together. <br>
    G) '3' + undefined = **'3undefined'**. Since '3' is a string, undefined maps to 'undefined. Then the plus sign addes two strings together. <br>
    H) '3' - undefined = **NaN**. We can do substraction on numbers. Since we only have '3' and undefined, JS comes out with NaN (not a number). <br>

14. A) **true**. '2' maps to number 2, which is greater than number 1. <br>
    B) **false**. '2' and '12' are both strings and '2' is larger than '12'. <br>
    C) **true**. '2' maps to number 2, which is the same with 2 on the left hand side. <br>
    D) **false**. === means 'strict equality'. Since 2 and '2' are not in the same type, it returns false. <br>
    E) **false**. true maps to number 1, which is not equal to number 2. <br>
    F) **true**. `Boolean(2)` is true, which is strictly equal to true on the left.

15. `===` always considers values in different types as different values and return false if values are not comparable. In comparison, `==` can convert values if they can be comparable under other representations (ex. `2 === '2'` returns false while `2 == '2'` returns true).

<hr>

16. Code in **part1b-question16.js**.

<hr>

17. The result would be **[2, 4, 6]**. The modifyArray function has two arguments: an array and a callback function, which return 2 times the original number. As we iterate all numbers in the for loop, the callback function return 2, 4, 6 for 1, 2, 3, respectively.

<hr>

18. Code in **part1b-question18.js**.

19. The output is <br>
    **1** <br>
    **4** <br>
    **3** <br>
    **2** <br>