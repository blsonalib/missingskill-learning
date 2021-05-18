**1. What is function ?**
- Function is a block, design to perform a perticular task (reusable).
- Functions are object the typeof function is function.
- Function is first citizen it means we can use function as a variable, parameter etc.(propeties).
- we can use the function in two ways:

1. Function declaration/named function   
- Function is declared by using name.
- The function get hoisted.

**Example :-**
```````
fn();                //function get hoisted
function fn() {
console.log("Hi")
}
Example 2:
const location = {
name: "Nagpur",
pincode:123456
}
function getLocation(param) {
const localP = {
name: param.name,                  //get the object from location
pincode:param.pincode
}
localP.name = "Mumbai",
localP.pincode = "199898"
console.log( localP)                 //{ name: 'Mumbai', pincode: '199898' }
}
getLocation(location)
console.log( location)                //{ name: 'Nagpur', pincode: 123456 }
````````

2. Function asignment/unnamde function/ananymous function 
- Function is declared without name it's just assign as a varible
- The function doesn't get hoisted

**Example :-**
``````````
const counter = (function (para) {
return function (step) {
let count = para;
return function (last) {
count = count + step
return function () {
var final = count + last;
last = last + count;
return {
count: final,
last:last
}
}
}
}
})(10)
console.log(counter(4)(2)())    //{ count: 16, last: 16 }
console.log(counter(4)(4)())    //{ count: 18, last: 18 }
console.log(counter(4)(6)())     //{ count: 20, last: 20 }
```````````
**2. What is closure ?**
- The inner function can use the scope of parent variable. (nested function).

**Example 1:**
`````````````
const counter = (function (para,step) {
var count = step;
return function () {
count = count + para
return count;
}
})(10,2)()
console.log(counter) //12
Example 2:

var a=(function(para){
return function(){
return para;                //closure
}
})(10)()    //short circuit or function chaining or currying  IIEF
`````````````

**3. Immediately Invoked Function Expression(IIEF)**

- It is invoked immediately (Encapsulation)

**Example :-**
``````````````
; (function outerFn(p1) {
return function (p1) {
return function (p2) {    //local scope
return function (p1) {
let sum = p1 + p1+ p2 + p2;
console.log(sum)        //220
return sum
}
}
}
})(20)(30)(50)(60)
`````````````````

**4. Spread operator (...)**
- If we want something change in already defined object that time without writting  this object again and again we use spread operator it is introduced in ES6.

**Example :-**
``````````````````
function getLocation(param) {
return localP = {
...param,                                              //by using spread operator we can get hole object
places:[...param.places,"Zilpi"]
}
}
getLocation(location)
console.log(location)              //{    name: 'Nagpur',pincode: 123456,places: [ 'Burdi', 'Hingna', 'Futala' ]}
console.log(localP)                 //{    name: 'Nagpur',pincode: 123456,places: [ 'Burdi', 'Hingna', 'Futala', 'Zilpi' ]}
```````````````````
**5. Higher order function**
- Higher order function function pass the function as a parameter is called as higher order function.

**Example :-**
```````````````````
; (function outerFn(p1) {
return function (p2) {
return function (p3) {
return function (cp) {
const sum =cp(p2 + p3) ;
return p1(sum);
}
}
}
})(function (print) {
console.log("print=>", print)
})(30)(50)(function (para) {
return para;
});
```````````````````
**6. Pure function**
- Pure function take the same parameter and return the same output  they do not perform any other task inside  the function

**Example :-**

```````````````````
const fun =(para)=>{
return para
}
fun(para)    //pure function
const fun =(para)=>{
return para+10+20;
}
fun(para)    //not pure function

`````````````````````
**7. Arrow function**
- Arrow functions allow us to write shorter function syntax it is introduced in ES6 It doesn't hoisted

**Example 1:-**
`````````````````````
const main=()=>{
console.log("Hi");
}
main();
Example 2:
; (outerFn=(p1)=> (p2) => (p3) =>(p4)=> (cp) => p1(cp(p2+p3+p4))
)(function (print) {
console.log("print=>", print)       //90
})(30)(50)(10)(function (para) {
return para;
});
`````````````````````
**8. Inline function**
- An inline function is a javascript function, which is assigned to a variable created at runtime.

**Example :-**
`````````````````````
const main=(val)=>{     //parameter
console.log( val);
}
main("Welcome Nagpur");    //pass the argument
```````````````````````






