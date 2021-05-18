**1. What is constructor ?**
- contructor is used to initilize the instance (object)
- By using new keyword we create the instance (object)

1. Class is blueprint (ES6)
2. With the help of prototype property we can add new property into the object
3. Method is nothing but the behaviour of function
4. this is keyword refers to the "owner" of the function. with the help of this keyword we can access on property of this class or function
in normal function this keyword act as a global to avoid this issue flate arrow function came.


**2. Constructor Methods**
1. String
2. Array
3. object

**1. String Constructor**
- String is a string constructor when we want to use string method the primitive string converted into string constructor(object)

**Example :-**  
`````
 var str = new String("my name is Sona");
           str.split(" ")   => here . is used to convert into object
`````
**- String Methods**
**1.split(delimeter)  **
- it is used to split the string into delimeter.
**Example :-**
```````
var str = new String("My name is Sona");
var str2=str.split(" ");
console.log(str2)                     //[ 'My', 'name', 'is', 'Sona' ]
```````

**2. toLowerCase()**
- it is used to convert the string in lower case

**Example :-**
`````````
var str = new String("My name is Sona");
var str2 = str.toLowerCase();
console.log(str2)     //my name is sona
``````````

**3. toUpperCase()**

- it is used to convert the string in upper case .

**Example :-**
```````````
var str = new String("My name is Sona");
var str2 = str.toUpperCase();
console.log(str2)     //MY NAME IS SONA
````````````

**4. trim()**
- it is used remove the white space from both the side of string

**Example :-**
````````````
var str = new String("           My name is Sona          ");
var str2 = str.trim()
console.log(str2)     //My name is Sona     =>   remove the whitespace
````````````

**5. length**
- length is property used to check how many char present in the string

**Example :-**
````````````
var str = new String("My name is Sona");
var str2 = str.length
console.log(str2)     //15
````````````

**6. replace(src,tag)**
- it is used to replace the string what we want to replace and it repalce only frist string and it is case sensitive

**Example :-**
````````````
var str = new String("My name is sona");
var str2 = str.replace("s","C");
console.log(str2)     //My name iC sona     => case sensitive
````````````


**2. Array Constructor**

- Array is constructor with the help of Array constructor we can use array methods.
**- Array Methods**



**1. isArray**
- It is check the value is array or not

**Example :-**
````````````
const arr = [{}, [], "Hi", 2, 4, 6, "6", { name: "sonali" },null,""];
const arr2 = arr.filter((item) => {
return !!item && typeof item === "object" && !Array.isArray(item)                      // [{}, { name: 'sonali' }]
})
console.log(arr2);
````````````

**2. length** 
- It is a property of array to check the last value of idex value of an array  eg . arr.length-1 (it is used to check last index   value of an array)
**Example :-**

````````````
var arr = [1, 2, 3, "6", "8"];
var arr2 = arr.length;
console.log(arr2)           //5
````````````

**3. join(delimeter)**
 - It is used delimeter and convert array to string
 
**Example :-**
````````````
var arr = [1, 2, 3, "6", "8"];
var arr2 = arr.join("")
console.log(arr2)           //1236*8
````````````

**4. map(item)**
- It is iterate the array value and return new array

**Example :-**
````````````
var arr = [ 9,1, 2, 3, "6", "8",11,18,90,70,"80","70"];
var arr2 = arr.map((item) => (item))
console.log(arr2)
````````````
**psudo code of map**
`````````````
const map = (arr,cb) => {
let length = arr.length;
const localArr = [];
for (var i = 0; i < length; i++){
const item = arr[i]
const res = cb(item,i);
localArr.push(res)
}
return localArr;
}

const final = map([1, 2, null, undefined, "hi", "9", 8], function (item, index) {
console.log("final","item :","\n\n",item,"Index :",index)
return item;
})
console.log(final)
`````````````


**5. forEach(item)**
- It is iterate ther array value

**Example :-**
`````````````
var arr = [ 9,1, 2, 3, "6", "8",11,18,90,70,"80","70"];
arr.forEach((item) => (item))
console.log(arr)               // [ 9,1, 2, 3, "6", "8",11,18,90,70,"80","70"];
`````````````
**psudo code of forEach**
`````````````
const forEach = (arr, cb) => {
let localArr = [];
const length = arr.length;
for (var i = 0; i < length; i++){
const item = arr[i]
}
return localArr;
}
const final= forEach([1, 2, 3, 4,"Hi"], function (item,index) {
console.log(item,index)
});
console.log(final)
`````````````

**6. includes()**
- It is used to check the key(index) present in array or not if it is present gives true  otherwise gives false (ES6)

