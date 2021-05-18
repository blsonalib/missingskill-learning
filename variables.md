**1. What is variable ?**
- Variable is a container.
- Variables are used to store the data.
**Example:-**
var x=20 here x is a variable which hold the value 20 and it is used to declared by using keyword var
There are 3 keyword in javascript to declare variable.

**2. Datatypes in javascript **
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


**2. Non primitive datatype**
- It is act as an container
- It is copy by reference
- Non primitive we can hold primitive and non primitive data both

object - object ({})
array  - object ([])

**Example :-**
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
