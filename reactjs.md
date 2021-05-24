# 1. What is React ?
- React is a javascript UI library.
- It is developed by facebook in 2011.
- It is used a component-based approach that can be reuse overall project.
- It has some features that's why react is more popular than other frameworks.

# 2. What are the features of React and Explain them?
## 1. Components
- Components are the building block of React application.
- Single applications contain multiple Components.
- Components are used to split the independent reusable part of an application that can be processed separately.
- React has two types of Components

**1. Class based component/Statefull component.**
- The class-based component writes by using the Class keyword
- The class-based component has its own state
- The class-based has their own render method

**2. Functional component/Stateless component**
- The Functional component has no own state and render method  
- They may derive data from other components as a props 

## 2.JSX
- JSX is a syntax extension from the javascript library
- JSX stands for javascript XML
- JSX is used to describe what the user interface should look like
- With the help of JSX, we can write the HTML structure into the same file that contains javascript code.
- Browser does not know the JSX because the browser reads only a plain javascript object and JSX is not a plain object to convert JSX into plain JS one transpiler used called babel

## 3. Unidirectional data flow
- React follows the one-way data binding means when designing a react app we often nest child withing parent-child
- With the help of one data binding, we can debug errors easily and find where is the problem occurs 

## 4. Virtual DOM
- React keeps a lightweight representation of real DOM called Virtual DOM.
- When the state of an object changes Virtual DOM only change this state of the component rather than updating all the object.

## 5. High Performance
- Because of virtual dom react has to update only changed component rather than updating all the component at once. The result is the performance of the application is high.


# 3. What is react router ?
- React router is a library used in react to navigate one to another because react used to create single-page application
- React router has some component Link,NavLink, Route, BrowserRouter and Switch
    - Link - It is work the same as an anchor tag link only difference is Link is used to navigating the page without refreshing the page
    - NavLink - It is used to style the active routes and It is work same as Link.
- React router has some hooks useLocation(), useRouteMatch(), useParams(),useHistory()

# 4. What is state ?
- It is nothing but the object in react.
- The state contain all the information and logic of the component
- The state of an object changes the component update only this changes rather than updating/re-rendering all the components
- The state is mutable
- Update the state by using setState()
- In Functional component we can manage the state by using useState() hook

# 5. What is props ?
- Props is a property that can be used as an attribute in component same as HTML attributes
- With the help of props, we can pass the data from one component to another component
- It is immutable
- It can read only

# 6. What is event ?
-  Event is an action that user or system may trigger for example mouse click, press the keyboard button.

# 7. What is key ?
- Key is a unique identifier It is used to identify which item of the list is update ,delete and add.
- It is used to determine which component need to be re-render instead of re-rendering all the component every time. 

# 8.What are the Life Cycle Methods in react ?
- getInitialState()- This method execute before creating a component
- componentDidMount() - This method execute when the components get render and placed into a dom
- shouldComponentUpdate() - This method invoked(call) when a component wants to change into the dom it gives true or false value depending on certain condition
- componentDidUpdate() - This method invoked immediatly after rendering takes place
- componentWillUnmount() - This method invoked immediatly before component distroyed  

# 9. What is render() method ?
- Every component has render() method
- It returns an HTML which is to display in the component
- If we want to render more than one element all the element must be inside the parent tag <div></div> or <></> (react fragment synthetic sugar form)

# 10. What is hook ?
- The hook is a new feature introduced the react in the 16.8 version
- The hook is a javascript function we use in the Functional component.
- Before react 16.8 version if we want to manage the state we used a class-based component but after the 16.8 version we manage the state by using 
useState() hook
**Pre-requisites**
- Hook use inside the function at the top
- We can't use hook inside class

# 11. What is useState() ?
- The useState() is a hook.
- The useState() is used to manage the state.

# 12. What is useEffect() ?
- The useEffect() is a hook.
- If we want to do something after rendering the component that time useEffect() hook is used
- The useEffect() allows Functional component to have lifecycle methods such as componentDidMount, componentDidUpdate and componentWillUnmount

# 13. How to create a React app ?
- Install node because node has npm package this package has react library
- npx create-react-app <appname>(small letter)
- Any text editor we can use for example vsCode, sublime text , atom etc

