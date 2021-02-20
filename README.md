# React Repo Which 63526 843 2-56837 263 27736259 56837 HELPED ME Make

### Fragments In React:
```
<> </>
```
### Module Not Found: Cannot Resolve ...
- This means that you are trying to use a file that isn't created or its path is incorrect when you imported it



### Default Port Which React Runs On:
- 3000



### CodeSnippets
- rfc: React Functional Component
- race: React Arrow Function Component Export
- rcc: class component skeleton
- rrc: class component skeleton with react-redux connect
- rrdc: class component skeleton with react-redux connect and dispatch
- rccp: class component skeleton with prop types after the class
- rcjc: class component skeleton without import and default export lines
- rcfc: class component skeleton that contains all the lifecycle methods
- rwwd: class component without import statements
- cwm: component will mount method skeleton
- cdm: componentDidMount method skeleton
- cwr: componentWillReceiveProps method
- scu: shouldComponentUpdate method
- cwup: componentWillUpdate method
- cdup: componentDidUpdate method
- cwun: componentWillUnmount method
- ren: render method
- sst: this.setState with object as parameter
- ssf: this.setState with function as parameter
- props: this.props
- state: this.state
- bnd: binds the this of method inside the constructor
- disp: MapDispatchToProps redux function




### Other Ports To Run React On:
- 37532
- 42932
- Range Of Ports: [0,65535]  .... I am using Interval Notation FYI

#### How To Install Components Features Through NPM
```bash
npm install -g create-react-component
```


#### Files Which Are Usually Deleted
- App.css
- App.test.js
- logo.svg
- setupTests.js

#### What is the difference between State And Props in React
- State houses the object vals which belong to a component
- Props are we pass in between components... Typically between parent comp and child comp



### How To Pass From One Part Of Your App to annother
- The end goal of passing data is for it to reach the tree of the child component. Now to move data from the child to the parent component I use props.

### What Is State? You will always here this keyword when dealing with ReactJS
- State is just an object. State is used in the class component, and we must remember that state stores the component data and determines the component behavior

### What is a Component?
- Your application is made up of thousands of pieces. Every piece is what we call a "component"
	- Example: navigation bar, sidebar


### Difference between Functional And Class Based Components:
- We Use a Class Based Ccmponent when you want a specific component to be aware of another component
- We use a Functional Component aka functions to perform certain tasks indepedent of another. Say Function A is unaware and doesn't know Function B nor of its role


#### Memoization
- The process by which we store a super heavy functional component in memory 
- I reuse this component thanks to Caching

#### Virtual DOM vs Real DOM
- Virtual DOM has the exact same properties as Real DOM but virtual DOM doesn't have the power to change things directly
- DOM Manipulation is slow
- Virtual DOM Manipulation is fast

### IF YOU DO NOT KNOW WHAT THE DOM IS:
- process by which we take all the nasty html elements and put them in a object that has tree structure

#### How To Create A Component
```bash
create-react-component thepasccomponentisthebestcompfor27375fb
```
#### Smart Components Vs Dumb Components
- Smart Components are components which are at the application level that have the ability to execute functions and manage data
- Dumb Components are components that strictly deal with the User Interface


#### How To Create A Column in file Whatever.js
```js
import React { Component } from 'react';

export default Whatever extends Component {
	render() {
		return (
			<div className="col-md-4"></div>
		)
	}
}
```

#### How To Create A Row in file Whatever.js
```js
import React { Component } from 'react';

export default Whatever extends Component {
	render() {
		return (
			<div className="row"></div>
		)
	}
}
```

#### How To Get the FE communicate with the BE:
- SOAP
- REST


### How to Render Sth In React 
#### I can put 27375 in place of this.state.pascal and it will render
```js
import React, { Component } from "react";

class Pasc extends Component{
	state = {
		pascal: 1
	};

	render(){
		return(
			<div>{this.state.pascal}</div>
		);
	}
}

export default Pasc;
```

### Destructuring Explained in React

#### Without Destructuring
```js
//Without destructuring I would have the following
var example = useState('yourStateGoesHereAndAskNelanToLearnLLP');
var firstElement = example [0];
var secondElement = example[1];
```

#### Using Destructuring
```js
const [firstElement, secondElement] = useState('yourStateGoesHereAndAskNelanToLearnLLP');
```

### Example 2
```js
//Without destructuring
const hookForNumbers = useState(2);
const number = hookForNumbers[0];
const setNumber = hookForNumbers[1];

//with destructuring
const [number, setNumber] = useState(2);
```


