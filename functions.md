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
``````

2. Function asignment/unnamde function/ananymous function 
- Function is declared without name it's just assign as a varible
- The function doesn't get hoisted

**Example :-**
``````
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
**2. What is closure ? **
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


