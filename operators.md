**1 What is operators ?**
- operators used to perform operation on operant (value or variables).
- There are some operators used in javascript.

**1. Arrithmatic:-** +,-,/,%,*,<,>,<=,>=,<==,>==

**2. Logical :-** !, &&, ||

**3. Ternary:-** ? , :


**Example 1 :-**

`````
var a = "5";
var b = 5;
if (a === b) {
console.log("It is equal")
} else {
console.log("It is not equal")
}
```````

**Example 2:**
```````
var a=5;
var b=5;
consol.log(a+b)   o/p <!--  5 >

var a ="sona"
var res = a ? "Hello sona wellcome" : "!Sorry your not sona";
console.log(res)  //Hello sona wellcome

var a = "sona";
var res = a && "Hello sona wellcome" || "!Sorry your not sona";
console.log(res)    //Hello sona wellcome
``````````



<!-- primitive datatype , call by value or copy by value -->

**Example 1:-**
````````
var a = 50;
var b = a;
console.log(b); //50
console.log(a); //50
```````````

**Example 2:-**
````````
var a = 50;
var b = a;
b = 30;
console.log(b); //30
console.log(a); //50
`````````


**Example 3:-**
`````````
var a = 50;
var b = a;
b = 30;
a = 100;
console.log(b); //30
console.log(a); //100
``````````

**Example 4:-**
```````````
var a = 50;
var b = a;
var c = b;
c = 100;
a = 500;
console.log(a);  //500
console.log(b); //50
console.log(c); //100
````````````

<!-- non primitive call by reference -->
**Example 1:-**
```````````
var city = {};
var b = true;
var b = city;
console.log(city)  //{}
console.log(b)  //{}
`````````````

**Example 2:-**
``````````````
var city = {};
var b = true;
var b = city;
var b = 80;
console.log(city)  //{}
console.log(b)  //80
````````````````

**Example 3:-**
`````````````````
var city = { name:"nagpur"};
var b = city;
b.station = "Nagpur Jn"
console.log(city); //{ name: 'nagpur', station: 'Nagpur Jn' }
console.log(b);     //{ name: 'nagpur', station: 'Nagpur Jn' }
b.station = "ajani"
console.log(b)    // { name: 'nagpur', station: 'ajani'}
console.log(city)    // { name: 'nagpur', station: 'ajani' }
`````````````````````




