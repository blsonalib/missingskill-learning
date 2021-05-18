**1. Controlled statement**
- if else
- switch


> we can use to check the condition in 3 ways such as using if else , ternary operator and logical operators

**Example 1:-**
```````
- By using if else 
var a ="sona" 
if (a){  console.log("Hello sona wellcome")  //Hello sona wellcome
  } else{ 
     console.log("!Sorry your not sona") 
}
```````
**Example 2:-**
`````````
- By using ternary operator 
var a ="sona" 
var res = a ? "Hello sona wellcome" : "!Sorry your not sona"; console.log(res) //Hello sona wellcome
```````````
**Example 4 :-**

- By using logical operator
````````````
 var a = "sona"; 
 var res = a && "Hello sona wellcome" || "!Sorry your not sona"; console.log(res) //Hello sona wellcome
 ````````````
**2. Truthy and Falsy value**
- Falsy values - "", null, undefined, 0, false, NaN
- Truthy Values - non primitive are always truthy , rather than falsy all are truthy
we have to check any value is true or false to convert into boolean by using !! logical operation it gives true or false result only

**Example :-**
`````````````````
var a = {}; console.log(a) //{}
``````````````````
- converted to booleans 
````````````````````
var a = {}; console.log(!!a) //true
````````````````````````
