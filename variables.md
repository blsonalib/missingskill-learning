**1. What is variable ?**
 - Variable is a container.
 - Variables are used to store the data.
**Example:-**
var x=20 here x is a variable which hold the value 20 and it is used to declared by using keyword var
There are 3 keyword in javascript to declare variable.

**2. Variable Declaration**
- Variable declared by:
      - var (ES5)
      - let  (ES6)
      - const (ES6)

**3. Difference between var, let and const**

|Sr No.| var                    | let    |   const  |
|----  | -----------------------| ------ |-------|
|1.   | It is introduced in ES5 |It is introduced in ES6     |  It is introduced in ES6    |
|2.   | It's get hoisted        |  It doesn't get hoisted    |It doesn't hoisted       |
|3.   | It has finctional scope | It has lexical/block scope |  It has lexical/block scope    |
|4.   | It can be redeclare and reassign/reinitialize | It's only reassign/reinitialize |  It can't be redeclare and reassign/reinitialize    |
|5.   |It can be first declare after that assign|It can be first declare after that assign|  It declare and assigne at a time|


**Example :-**
- Variable declaration by using var
````````````
var num = 20;
console.log("1", num);  //20
num = 30;
function fuNumber() {
num = 60;                      //only functional scope
console.log("3", num);           //60
var num;                          //get hoisted on top of the function
}
num = 40;
console.log("2", num);  //40
fuNumber();
````````````

**Example :-**
- Variable declaration by using let

````````````````
let num ;
console.log("1", num);   //undefined
num = 30;
function fuNumber() {
console.log("3", num);        //error
function innerFun() {
console.log("5",num)
}
console.log("4", num)
let num = 60;               //let doesnt hoisted
innerFun();
}
console.log("2",num)  //30
fuNumber();
console.log("6", num);
```````````````

**Example :-**
- Variable declaration by using const

````````````````
const num =30;
console.log("1", num);
function fuNumber() {

console.log("3", num);
function innerFun() {
let num = 70;
console.log("5",num)
}
console.log("4", num)
innerFun();
console.log("6",num)
}
console.log("2",num)  //30
fuNumber();
console.log("7", num);
````````````````

**4. Datatypes in javascript **
- Javascript datatypes is use to check variable has hold which type of data.
- typeof method used to check the datatype.
- There are two type of datatype.


1. Primitive datatype
2. Non primitive datatype

**1. Primitive datatype**
- It is copy by value /call by value
**Example:-**
Assingment copy in college.

- number - number
- string - string
- boolean - boolean
- null - object
- undefined - undefined (js engine)
- symbol (ES6)

**Example :-**
```````````````
var a = 20;
var b = "Hello";
var c = true;
var d = undefined;
var e = null;
console.log(typeof a);  //number
console.log(typeof b)   //string
console.log(typeof c);  //boolean
console.log(typeof d)   //undefined
console.log(typeof e)    // object   tech debt
Example 2 : call by value/copy by value
var a = 50;
var b = a;
var c = b;
a = 500;
console.log(a);  //500
console.log(b); //50
console.log(c); //50
b = 60;
console.log(b); //60
console.log(c);   //50
``````````````````

**2. Non primitive datatype**
- It is act as an container
- It is copy by reference
- Non primitive we can hold primitive and non primitive data both
**Example:-**
 Debit cards linked to account

object - object ({})
array  - object ([])

**Example :-**
````````````````````````````
var city={
"Nagpur city": [
0, 0, [
0, 0, 0, [
0, 0,  [
               {haldiram:"nagpur"}
            ]
        ]
    ]
]
}
var res = city["Nagpur city"][2][3][2][0].haldiram
console.log(res)
````````````````````````````
