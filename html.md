**1. What is HTML ?**
- HTML is a Hyper Text Markup Language.
- HTML is used for create the structure of web pages.

**2. HTML Basics**

**```<!DOCTYPE html>```**
- All HTML document must start from ```<!DOCTYPE html>``` It's means we used document type is HTML .


**```<html>```**
- HTML start from ```<html>```  tag itself and end with  ```</html>```. This is parent node of all html tags.

**```head```**
- ```head``` tag is a container for metadata 
- Inside ```head```  tag we can use
1. ```title``` -  ```title```  tag defines the title of the document
2. ```meta``` -  ```meta```  tag used for metadata 
3. ```script``` -  ```script```  tag used to write a javascript
4. ```link``` - ```link```  tag used for relation between current file and external source.

**```<body>```**
- It is visible part of document start with ```<body>``` and end with ```</body>```


**3. Basic HTML Element**
- The HTML element is everything from the start tag to end tag.
- Example: ```<tagname>``` content... ```</tagname>```


**h1,h2,h3,h4,h5,h6**
- This is heading element
- ```<h1>``` is the largest heading and  ```<h6>``` smallest heading

**Example :-**
``````
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>This is first heading.</h1>
    <h2>This is second heading.</h2>
    <h3>This is third heading.</h3>
    <h4>This is fourth heading.</h4>
    <h5>This is fifth heading.</h5>
    <h6>This is sixth heading.</h6>
</body>
</html>
``````

**```<p>```**
- It is block element used for paragraph .
- start with ```<p>``` and end with ```</p>```

**Example :-**
``````
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <p>This is paragraph....</p>
</body>
</html>
``````

**```<div>```**
- ```<div>``` tag defines the section
- It is block element start with ```<div>``` and end with ```</div>```

**Example :-**
``````
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <div>This is division....</div>
</body>
</html>

``````

**```<span>```**
- ```<span>``` tag is inline element used to mark up a part of a text

**Example :-**
``````
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    div{
        display: flex;
    }
    span{
        margin-top: 0.1rem;
    }
</style>
<body>
 <div>
    <input type = "checkbox">
    <span>Terms and conditions</span>
 </div>
</body>
</html>
``````
**```<b>```**
- ```<b>``` tag display the text in bold size.

**```<i>```**
- ```<i>``` tag display the text in italic 

**```<strong>```**
- ```<strong>``` tag indicates that content have strong importance

**Example :-**
``````
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
 <div>
    <p>
        Lorem ipsum <b>dolor</b> sit amet.
    </p>
    <p>
       <i> Lorem ipsum dolor sit amet.</i>
    </p>
    <p><strong>Lorem ipsum dolor sit amet consectetur adipisicing.</strong></p>
 </div>
</body>
</html>
``````
**```img```**
- ```img``` tag used to display image on web page.
- The attributes of ```img``` are : 
1. src 
2. alt
3. height
4. width

**Example :-**
``````
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image</title>
</head>
<body>
<img src="image.jpg" alt="cute dog" width="300px" height="200px">
</body>
</html>
``````


**```<br>```**
- ```<br>``` tag used to break line. This element called empty element. Empety element do not have an end tag. 

**Example :-**
``````
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Paragraph</title>
</head>
<body>
    <div>This is division....</div>
       <p>This is paragraph 1</p><br>
       <p>This is paragraph 2</p><br>
       <p>This is paragraph 3</p>
</body>
</html>

**Example :-**
``````
**```table```**
- ```table``` tag used to create a table
``````
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>

<body>
    <table>
        <tbody>
            <thead>
                <tr>
                    <th>Name</th>
                    <th>Email</th>
                </tr>
            </thead>
            <tr>
                <td>Sonali</td>
                <td>sonali@gmail.com</td>
            </tr>
            <tr>
                <td>Kumud</td>
                <td>kumud@gmail.com</td>
            </tr>
            <tr>
                <td>Priya</td>
                <td>priya@gmail.com</td>
            </tr>
        </tbody>
    </table>
</body>

</html>
``````
**```<header>```**

- ```<header>``` tag specifies the header (navigation) content of the document.
- It is block element.

**```<main>```**

- ```<main>``` tag specifies the main content of the document.
- It can use only once in a document
-  tag must not be descendant ```<article>```,```<section>```,```<aside>```,```<header>```,```<footer>```


**```<article>```**

-  ```<article>```tag specifies the article content of the document.
- It is used for writing articles and blogs on the website.

**```<aside>```**

-  ```<aside>```tag display aside from the content it is placed in.

**```<footer>```**

-  ```<footer>```tag specifies the footer of the document.
**Example :-**

``````
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    main {
        display: flex;
        margin: 2rem;
        padding: 0.8rem;
        text-align: center;
    }
    footer,header{
        background-color: beige;
        border: 2px solid black;
        padding: 0.8rem;
        margin: 0;
        text-align: center;  
    }
    aside{
        width: 50%;
        background-color: powderblue;
        padding: 2rem;
    }
</style>
<body>
    <header>This is navbar</header>
    <main>
        <section>
            The section 1
            <article>
               <p>
                   Lorem ipsum dolor sit, amet consectetur
                    adipisicing elit. Molestiae odio possimus consequuntur quas laudantium ullam nihil dolor consequatur, magnam nulla
               </p>
            </article> 
        </section>
            <section>
                <aside>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia illum
                         laborum commodi ipsa repudiandae quod rem exercitationem
                             eveniet quas reiciendis inventore quisquam!</p>
                </aside> 
            </section>       
    </main>
    <footer>
        <p>This is footer....</p>
    </footer>   
</body>
</html>
``````

**4. HTML List**

- ```<li>``` tag it is used to define the list of items.
- We can list the items in two way 

**1. order list**
    - ```<ol>``` tag used the list the items in order format.

**2. unorder list**     
    - ```<ul>``` tag used the list the items in unorder format.(number, alphabets, roman number etc.)

**Example :-**
``````
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <p1>
        <ol>
            <li>item 1</li>
            <li>item 2</li>
            <li>item 3</li>
        </ol>
        <ul>
            <li>item 1</li>
            <li>item 2</li>
            <li>item 3</li>
        </ul>

        <!-- both -->
        <ol>
           <li>
            <ul>
                <li>item 1</li>
                <li>item 2</li>
                <li>item 3</li>
            </ul>
           </li><br><br>
           <li>
            <ul>
                <li>item 1</li>
                <li>item 2</li>
                <li>item 3</li>
            </ul>
           </li>
        </ol>
    </p1>
</body>
</html>
``````

**5. HTML Link**

- We can use the link in HTML by using ```<a>``` tag with thier attributes "href"

**Example :-**
``````
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    header{
        background-color: powderblue;
        padding: 1rem;
    }
</style>
<body>
   <header>
       <a href="/home">Home</a>
       <a href="/contact">Contact</a>
   </header>
</body>
</html>
``````


**6. HTML form**
- The HTML form used for the interaction between user and website
- ```<form>``` tag has some inner tags.
**```<input>```**
- ```<input>```  tag used to get the input from the user side.
- It is used in html form
- It has no close tag
- It is inline element
- It's get radio, checkbox etc.
- The attributes of ```<input>``` are :
1. type
2. id 
3. name
4. placeholder
5. value

```<textarea>```
-  ```<textarea>``` tag control multi-line text input
- The attributes of ```<textarea>``` are :
1. id 
2. name
3. rows 
4. cols
5. maxlength

```<button>```
- ```<button>``` tag defines button clickable

**Example :-**
``````
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
``````
