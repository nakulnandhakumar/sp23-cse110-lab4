# Part 2
1. 3 should be printed since `var i` should ignore block scope and should be 3 
after it finishes executing
2. It should print 150. Because `discountedPrice` was declared using `var` it should ignore block scope
and therefore no error should occur. The last value that is assigned to `discountedPrice`
should be 150 so that's what it will print
3. Should also print 150 for the same reasons as above, `var` ignores blockscope and last value assigned to `finalPrice` is 150. Also even if the variable was defined with `let` it would still work because the variable is being accessed in the same scope that it was declared
4. No error occurs and the function will return a list of discounted prices, `[50,100,150]`. This is because the variable `discounted` is declared in the same block as the `return discounted` line
5. There is an error because `i` was declared with `let` in another scope than where it is being referenced and `let` has blockscope
6. There is an error for the same reason as the problem above because `let` was used to define `discountedPrice` and `let` has blockscope and the program is trying to access it in another scope
7. Should print 150 because even though the variable was declared using `let` it is being accessed in the same scope it was declared in.
8. No error occurs and the function return a list of discounted prices, `[50,100,150]`. This is because the variable `discounted` is declared in the same block as the `return discounted` line
9. There is an error in the code and the error occurs at line 11. Becuase `i` was defined with `let`, it has blockscope and we are trying to log `i` outside of the scope it was declared in
10. 3 is printed. This is because the variable `length` is being accessed in the same block as it was declared and we didn't attempt to reassign a new value to it
11. The function will not cause an error and will return a list of discounted prices, `[50,100,150]`. This is because although the variable `discounted` was declared with `const` that just means that the varaible cannot be reassigned. It can still be manipulated so pushing values to the list `discounted` is still very much allowed. <br>
    
12. 
>**A.** `student.name` <br>
**B.** `student["Grad Year"]` <br>
**C.** `student.greeting()` <br>
**D.** `student["Favorite Teacher"].name` <br>
**E.** `student.courseLoad[0]` <br> <br>

13. <br>
>**A.** *32, string.* This is because when adding a string and a number, the number is converted to a string then concatenated to the string. Although `+` is a mathematical operator, it's different than the other ones in that it converts the number to a string instead of the string to a number <br>
**B.** *1, number.* The `-` forces the string to convert to a number and then evaluates the expression. <br>
**C.** *0, number.* The `+` forces the `null` to convert to `0` and then the expression is evaluated. <br>
**D.** *3null, string.* The `+` forces the `null` to convert into an equivalent string and then is concatented to the end of '3'. <br>
**E.** *4, number.* The `true` is converted to `1` and then the expression is evaluated. <br>
**F.** *0, number.* Both the `false` and `null` are converted to `0` and then are added. <br>
**G.** *'3undefined, string'.* The `undefined` is converted into a string and then concatenated to the end of '3'. <br>
**H.** *NaN, number*. The `-` sign forces both the 3 and the `undefined` to be converted into numbers but the `undefined` is converted into `NaN` so when the expression is carried out, the final value is `NaN`. <br><br>

14. <br>
>**A.** *TRUE*, in comaprisons all values involved are converted to numbers so 2>1 is true <br>
**B.** *FALSE*, for the same reason as above 2<12 <br>
**C.** *TRUE*, for the same reason above 2=2 <br>
**D.** *FALSE*, `===` is a strict equality check which means that both the type and the value must be the same. Since the types are different, this is false <br>
**E.** *FALSE*, true is converted to `1` which is not equal to 2 <br>
**F.** *TRUE*, because even though a strict equality check is used the type of `Boolean(2)` is a boolean, same as `true`, and `Boolean(2) = true` <br><br>

15. The difference between `==` and `===` is that the former converts all the operands involved into numbers (except for some very special cases involving `null` and `undefined`) before then carrying out the comparison. The latter does not do type conversion before carrying out the comparison. This means that if you use `===` to compare values of different types, the result will always be false. However, if you use `==` to compare values of different types, it is not necessarily false.
16. In separate JS file
17. The function will return an array of `[2,4,6]`. First the array `[1,2,3]` is passed in to `modifyArray`. There is a for loop that iterates over all the elements in `[1,2,3]` and calls the function `doSomething` on each element and then pushing the modified element to `newArr`. Then `newArr` becomes `[2,4,6]` at the end and is returned.
18. In separate JS file
19. 1 4 3 2 is printed because the 2 is set to be printed 1000 ms after it is called, the 3 is set to be printed 0 ms after its cxalled which is still slower than the 1 and the 4.