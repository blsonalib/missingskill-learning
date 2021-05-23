# 1. What is CSS ?
- CSS stands for Cascading Style Sheet.
- CSS used to style HTML file

# 2. How to use CSS in HTML ?
- We can use CSS in HTML file in three ways:
- 1. Linking external Css document by using ```<link>``` tag
- 2. Using ```<style>``` tag
- 3. Using inline CSS. only style this tag content.

# 3. List the CSS selectors
| Selector   | Example   | Description            |
| ---------- | --------- |-------------------------|
| # (id)     | #main     |Select the element with id = main It is unique|
|.(class)    | .data     |Select all the element with class=data|
|*           | *body     |Selects all element it is called universal selector |
|div         |div        |Selects all ```<div>```  element |
|div,p,h1    |div,p,h1    |Selects all ```<div>``` ,```<p>``` and ```<h1>``` element |
|div .class  |div .data   |Selects only ```<div>``` element which has class=data |


**Example :-**
```````
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Input form</title>
</head>
<style>
    label,input,button{
        padding: 0.2rem;
        margin: 1rem;
    }
   
</style>
<body>
 <label>Email: <input type="email" placeholder="enter your email"></label><br>
 <label>password: <input type="password" placeholder="enter your password"></label><br>
 <label>Message:<textarea rows="4" cols="50" maxlength="200">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ex, quo!</textarea></label><br>
 <button>submit</button>
</body>
</html>
```````

# 4. CSS Properties

**1. CSS Margins**
- It is used to create a space outside the border

**Example:-**
```````
margin : 4rem;   (top, right,bottom,left)
margin-bottom : 4rem 2rem; (top and bottom 4rem right and left 2rem)
margin-left : 4rem;
margin-right : 4rem;
margin-top : 4rem;
margin-bottom : 4rem;
```````

**2. CSS Padding**
- It is used to create a space inside the border 

**Example:-**
```````
padding : 4rem;   (top, right,bottom,left)
padding-bottom : 4rem 2rem; (top and bottom 4rem right and left 2rem)
padding-left : 4rem;
padding-right : 4rem;
padding-top : 4rem;
padding-bottom : 4rem;
```````
**3. CSS Text**
- It is used for text to design 
    - text-align - align/shift the text on center, left and right
 
        **Example:-**
        ```````
        text-align: center;
        text-align: left;
        text-align: right;
        ```````
    - text-decoration- It is used to remove the decoration of the text

        **Example:-**  
        ```````
        text-decoration: none;
        ```````
    - text-transform - It used to convert the text in uppercase, lowercase and capitalize
        
        **Example:-**  
        ```````
        text-transform: uppercase;
        text-transform: lowercase;
        text-transform: capitalize;
        ```````
**4. CSS Font**  
- It is used to style the font of the text
    - font-family - It is used to style the font 

       **Example :-**
        ```````
        font-family: "Times New Roman", Times, serif;
        ```````
    - font-weight- It used to change the font weight

        **Example :-**
        ```````
        font-weight: 500;
        ```````
    - font-size- It is used to change the size of font

        **Example :-**
        ```````
        font-size : 2rem:
         ```````
**4. CSS Border**  
- It is used to create border

**Example :-**
 ```````
 border: 2px solid blue;
 border: 2px dotted blue;       
```````  
  
**5. CSS Display**  
- It is used to display the element (block to inline /inline to block)

**Example :-**
 ```````
   display:block;
   display:inline;
   display:inline-block;
   display:flex;     
```````    
**6. CSS Background**  
- It is used to add background  effect for element.

**Example :-**
 ```````
 background-color: red;          
 background-image:url("Image-url")       
```````  
**7. CSS Color**  
- It is used for the color .

**Example:-**
``````` 
color:red;     //used to change the text color
``````` 
