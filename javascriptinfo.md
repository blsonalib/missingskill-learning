**1. What is javascript ?**
- JavaScript is programming language for web and server (nodejs).
- With the help of javascript the application is alive.

**2. History of JavaScript**
- In 1995, a Netscape programmer named Brandan
- Developed a new scripting language withing 2 week .
- It was named Mocha, but quickly became known as LiveScript and, later JavaScript
- Donated to ECMA to create a standard implementation
- New Js based on ECMAScript
- Javascript = Java + Live Script

**3. Browsers**
1. Chrome - v8 Ebngine - node js
2. Brave
3. Firefox
4. Edge
5. Opera
6. Safari

**3. There are four pillers of javascript**
1. Variables
2. Function
3. Object
4. Array


**4. Browser object**
- window or this is the browser object(parent)
- some browser objects are :
**1. location**
- It is use to check current location  (url,port etc)

**Example :-**
``````
location.reload()- to reload the page
```````

**2. Events**
- It is used to perform different different events operations(actions).


**3. localStorage (methods setItem() and getItem())**

**Example :-**
```````
//store Data
var obj = { name: "sona", city: "Nagpur" };
var myJsonData = JSON.stringify(obj);
localStorage.setItem("Item", myJsonData);


// Retrive data:
data = localStorage.getItem("Item");
obj = JSON.parse(data);
```````
**4. alert**

**Example :-**
```````
alert("Hello");   //pop up Hello
```````

**5. moment**
- It is the libary used for date

**Example :-**
```````
moment().format('MMMM Do YYYY, h:mm:ss a');
moment().format('dddd');  
moment().format("MMM Do YY");   
```````
**6. Json**
- When exchanging data between a browser and a server and the data can only be text.(Javscript Object Notation)
There are two main methods:

**1.stringify()**
- It is to send data from web to server.

**Example :-**
``````````
var obj = { name: "sona", city: "Nagpur" };
var myJsonData = JSON.stringify(obj);
``````````
**2. parse()**
- It is used to recieve data from server in json format

**Example :-**
``````````
var myJsonData = JSON.stringify('{ name: "sona", city: "Nagpur"}');
``````````

**7. Gotcha**
1. If we doing addition of two number and second number is string then this string convert into a number used + operator before that operant

**Example :-**
``````````
var a=2;
var b="5";
var c= a+(+b)
``````````

2. In Object if a key has space the used barcket notation

**Example :-**
``````````
let biodata = {
full name:"sona"
}
let res = biodata["full name"]
``````````

3. Array are nothing but object but referenced with index value.

**Example:-**
``````````
let biodata = {
fullname:"sona",
friend : ["shweta","mona","arti"]
}
const res =biodata.friend["hi"] = "Kumud"
console.log(biodata)                        //{ fullname: 'sona', friend: [ 'shweta', 'mona', 'arti', hi: 'Kumud' ] }
``````````

**8. Tech debts**
1. It is act as a concat method if we used two number 1 number is string and another is number type the + sign act as a concat

**Example :- **
``````````
var a = "6";
var b= 20;
var c= a+b  => 620  rather than 26
``````````

2. null 
- null datatype is object but is does not work like object

**Example :-**
``````````
var a=null;
typeOf a   //object
``````````

3. ===
**Note:** 
- If we used == it is used to check only number is same
- If we used === it is used to check datatype

**Example :-**
``````````
var name = "sona"
var myName= "sona"
if(name===myName){
    console.log("true");
}else{
    console.log("false");
}
``````````






