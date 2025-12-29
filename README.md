# React-Short-Notes
--Handwritten Notes--

React js is a javascript library developed by facebook. it is used for building user interfaces specifically for single page applications. it is used for handling the view layer for web and mobile apps. react also allows us to create reusable ui components.

the main goal for using react is that the websites build using only html css and javascript are static websites. to make them dynamic we need to use some javascript libraries like jquery. but jquery is not efficient for building large scale applications. so to overcome this problem react js was developed.
reloading the entire webpage is not required when using react js. only the components which are changed are reloaded. this makes the application faster.

this is done using a concept called virtual dom. when a component is changed a new virtual dom is created and it is compared with the previous dom. then only the changed components are updated in the real dom. this makes the application faster and efficient.

some of the features of react js are:
1. jsx: jsx is a syntax extension for javascriptXML. it looks similar to html. it is used to describe what the ui should look like. jsx makes it easier to write and add html in react.
2. components: components are the building blocks of a react application. they are reusable pieces of code that return a react element to be rendered to the page. components can be functional or class based.
3. one way data binding: react follows one way data binding. this means that the data flows in one direction. from parent to child. this makes the application more stable and easier to debug.
4. performance: react uses virtual dom to improve the performance of the application. it minimizes the number of updates to the real dom by only updating the changed components.
5. ecosystem: react has a large ecosystem of libraries and tools that can be used to build complex applications. some popular libraries are redux, react router, and axios.

we generally use react with jsx. jsx is a syntax extension for javascript. it looks similar to html. it is used to describe what the ui should look like. jsx makes it easier to write and add html in react.
jsx is not a necessity to use react. we can also use react without jsx. but using jsx makes the code easier to understand and write.
jsx is not supported by browsers. so we need to use a transpiler like babel to convert jsx to javascript. babel is a popular javascript compiler that is used to convert jsx to javascript.
we also use vite as a bundler. vite is a build tool that is used to bundle the react application. it is faster than other bundlers like webpack and parcel.

jsx syntax is similar to html. but there are some differences.
1. jsx uses className instead of class. this is because class is a reserved keyword in javascript.
2. jsx uses htmlFor instead of for. this is because for is a reserved keyword in javascript.
3. jsx uses camelCase for event handlers. for example, onclick is written as onClick.
4. jsx uses curly braces {} to embed javascript expressions. for example, to display a variable we use {variableName}.
5. jsx elements must be closed. for example, <img> must be written as <img />.
6. jsx elements must have a single parent element. for example, if we want to return multiple elements we need to wrap them in a div or a fragment <> </>.
7. jsx comments are written inside curly braces. for example, {/* this is a comment */}.
8. jsx supports conditional rendering using ternary operators or logical && operator.
9. jsx supports lists and keys. we can use the map() function to render a list of elements. each element in the list must have a unique key prop.
10. jsx supports inline styles. we can use the style prop to add inline styles to an element. the value of the style prop must be an object with camelCase properties.
11. jsx supports fragments. fragments are used to group a list of children without adding extra nodes to the dom. we can use <> </> or <React.Fragment> </React.Fragment> to create fragments.
12. jsx supports self-closing tags. for example, <input> must be written as <input />.
13. jsx supports spreading props. we can use the spread operator ... to pass all the props of an object to a component.
14. jsx supports default props. we can use  defaultProps to set default values for props.
15. jsx supports prop types. we can use prop-types library to define the types of props.
16. jsx supports higher order components. higher order components are functions that take a component and return a new component.
17. jsx supports context. context is used to pass data through the component tree without passing props down manually at every level.
18. jsx supports portals. portals are used to render children into a different part of the dom.
19. jsx supports error boundaries. error boundaries are components that catch javascript errors anywhere in their child component tree, log those errors, and display a fallback ui instead of the component tree that crashed.
20. jsx supports hooks. hooks are functions that let us use state and other react features without writing a class.
21. jsx supports suspense. suspense is a feature that lets us wait for some code to load and declaratively specify a loading state while we wait.


we generally use vite as a bundler for react applications. vite is a build tool that is used to bundle the react application. it is faster than other bundlers like webpack and parcel.
there are several configuration files that are used in a react application. some of the important configuration files are:
index.html
 this is the main html file of the react application. it is used to load the react application in the browser. it contains a div with an id of root. this is where the react application is rendered.
index.jsx
 this is the main javascript file of the react application. it is used to render the react application in the browser. it imports the react and react-dom libraries and renders the App component inside the root div in index.html file.
App.jsx
 this is the main component of the react application. it is used to define the structure and layout
index.css
 this file is used to define the global styles for the react application. it is imported in the index.jsx file.
package.json
 this file is used to define the dependencies and scripts for the react application. it contains information about the project like name, version, description, author, license, etc. it also contains the scripts that are used to run the react application like start, build, test, etc.
vite.config.js
 this file is used to configure vite for the react application. it contains information about the root directory
eslint.config.js 
is used to include the necessary plugins and rules for linting React code.
this is used to make sure that the code follows best practices and is free of common errors.
 for example if multiple users are working on the same project it helps to maintain a consistent coding style.
 so they have to follow the same rules and guidelines.
gitignore
 this file is used to specify which files and directories should be ignored by git.
 for example node_modules directory is ignored because it contains all the dependencies of the project and it can be easily recreated by running npm install command.
 so there is no need to include it in the version control system.
 it helps to keep the repository clean and free of unnecessary files.
 it also helps to reduce the size of the repository and improve performance.
 it also hepl to secure sensitive information like API keys and passwords by ignoring files that contain them.


component based structure
in react js the ui is divided into small reusable components. each component is a self contained piece of code that defines the structure and behavior of a part of the user interface.
this is done by creating a separate file for each component and importing them in the app component.
finally this app component is rendered in the main.jsx file.

how index.css applies css properties to app.jsx and somponents
 index.css is like “foundation styling” for the whole site.

App.css is like “styling the main app container”.
