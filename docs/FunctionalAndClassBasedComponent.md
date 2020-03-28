# Functional and Class Based Component

## React Component

React component is a function or a class that produces HTML to show the user and handles feedback from the user.

Inorder to produce HTML to show the user we make use of `JSX` and to handle feedback from the user we make use of `Event Handlers`.

React supports function and class based component.

## Function based component.

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

// The root is an element inside public/index.html

ReactDOM.render(
    <App />,
    document.getElementByID('root'),
);

```

## Class based component.

```js
// Importing React and ReactDOM libraries
import React from 'react';
import ReactDOM from 'react-dom';

// Create react component
// This is a function based component following ES5 syntax
class App extends React.Component

ReactDOM.render(
    <App />,
    document.getElementByID('root'),    // This is element inside public/index.html
);

```
