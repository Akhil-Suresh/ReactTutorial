# JSX

JSX is an XML/HTML-like syntax used by React that extends ECMAScript so that XML/HTML-like text can co-exist with JavaScript/React code. We make use of **Babel** to convert JSX to HTML. Browsers can't understand what JSX is, so behind the scene when JSX is send to browser it gets converted to normal Javascript code.

## JSX VS HTML

Though both looks like same, There are some obvious differences.

    - Adding custom styling to an element uses different syntax
    - Adding a class to an element uses different syntax
    - JSX can reference JS variable.

## Building content with JSX

We have seen how to create functional component in JSX and what a JSX is , now let's see how to build content with JSX

A very simple program can be written in JSX as

```js
    import React from 'react'
    import ReactDOM from 'react-dom'

    const App = () => {
        return (
            <div>
                <h1> Hello Akhil! </h1>
            </div>
        )
    }

    ReactDOM.render(<App />, document.getElementById('root'));
```

As I have already said above, JSX is not simply HTML. Its a XML/HTML-like syntax used by React. So there is a little bit difference with JSX.

### Some main things to note are

    - Adding a class follows a different syntax
    - Custom styling to an element follows a different syntax
    - JSX can reference JS variables

## Adding class

Class can be referenced inside JSX in a different format.

Normal HTML: `<div class="container"></div>`

JSX: `<div className='container'></div>`

## Inline styling with JSX

We can't normally put inline styling inside JSX, it also follows a different syntax

Normal HTML: `<div style="background-color: dark-red; position: absolute"></div>`

JSX: `<div style={{'backgroundColor': 'dark-red', 'position': 'absolute'}}></div>`

The above html element when put inside JSX will give you an error.

## Referencing Javascript Variables inside JSX

Javascript variable can be referenced inside JSX with the help of `{ }`(curly braces).

In the below code snippet see how the welcome message is referenced.

```js
const welcomeMessage = "Hi Akhil";

const App = () => {
    return (
        <div className="container">
            <span style={{'backgroundColor': 'black', 'color': 'white', 'border': '1px solid red'}}>
                {welcomeMessage}
            </span>
        </div>
    )
}
```

```js
const getWelcomeMessage = () => {
return "Hi Akhil"
};

const App = () => {
    return (
        <div className="container">
            <span style={{'backgroundColor': 'black', 'color': 'white', 'border': '1px solid red'}}>
                {getWelcomeMessage()}
            </span>
        </div>
    )
}
```

### gotchas

We can reference other types of variables other than string here.

```js
const text = ['Hi', 'Akhil'];
const number = [10, 20];
```

This is going to create trouble. `const textObj = {text: 'Hi there'}`

This can be solved through

```js
    const App = () => {
        return (
            <div className="container">
                <span style={{'backgroundColor': 'black', 'color': 'white', 'border': '1px solid red'}}>
                    {textObj.text}
                </span>
            </div>
        )
    }
```
