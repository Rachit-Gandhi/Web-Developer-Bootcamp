# Javascript Basics

# Javascript Strings
* Topics Covered: Strings Basics, Indices and Length, Undefined & Null, String Methods, String Template Literals, Random Numbers and the Math Object*

Number Boolean already seen, String - series of characters
->stringVariable
```
let firstName = "Unknownanony";
let dialogueActor1 = 'He said, "Move Slowly and Carefully in the darkness!"'
```
-> Indices and length
Strings are indexed
```
let animal = "Dumbo Octopus"
animal[0]
animal.length
"lol" + " " + "lol"
```
Can't update a particular index of the string seperately, assign a new string works

-> String Methods
built in actions we can take for each individual strings
```thing.Method()```
1. toUpperCase() Non-destructive, copy of original
2. trim() remove white space at beginning and end, non-destructive too
```thing.Method1().Method2()``` 
Chain methods
-> ->with arguments
```thing.Method(args)```
1. indexOf(): first occurance of the given literal
2. slice(beginIndex[, endIndex]); endIndex is optional
3. replace('arg1', 'arg2'); Only first occurance
4. replaceAll: Not for all browsers
5. repeat(int); repeats the string int times

->String Tempelate Literals
```
`I counted ${3 + 4} sheep`;
```

->Undefined and Null
Null - intentional absence of any value - Must be assigned - lack of value, needs to be set
Undefined - Variables that do not have an assigned value are undefined- js saying idk

-> Random numbers and the math object
Math Object: Contains properties and methods for mathematical constants and functions
```
Math.PI
Math.round(4.9) //5
Math.abs(-456) //456
Math.pow(2,5) //32
Math.floor(3.9999) //3
Math.ceil(34.01) //35
Math.random() //(0,1)
Math.floor(Math.random()*10) // 1-10
```
Math is an object, a collection of methods and properties which we always have access to 

# Javascript Decision Making
*Topics covered: Comparison Operators, Running js from a file, Conditional If, Else-If and Else, Truthy and False-y values, Logical AND/OR/NOT

-> Decision Making in Javascript: Branching paths
Comparison Operators: >,<,==,!=,===,!==,<=,>=
All of these return a boolean, even strings can be compared, but be careful, there is ascii code comparison

```
== //check equality of value, invariant of types, like not just numeric 1 and '1'
0 == false
null == undefined;
=== //

!= // == analogous
!== // === analogous
```
-> console.log("hello")
console is also object, .warn, .error
```
alert("hi there")
let userInput = prompt("Please enter a number")
parseInt(userInput)
userInput + 1
parseInt(101akshfoi) //101
```
-> js files //check Running_js.... folder
-> Conditional Statements
```
if(rating ==== 3){
    console.log("You are a student")
}
```
```
num = userInput("Enter a number: ")

if (numm % 4 === 0) {
    console.log("Here is a number divisible by 4");
} else if (num % 2 === 0) {
    console.log("Here is a number divisible by 2");
}
else{
    console.log("WHY DID YOU GIVE THIS NUMBER");
}
```

->Truthy and Falsey values
All js values have an inherent truthyness and falsyness, Falsy values: false, 0, "", null, undefined, NaN, Everything else is truthy

->Logical Operators
AND/OR/NOT
```
true && true
true || false
0 || undefined // false
!null
```
-> Switch statement
```
const day = 2;
switch(day) {
    case 1:
        console.log("Monday");
        break;
    case 2:
        console.log("Tuesday");
        break;
    case 3:
        console.log("Wednesday");
        break;
    case 4:
        console.log("Thursday");
        break;
    case 5:
        console.log("Frday");
        break;
    case 6:
    case 7:
        console.log("Weekend!");  
        break;
    default:
        console.log("We don't know");
}
```