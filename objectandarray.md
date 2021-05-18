 **1. What is Object ?**
- Object is a call by reference 
- In javascript everything is object (eg. object is a real time intity real life example a dog is a object he has some properties like color, species,weight,height) 
- Read object by using . or [""] bracket notation , bracket notation is used when the key has space example. location city location city is one key but has space.

**Example 1 :-**
````````
var city = {};
 var b = true; 
 var b = city; 
 console.log(city) //{} console.log(b) //{}
````````
**Example 2 :-**
````````
var city = { name:"nagpur"}; 
var b = city;
 b.station = "Nagpur Jn" 
 console.log(city); //{ name: 'nagpur', station: 'Nagpur Jn' } 
 console.log(b); //{ name: 'nagpur', station: 'Nagpur Jn' }
b.famous = "haldiram";
console.log(b); // { name: 'nagpur', station: 'Nagpur Jn', famous: 'haldiram' }
 console.log(city); // { name: 'nagpur', station: 'Nagpur Jn', famous: 'haldiram' }
````````
**2. What is Array**
- Array is used to store multiple value into a single variable .
- Type of array is object Read by using [] with index value like 0,1,2, and "hi" also because array has type object so index can be work as an object key.

**Example used array and object both together**

**Example :- **
````````
var city={ "Nagpur city": [ 0, 0, [ 0, 0, 0, [ 0, 0, [

               {haldiram:"nagpur"}
            ]
        ]
    ]
]
} var b = city["Nagpur city"][2][3][2][0].haldiram console.log(b)
````````

**Example 1:-**
````````
let fruites = ["mango","banana","lichi"] 
console.log(fruites[1]) //banana
````````
**Example 2 :-**
````````
var city = {
     name: "nagpur",
     stations: {
         nagpuJn: ["burdi"],
         ajani: ["ajani Rail","new Ajani",{"Butibori":"IT Companies"}]
     },
     famous: {
         "haldiram":
             { "food": "samosa" }
     }
};   //references are 6
var res = city.stations.ajani[2].Butibori;
var res2=city.famous.haldiram.food
console.log(res)  //IT Companies
console.log(res2)   //samosa

````````
**Example 3 :-**
````````
function a(){
    return function () {
        return {
            b: [0, [0, 0, {
                c: function () {
                    return function () {
                        return {
                        d:"execute"
                    }
                }
            }}]]
        }
    }
}

const final =a()().b[1][2].c()().d
console.log(final)

````````
