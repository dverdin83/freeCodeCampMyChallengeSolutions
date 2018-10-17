```Javascript
/* Project Euler: Problem 1: Multiples of 3 and 5
If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23.

Find the sum of all the multiples of 3 or 5 below the provided parameter value number.
*/

/* PSEUDOCODE
1.Pass number argument into function multiplesOf3and5,
2..In the function multiplesOf3and5 declare and initialize variable sumOfmultiplesOf3and5 = 0.
3...Create a for loop with variable i which incraments by 1 and terminates when it reaches a value of argument number.
4....In the for loop, test if i is evenly divisible by 3 or 5 using a modulus operator.
5a....If the i is divisible by 3 or 5 add it to the variable sumOfmultiplesOf3and5.
5b..... If i is not divisible by 3 or 5 run the loop again.
6......When the loop is finished return sumOfmultiplesOf3and5.  
*/

"use strict";

function multiplesOf3and5(number) {
  let sumOfmultiplesOf3and5 = 0;
  for (let i = 1; i < number; i++) {
    if (i%3 === 0 || i%5 === 0) {
      sumOfmultiplesOf3and5 += i;
    }
  }
  return sumOfmultiplesOf3and5;
}

//Solution^
```
