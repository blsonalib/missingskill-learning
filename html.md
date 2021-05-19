**1. What is HTML ?**
- HTML is a Hyper Text Markup Language.
- HTML is used for create the structure of web pages.

**2. HTML Basics**

**```<!DOCTYPE html>```**
- All HTML document must start from ```<!DOCTYPE html>``` It's means we used document type is HTML .


**```<html>```**
- HTML start from ```<html>``` tag itself and end with  ```</html>```. This is parent node of all html tags.


**```<body>```**
- It is visible part of document start with ```<body>``` and end with ```</body>```


**3. Basic HTML Element**
- The HTML element is everything from the start tag to end tag.
- Example: ```<tagname>```content...```</tagname>```


**h1,h2,h3,h4,h5,h6**
- This is heading element
- ```<h1>``` is the largest heading and ```<h6>``` smallest heading

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
    <title>Document</title>
</head>
<body>
    <div>This is division....</div>
       <p>This is paragraph 1</p><br>
       <p>This is paragraph 2</p><br>
       <p>This is paragraph 3</p>
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

