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

7.