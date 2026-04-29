1. 3, because the variable i is declared with var and var is function-scoped so i is accessible anywhere inside the function discountPrices. The loop runs 3 times because that's the length of the prices array.
2. 150, discountedPrice is also declared with var, so it is still accessible when the loop ends. That means value is the result of the last iteration of the loop, which is 150=300*(1-0.5)
3. 150, finalPrice is declared with var so it is accessible when the loop ends and the last value it has is rounding 150 to the nearest integer which is 150.
4. [50, 100, 150] The function is populating the array with discounted price of each price and var allows all the variables to accessed and updated throughout the function, the array is returned without an error
5. ReferenceError: i is not defined, because the variable i is declared with let and let is block-scoped it only exists in the for-loop block. Once the loop finishes it no longer exists and trying to access it throws an error.
6. ReferenceError: discountedPrice is not defined, this variable is declared in the for loop using let which means it only exists within the for loop. Once the loop is exited, accessing it will through an error.
7. 150, because finalPrice is declared in the function block it is accessible by the whole function, so exiting the loop doesn't cause it to be inaccessible, only when the function is exited it is destroyed. Therefore the last value assigned to it will be 150.
8. [50, 100, 150] The function is populating the array with discounted price of each price and while it uses let, the discounted array is in the same block as the return call.
9. ReferenceError: i is not defined, because the variable i is declared with let and let is block-scoped it only exists in the for-loop block. Once the loop finishes it no longer exists and trying to access it throws an error.
10. 3, because length is declared as a const meaning it is block-scoped and you can't reassign the value. It is declared in the function block so it is accessible and there is no attempt to reassign it. Therefore it will print the length of the prices array.
11. [50, 100, 150], even though we are pushing values to the array that is declared as a const in javascript you can modify a const array with push(). It only prevents you from reassigning the variable to a different object. the const variable discountedPrice doesn't throw an error because after every iteration it is technically a new variable.
12. DataTypes
    A. student.name
    B. student['Grad Year']
    C. student.greeting()
    D. student['Favorite Teacher'].name
    E. student.courseLoad[0]
13. Arithmetic
    A. '32' The addition operator signals a string concatenation because '3' is a string type so adding 2 causes string concatentation
    B. 1 The - operator only works with numbers so it forces '3' into a number 3.
    C. 3 null is forced to be a 0, so we get 3+0=3
    D. '3null' since '3' is a string type, the + signals string concatenation and null becomes a string type, 'null'.
    E. 4 in numerical conversion true is 1 and since 3 is a number it forces a numerical conversion and we get 1+3=4.
    F. 0 the + causes conversion of false and null to 0's giving 0+0=0
    G. '3undefined' concatenation is caused and undefined becomes a string 'undefined'
    H. NaN the - operator only works with numbers so '3' is forced to the number 3, but since undefined is represented by NaN the result is NaN.
14. Comparison
    A. true, string '2' becomes a number 2
    B. false, when comparing two strings, JavaScript uses lexicographical order and '2' becomes '1' which is lexicographically greater than '12'
    C. true, == forces type conversion from string to a number so '2' becomes the number 2.
    D. false, === checks that the value and type are the same, since one is a number and the other is a string, it returns false
    E. false, == causes true to be interpretted as the number 1 and 1==2 is false.
    F. true, Boolean(2) converts the number 2 to true and true === true are of the same type and value so it returns true
15. difference between == and ===
    1.  == is Loose Equality which means it just checks for the equality of values after preforming type conversion. Meaning if the two variables on each side are different it will try to convert to a common type before comparing
    2.  === is Strict Equality which means it checks for both value and type. It doesn't preform any type conversions, if the types are different then it returns false.
17. [2,4,6]. We call modifyArray([1,2,3],doSomething), so inside modifyArray, the variable callback refers to doSomething function. Inside modifyArray() an empty array newArr is created. In the for loop, when i = 0, we take array[0]=1 and we run the function doSomething(1). This returns 1*2=2 and then back in modifyArray() we push this to newArr. Then i=2 and we do the same thing, array[1]=2 is passed to doSomething(2)=4 and 4 is pushed into newArr. The next iteration, i=2, array[2]=3 is passed to doSomething(2)=6 and 6 is pushed into newArr. The loop finishes because i=3 is not less than 3 and the function returns newArr which is now [2,4,6].
19. output:
1
4
3
2