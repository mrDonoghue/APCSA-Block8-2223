# Lab 0: Numismatics
Write a program that will allow the user to enter an amount in cents, and outputs the number of quarters, dimes,
nickels, and pennies needed to add up to the amount.
Your program should use as many quarters as possible, then as many dimes as possible, etc.

## Example: The user enters 82

Your program should output:
```
Quarters: 3
Dimes: 0
Nickels: 1
Pennies: 2
```
Note that 2 quarters, 3 dimes, and 2 pennies would be incorrect for this task
even though that does add to 82 cents (it doesn't use as many quarters as possible).


## Requirements for an A
* your program should work
* use the static method `getIntFromUser()` from the `Util.java` file
* you don't need to worry about the user misbehaving (e.g., entering a negative amount of cents or a non-int number)
* you should use well-named variables (camelCase, meaningful, etc.)
* you should use variables where it helps make the code more readable
* you must use at least one compound assignment operator (`+=`, `*=`, etc.)
* you can help each other, but don't give each other code!! (This includes letting someone look at your code while they copy it down)


## Hints:
<details>
  <summary> Hint 0: How can we handle user input?</summary>
   
   There is a static method, `getIntFromUser()` in the `Util.java` file.

   Remember that we use static methods by using dot notation!
  
</details>
<details>
  <summary> Hint 1: How can you figure out how many quarters should be used?</summary>
  
  What's the most number of quarters that can be used for 26 cents? Why? What about 30 cents? What about 52 cents?
  
  Is there an operator that might help us answer this question?
  
</details>

<details>
  <summary> Hint 2: How can you figure out how many quarters should be used?</summary>
  
  Wait a minute! Would int division solve this problem for us?
</details>

<details>
  <summary> Hint 3: How can you figure out how many cents are left after taking care of the quarters?</summary>
  
  Is there an operator that helps us think about what's left over after doing int division?
  
</details>


<details>
  <summary> Hint 4: How can you figure out how many cents are left after taking care of the quarters?</summary>
  What about the modulo operator?
</details>


## Bonus:
In real life, a program is rarely ever actually finished. Here are some ideas for ways to improve the program. Note that these updates are not required.
* Instead of prompting the user for a single number, prompt the user for two numbers: the cost of an item and the amount paid by a customer. Then your program can calculate how a cashier might make change.
* Instead of accepting ints, perhaps your program could accept doubles to allow the user to enter something closer to the way most people think about prices. (Hint: try scan.nextDouble() instead.) How can you reasonably turn the doubles into something nicer to work with? Might it still be helpful to convert to cents? Can you use casting somehow?
* Especially if you start working with doubles, it might be nice to modify the program to report how many of each bill ($100, $50, $20, $10, $5, and $1) can be used as well.
* If you've modified the program to accept a price and a payment (like the first bullet), you might modify the program to incorporate sales tax into the actual cost of the transaction.
* Perhaps this transaction is happening at a business where tipping occurs? Maybe you might also prompt the user to provide what percentage they'd like to tip, and included that in the actual cost of the transaction.
