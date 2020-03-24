# Hello World React App

`create-react-app` create a lot of files which is not necessary at this point so delete all those files and put only `index.js` inside src folder.

# Hello World Program

```js
import React from 'react'
import ReactDOM from 'react-dom'


ReactDOM.render(
    <div><h1>Hello World</h1></div> ,
    document.getElementById('root')
);
```

We need to import react and react-dom libraries.

When we run `npm start` it will bring up `Hello World`.

The First part
     <div> 
        <h1> Hello World </h1> 
    </div>
    
Is called JSX