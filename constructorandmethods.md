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

map(item)
- It is iterate the array value and return new array

**Example :-**
````````````
var arr = [ 9,1, 2, 3, "6", "8",11,18,90,70,"80","70"];
var arr2 = arr.map((item) => (item))
console.log(arr2)
````````````
**pseudo code of map**
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



