# Part 1

1. 20 is printed. 
2. 20 is printed also here because the `var` keyword used to declare the variable ignores block scope
3. 20 is printed
4. There is an error here. The variable `result` isn't recognized here because
it was defined using the `let` keyword which means it has block scope and cannot be seen outside of the block it was defined in
5. There is an error here. We assign 0 to `const result` and then try to reassign another value to it `sum1 + sum2` which is against the rules of a `const` variable
6. There is an error here for the same reasons as problem #4 because `const result` has the same scope as `let result` and the program is trying to access it in another scope than which it was declared.