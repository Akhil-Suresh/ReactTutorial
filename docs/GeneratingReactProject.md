# Why React

    - Virtual DOM
    - Reusable (and clearer) Web Component

## Generating react project

To start a react project we need to have node and npm installed on our local machine.

Then react application can be started by adding just React and ReactDOM libraries

The project scaffolding and bare project structure will be available through `create-react-app` tool.

So we can make utilise that to quickly start our project.

## Steps to start React Project

```
    Install NodeJS -> Install create-react-app tool -> generate project -> Build project
```

### Installing Node JS

    Follow any tutorial (Digital Ocean one is recommended)

### Install create-react-app tool

```sh
    sudo npm install -g create-react-app
```

The above command will take some time to install

### Generate Project


```sh
create-react-app <app-name>
```

## Why create react app

Create react app behind the scene setup a ton of dependencies that's necessary for our project. The main being `Webpack`, `babel` and `Dev Server`

## Exploring create-react-app created project structure.

`create-react-ap` will setup the following list of project structure for us.

    src                 -> Folder to put our source code
    publlic             -> Folder to store static files
    node_modules        -> Will contain project dependencies
    package.json        -> Records our project dependencies
    package-lock.json   -> Exact version of packages that we install.
    Readme.md           -> Instruction on how to use project.


## Starting and stopping React application

To start and stop react application 

To start project

    cd <app-name>
    npm start

To stop the project

    cntrl + c