**Example :-**
`````````````
var arr = [ 9,1, 2, 3, "6", "8",11,18,90,70,"80","70"];
var arr2 = arr.includes(9)
console.log(arr2)     //true
`````````````
**psudo code of includes**
`````````````
let foundIndex = false;
for (var i = 0; i < arr.length; i++){
    const item = arr[i]
    // console.log(item);
    if (item === value) {
        foundIndex = true
        // console.log(foundIndex)
        break;
    }

}

return foundIndex;
}
const final = includes([1, 2, 4,"999"],999)
console.log(final)
`````````````

**7. indexOf()**
-  It is used to check the key(index) present in array or not if it is present gives index value otherwise gives -1

**Example :-**
`````````````
var arr = [ 9,1, 2, 3, "6", "8",11,18,90,70,"80","70"];
var arr2 = arr.indexOf(9)
console.log(arr2)     //0
`````````````
**psudo code of indexOf**
`````````````
const indexOf = (arr,value) => {
let foundIndex = -1;
for (var i = 0; i < arr.length; i++){
    const item = arr[i]
    // console.log(item);
    if (item === value) {
        foundIndex = i
        // console.log(foundIndex)
        break;
    }

}

return foundIndex;
}

const final = indexOf([1, 2, 4], 2)
console.log(final)
`````````````
8. filter(item)
 -  It is used to filter the value
 
**Example :-**
`````````````
var arr = [ 9,1, 2, 3, "6", "8",11,18,90,70,"80","70"];
var arr2 = arr.filter((item) =>
item>9 && typeof item === "number"
)
console.log(arr2)  //[ 11, 18, 90, 70 ]
`````````````
**psudo code of filter**
`````````````
const filter = (arr,cb) => {
let length = arr.length;
const localArr = [];
for (var i = 0; i < length; i++){
const item = arr[i]
const re8s = cb(item);
if (res) {
// console.log( res)
localArr.push(item)
    }
}
return localArr
}
const final = filter([1, 2, null, undefined, "hi", "9", 8], function (item) {
return !!item;
})
console.log(final)
`````````````

**9. concat(arr2)**
- It is used to add two or more arrays

**Example :-**
`````````````
var arr = [ 9,1, 2, 3];
var arr2 = [6, 9, 2]
var arr3=arr.concat(arr2)
console.log(arr3)  //[ 9,1, 2, 3, 6, 9, 2];
`````````````

**10. push(index)**
- It is add the value in end of an array
**Example :-**
`````````````
var arr = [1, 2, 3, "6", "8"];
arr.push(9)
console.log(arr)      //[ 1, 2, 3, '6', '8', 9 ]
`````````````

 **psudo code of push**
`````````````
const push=(arr,value)=>{
let length = arr.length;
arr[length] = value;
return arr
}

let arr = [1, 5, 8, "hi"];
arr = push(arr, "hello");
console.log(arr)
`````````````

**11. pop() ** 
-  It is remove the value in end of an array

**Example :-**
`````````````
var arr = [1, 2, 3, "6", "8",9];
arr.pop(9)
console.log(arr)      //[ 1, 2, 3, '6', '8']
`````````````

**12. unshift(index)**
-  It is add the value in begining of an array
**Example :-**
`````````````
var arr = [1, 2, 3, "6", "8"];
arr.unshift(9)
console.log(arr)      //[ 9 ,1, 2, 3, '6', '8']
`````````````

**13. shift ()**
- It is remove the value in begining of the array

**Example :-**
`````````````
var arr = [9,1, 2, 3, "6", "8"];
arr.shift(9)
console.log(arr)      //[ 1, 2, 3, '6', '8']
`````````````


**3. Object Conctructor**
- We can use object method by using Object constructor
object methods
- 1. values
- 2. keys



**3. this keyword**
- It is window (browser object)  with the help of this we can get  current function, class and object
when we use normal function it is act as a window object and arrow function solve this problem.

**Example :-**
`````````````````
function Bank (name,branch) {
this.name = name;
this.branch = branch;      //this keyword only get the data from this function
this.getDetails = function () {
return  this.name +" "+ this.branch
}
function fn() {            //global value   to avoid this tech dept using arrow function
return this.name
}
}
// let details = Bank.prototype.Axis
let Axis = new Bank("Axis", "Nagpur")   // this new keyword used to create the instant (object) of this function of Bank
let Sbi = new Bank("sbi", "Pune")
let HDFC = new Bank("HDFC", "Mumbai")
let BOM = new Bank("BOM", "Nagpur")
console.log(Axis.fn)
```````````````````````````


