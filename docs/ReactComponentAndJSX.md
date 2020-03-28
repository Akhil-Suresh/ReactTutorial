
# React Component and JSX

## React Component

React component is a function or a class that produces HTML to show the user and handles feedback from the user.

Inorder to produce HTML to show the user we make use of `JSX` and to handle feedback from the user we make use of `Event Handlers`.




# JSX

JSX is an XML/HTML-like syntax used by React that extends ECMAScript so that XML/HTML-like text can co-exist with JavaScript/React code.

## JSX VS HTML

Though both looks like same, There are some obvious differences.

 - Adding custom styling to an element uses different syntax
 - Adding a class to an element uses different syntax
 - JSX can reference JS variable.


### Adding inlline syntax with JSX

HTML: <div style="background-color:red;"></div>
JSX :  <div style={{backgroundColor: 'red'}}></div>


```js
// Importing React and ReactDOM libraries
import React from 'react';
import ReactDOM from 'react-dom';

// Create react component
// This is a function based component following ES5 syntax
const App = function() {

    // JSX that is being returned
    return (
        <div> Just a hello world </div>
    )
}

// Since we are making use of Babel behind the scene we can utilise ES2015 syntax
// This is a function based component following ES2015
const AppTwo = () =>  {
    return (
        <div> Just a hello world </div>
    )
}


ReactDOM.render(
    <App />,
    document.getElementByID('root'),    // This is element inside public/index.html
);

```
