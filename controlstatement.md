**1. Control statement**
- control statement allows us to decide which statement want to execute
1. if else
  - If the condition is true then execute if statement.
  - If the condition is false then execute else statement.
2. switch
  - The switch statement executes a block of code depending on different cases.
  - It executes the block of code according to the input we give.

> we can use to check the condition in 3 ways such as using if else , ternary operator and logical operators

**Example 1:-**
- By using if else

```````
var a ="sona" 
if (a){  console.log("Hello sona wellcome")  //Hello sona wellcome
  } else{ 
     console.log("!Sorry your not sona") 
}
```````
**Example 2:-**
- By using ternary operator 
`````````

var a ="sona" 
var res = a ? "Hello sona wellcome" : "!Sorry your not sona"; console.log(res) //Hello sona wellcome
```````````
**Example 4 :-**

- By using logical operator
````````````
 var a = "sona"; 
 var res = a && "Hello sona wellcome" || "!Sorry your not sona"; console.log(res) //Hello sona wellcome
 ````````````
**Example :-**
- switch case statement
```````````````
const result = () => {
   let percent = 90;
      switch (percent) {
        case 65:
            console.log("A divison")
            break;
       case 70:
            console.log("Excellent")
            break
        case 90:
            console.log("Merit List")
            break
    }
}
result()
```````````````

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
