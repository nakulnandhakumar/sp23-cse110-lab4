# Part 2
1. 3 should be printed since `var i` should ignore block scope and should be 3 
after it finishes executing
2. It should print 150. Because `discountedPrice` was declared using `var` it should ignore block scope
and therefore no error should occur. The last value that is assigned to `discountedPrice`
should be 150 so that's what it will print
3. Should also print 150 for the same reasons as above, `var` ignores blockscope and last value assigned to `finalPrice` is 150
4. No error occurs and the function will return a list of discounted prices, `[50,100,50]`
5. There is an error because `i` was declared with `let` in another scope than where it is being referenced and `let` has blockscope
6. 