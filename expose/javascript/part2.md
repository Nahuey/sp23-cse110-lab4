# Part 2. A Little More of a Challenge...
1. Since i is a var, it will be in the scope throughout the function. Line 12 will output 3 because the for loop ends after the length of prices which is 3.
2. At line 13, the output will be 150. Since discountedPrice is a var, its scope is throughout the function. At the last iteration of the for loop, discountedPrice would be 150 because 300 * 0.5 is 150.
3. At line 14, the output will be 150. Since finalPrice is a var, its scope is throughout the function. At the last iteration of the for loop, finalPrices = (150 * 100)/100 = 150. After this iteration, it would break out of the for loop and go to line 14 where finalPrice was set to be 150.
4. The function will return [50,100,150]. This is what is stored inside the variable discounted. In for loop, the finalPrice is pushed into the discounted array. So each time the loop iterates, it will basically multiply the elements of the original array by 0.5 then push it to the discounted array. This will result in the array [50,100,150] being returned.
5. There will be an error at line 12. i uses the let keyword this means it is only defined within the for loop. Since line 12 is outside of the for loop, i is outside the scope which will result in an error.
6. There will be an error at line 13. discountedPrice uses the let keyword that is defined within the for loop. Once the loop ends, discountedPrice is no longer defined resulting in an error at line 13.
7. At line 14, the output will be 150. finalPrice is a let defined to be 0 at the beginning of the function. This means its scope is throughout the function. At the last iteration of the for loop, finalPrice = (150 * 100) / 100 = 150. Then the loop ends, so finalPrice is defined to be 150.
8. The function will return [50,100,150] because discounted uses the keyword let, so its scope is throughout the function. In the loop, we calculate finalPrice and push it into the array discounted. After the for loop is executed, we return the discounted array which is [50,100,150].
9. There will be an error at line 11. i uses the let keyword  this means it is only defined within the for loop. Since line 11 is outside of the for loop, i is outside the scope which will result in an error.
10. At line 12, the output will be 3. length uses the const keyword and is defined to be prices.length which is the length of the input array. The array length is 3 so length = 3. The variable length isn't used anywhere else in the function except for line 12, so the output is 3.
11. The function will return [50,100,150]. We are able to return an array because discounted was set to be an empty array. Even though discounted uses the keyword const, we aren't trying to re-assign it anywhere in the function so there is no error. We run through the for loop and push each element multipled by (1 - discount), then we push that value to the discounted array. After the loop is executed, we return the discounted array which is [50,100,150].
12. A. student.name <br>
    B. student["Grad year"] <br>
    C. student.greeting() <br>
    D. student['Favorite Teacher'].name <br>
    E. student.courseLoad[0] <br>
13. A. '3' + 2 = '32' because '3' is a string and 2 is an integer so the + would concatenate them together making '32' <br>
    B. '3' - 2 = 1 because the '3' is converted into the integer 3, so 3 - 2 = 1. <br>
    C. 3 + null = 3 because null is converted to the integer 0, so 3 + 0 = 3. <br>
    D. '3' + null = '3null' because null is converted to the string 'null', so the 3 is concatentated with 'null' resulting in '3null'. <br>
    E. true + 3 = 4 because the true is converted to the integer 1, so 1 + 3 = 4.
    F. false + null = 0 because false is converted to the integer 0 and null is converted to the integer 0, so 0 + 0 = 0. <br>
    G. '3' + undefined = '3undefined' because undefined is converted to the string 'undefined', so the 3 and undefined are concatenated to be '3undefined'. <br>
    H. '3' - undefined = NaN because '3' is converted to be the integer 3 and undefined is not an integer, so the result would be NaN.<br>
14. A. '2' > 1 would evalute to true because '2' is converted to the integer 2, so 2 > 1 is true. <br>
    B. '2' < '12 would evalute to be false because since '2' and '12' are both strings, they would be compared by each char. So it would first compare '2' < '1'. Since the '1' comes before '2' in lexicographical order, the result is false. <br>
    C. 2 == '2' would evaluate to true. The '2' would be converted to an integer 2. So now it is 2 == 2, which is true. <br>
    D. 2 === '2' would evaluate to false because 2 is an integer while '2' is a string. Since they are different types, 2 === '2' would be false. <br>
    E. true == 2 would evalute to false because true would be converted to the integer 1. So, 1 == 2 is false. <br>
    F. true === Boolean(2) would evaluate to true because Boolean(2) is true, so true === true would evalute to true.
15. The difference between == and === operators is that == uses type conversions if needed during the comparison. The === operator doesn't use type conversions so if the types are different it will automatically evaluate to false.
16. In part2-question16.js
17. The result of the function, modifyArray([1,2,3], doSomething), is the array [2,4,6]. Within modifyArray, there is a for loop that takes in each element in the input array and uses the callback function on each of the elements. The function doSomething multiples each input by 2. So for each element in the input array, the element is multiplied by 2 then pushed to a new array. The return of the function is the new array containing [2,4,6].
18. In part2-question18.js
19. The output of the code would be 1,4,3,2 in that order.