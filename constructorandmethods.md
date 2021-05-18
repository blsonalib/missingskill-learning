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

1. String Constructor
- String is a string constructor when we want to use string method the primitive string converted into string constructor(object)

**Example :-**  
`````
 var str = new String("my name is Sona");
           str.split(" ")   => here . is used to convert into object
`````
**- String Methods**
- split(delimeter)  
    - it is used to split the string into delimeter
**Example :-**
```````
var str = new String("My name is Sona");
var str2=str.split(" ");
console.log(str2)                     //[ 'My', 'name', 'is', 'Sona' ]
```````

- toLowerCase() 
    - it is used to convert the string in lower case
**Example :-**
`````````
var str = new String("My name is Sona");
var str2 = str.toLowerCase();
console.log(str2)     //my name is sona
``````````

- toUpperCase() 
    - it is used to convert the string in upper case .
**Example :-**
```````````
var str = new String("My name is Sona");
var str2 = str.toUpperCase();
console.log(str2)     //MY NAME IS SONA
````````````

- trim() 
    - it is used remove the white space from both the side of string
**Example :-**
````````````
var str = new String("           My name is Sona          ");
var str2 = str.trim()
console.log(str2)     //My name is Sona     =>   remove the whitespace
````````````

- length 
    - length is property used to check how many char present in the string
**Example :-**
````````````
var str = new String("My name is Sona");
var str2 = str.length
console.log(str2)     //15
````````````

- replace 
    - it is used to replace the string what we want to replace and it repalce only frist string and it is case sensitive
**Example 6 :-**
````````````
var str = new String("My name is sona");
var str2 = str.replace("s","C");
console.log(str2)     //My name iC sona     => case sensitive
````````````