### 1 How to install prereqs for react and all other dependencies necessary to your project
```bash
mkdir my-react-app
cd my-react-app
npm init --y
npm install react react-dom 
npm install --save-dev webpack webpack-dev-server html-webpack-plugin @babel/core babel-loader @babel/preset-env @babel/preset-react 
```

### 2: Create React Application using the create-react-app command
```bash
npx create-react-app 
```
### 3: Remove the following files that come shipped with the create-react-app command
- setupTests.js
- serviceWorker.js
- logo.svg
- index.css
- App.test.js



### 4: Paste the required script in the webpack.config.js file for webpack setup
```js
const path = require('path');
const HtmlWebpackPlugin = require('html-webpack-plugin');

module.exports = {
  // the output bundle won't be optimized for production but suitable for development
  mode: 'development',
  // the app entry point is /src/index.js
  entry: path.resolve(__dirname, 'src', 'index.js'),
  output: {
  	// the output of the webpack build will be in /dist directory
    path: path.resolve(__dirname, 'dist'),
    // the filename of the JS bundle will be bundle.js
    filename: 'bundle.js'
  },
  module: {
    rules: [
      {
      	// for any file with a suffix of js or jsx
        test: /\.jsx?$/,
        // ignore transpiling JavaScript from node_modules as it should be that state
        exclude: /node_modules/,
        // use the babel-loader for transpiling JavaScript to a suitable format
        loader: 'babel-loader',
        options: {
          // attach the presets to the loader (most projects use .babelrc file instead)
          presets: ["@babel/preset-env", "@babel/preset-react"]
        }
      }
    ]
  },
  // add a custom index.html as the template
  plugins: [new HtmlWebpackPlugin({ template: path.resolve(__dirname, 'src', 'index.html') })]
};
```

### 5: Paste the required script in the index.js file that is in your src directory aka source
```js
import React from 'react';
import ReactDOM from 'react-dom';

ReactDOM.render(<h1>Helloworld React!</h1>, document.getElementById('root'));
```


### 6: Paste the required script in the index.html file that is in your src directory aka source
```html
<html>
  <head>
    <title>Hello world App</title>
  </head>
  <body>
  <div id="root"></div>
  <script src="bundle.js"></script>
  </body>
</html>
```


### 7: Paste the required script in your package.json file so that you can automate with scripts your projects
```json
{
	"name": "my-react-tutorial-app",
	"version": "0.1.0",  
	"private": true,
	"dependencies": {
    	"react": "^16.5.2",
	    "react-dom": "^16.5.2",
	},
	"devDependencies": {
    	"react-scripts": "1.0.7"
  	},
  	"scripts": {
		"start": "react-scripts start",
		"build": "react-scripts build",
		"test": "react-scripts test --env=jsdom",
		"eject": "react-scripts eject"
	}    
}
```

### 7. React Project Layout. If you are build a SPA no need for components dir ignore this step and any subsequent one
```
├── README.md
├── node_modules
├── package.json
├── .gitignore
├── public
│   ├── favicon.ico
│   ├── index.html
│   └── manifest.json
└── src
    ├── App.css
    ├── App.js
    ├── App.test.js
    ├── components
        ├── Home.jsx
	├── NameOfYourSecondPage.jsx
	├── NameOfYourThirdPage.jsx
	├── NameOfYourFourthPage.jsx
	├── NameOfYourNthPage.jsx
	├── Navigation.jsx
	├── Footer.jsx
    ├── index.css
    ├── index.js
    ├── logo.svg
    └── serviceWorker.js

```
## For Projects

### Create a components folder in your src folder
```
├── README.md
├── node_modules
├── package.json
├── .gitignore
├── public
│   ├── favicon.ico
│   ├── index.html
│   └── manifest.json
└── src
    ├── App.css
    ├── App.js
    ├── App.test.js
    └── components
      └── Footer
      └── Navbar
         ├──index.js
         ├──
    └── images
    └── pages
    └── videos
    ├── index.css
    ├── index.js
    ├── logo.svg
    └── serviceWorker.js

```

### 8. If you are a build a MPA run this command to setup routing
```bash
npm i react-router-dom
```

### 9. If you want bootstrap here is the boiler plate index.html
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <link rel="icon" href="%PUBLIC_URL%/favicon.ico" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta name="theme-color" content="#000000" />
    <meta
      name="description"
      content="Web site created using create-react-app"
    />
    <link
      rel="stylesheet"
      href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css"
    />
    <title>React App</title>
  </head>
  <body>
    <noscript>You need to enable JavaScript to run this app.</noscript>
    <div id="root"></div>
  </body>
</html>
```
