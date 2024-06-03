# **REACT**

## WHAT IS REACT ?
React is a popular open-source JavaScript library  developed by Facebook for building user interfaces, particularly for single-page applications where you need a fast, interactive user experience.

  // Library : A library is a collection of pre-written code that you can use to perform specific tasks

## ADVANTAGES OF REACT 

1) EASY TO LEARN  
ReactJS is much easier to learn and use. It comes with a good supply of documentation, tutorials, and training resources. Any developer who comes from a JavaScript background can easily understand and start creating web apps using React in a few days


2) REUSABILITY   
Reusability means that we can reuse same components in multiple different places within your project    
         
// Components : Components can be considered as building blocks by which different parts of user interface is built for example : button , navbar etc

3) FLEXIBILITY   
Flexibility in React means the code is easier to work with and update because it's built in small, separate pieces called components. This makes React code easier to understand and maintain compared to other frontend frameworks.

4) SINGLE WEB APPLICATION   
Building of single web page application can be considered as advantage of React because it provides Fast and Responsive User Experience


## COMPARISION BETWEEEN REACT AND ANGULAR

### React

### Key Features
- **Library**: Focuses on building reusable UI components.
- **JSX**: Uses JSX, a syntax extension that allows HTML to be written within JavaScript.
- **Virtual DOM**: Updates the UI efficiently by only re-rendering components that have changed.
- **One-Way Data Binding**: Ensures a unidirectional data flow, making data management more predictable.
- **React Hooks**: Introduced hooks to allow the use of state and other React features in functional components.
- **Ecosystem**: Relies on third-party libraries for routing, state management, and other functionalities, offering great flexibility.

### Angular -

### Key Features
- **Framework**: Provides a complete solution including UI components, routing, state management, form validation, and more.
- **TypeScript**: Uses TypeScript, a statically typed superset of JavaScript, which helps catch errors early during development.
- **Two-Way Data Binding**: Simplifies synchronization between the model and the view, making it easier to handle user input.
- **RxJS**: Utilizes RxJS for reactive programming, making it easier to handle asynchronous data streams.
- **Angular CLI**: Provides a powerful command-line interface to scaffold and manage projects easily.  

## GETTING STARTED WITH REACT

## Installation

To start using React, you need to set up your development environment. The easiest way to get started is by using Create React App, a tool that sets up a new React project with a good default configuration.

### Prerequisites

Before you begin, make sure you have the following installed on your machine:
- **Node.js** (https://nodejs.org/) - React requires Node.js for building and running your application.
- **npm** (Node Package Manager) - This comes bundled with Node.js and helps manage dependencies.

### Steps

1. **Install Node.js and npm**:
   - Download and install Node.js from the official [Node.js website] (https://nodejs.org/).
   - After downloading Verify the installation by running the following commands in your terminal:
     ```bash
     node -v
     npm -v
     ```

2. **Install Create React App**:
   - Open your terminal and run the following command to install Create React App globally:
     ```bash
     npx create-react-app my-app (You can use any name for your directory instead of my-app just replace my-app with that name)
     ```
     This command creates a new directory called `my-app` with a default React project setup.

3. **Navigate to Your Project Directory**:
   - Change to the newly created directory:
     ```bash
     cd my-app  (Here we use cd to enter the directory . To go out of directory use cd..)
     ```

4. **Start the Development Server**:
   - Run the following command to start the development server:
     ```bash
     npm start
     ```
     Your new React application will open in your default web browser at `http://localhost:3000` (port number can change if port 3000 is busy with some other content)

## Hello World

Let's create a simple "Hello World" component to get a feel for how React works.

### Steps to Write Hello World 

1. **Open Your Project in a Code Editor**:
   - Use a code editor like Visual Studio Code (VS Code) to open the `my-app` directory.

2. **Edit `src/App.js`**:
   - Replace the content of the `src/App.js` file with the following code:
     ```jsx
     import React from 'react';

     function App() {
       return (
         <div>
           <h1>Hello, World!</h1>
         </div>
       );
     }

     export default App;
     ```

3. **Run Your Application**:
   - If the development server is not already running, start it by running `npm start` in your terminal.
   - Open your web browser and navigate to `http://localhost:3000`. You should see "Hello, World!" displayed on the page.

## Core Concepts of React

### JSX 
JSX stands for javascript XML and it allows us to write HTML in react 
So basically it converts HTML into React elements 

**Example 1**
```jsx
const myElement = (
  <div>
    <p>This is a react documentation</p>
    <p>It is written by Aryan Mamania</p>
  </div>
);
```

**Example 2**
Write "Hello" if x is less than 10, otherwise "Goodbye":
```jsx
const x = 5;
let text = "Goodbye";
if (x < 10) {
  text = "Hello";
}

const myElement = <h1>{text}</h1>;
```

### Components
Components can be considered as building blocks by which different parts of user interface is built for example : button , navbar etc
Componets are independent and reusable bits of code 
There are 2 types of React componets -
- Functional Components
Functional components are JavaScript functions that return React elements. They are used to build parts of the user interface in a React application. They may or may not recieve data as paramaeters 

Note :- The functional component is also known as a stateless component because they do not hold or manage state.

- Class based Components 

__________________________________________________________________________________________________________________________



### Props
Props is shorrt for properties and are used to pass data from one component to another . Props are similiar to function arguments and are passed to components in same was as arguments are passed in a function .  
The child component can't modify the props it recieves and can only read and use the props  

Example using Props-
App.js File (Parent class where we will define Props)
```jsx 
import React from 'react';
import Greeting from './Greeting';


function App() {
  
  const userName = 'Mamania';  // This is the data we want to pass to the child component

 
  return (
    <div>
      <Greeting name={userName} />  {/* Where Props is userName */}
    </div>
  );
}

export default App;
```
Greeting.js file (Child component where we will pass the Props)
```jsx  
import React from 'react';

function Greeting(props) {
  // Access the name prop from the props object
  const { name } = props;

  // Use the name prop to display a greeting message
  return <h1>Hello, {name}!</h1>;
}

export default Greeting;
```
OutPut -
```jsx
Hello, Mamania!
```

## State Management   

### State
State in React is like an object that stores information about the current state or state of your component. In easy words we can say how it is actually looking like in a given point of time . This information may change over time, and React will update the feature to reflect the latest information.  

- State as a Data Store: Each React component can have its own state, which stores dynamic information that the component can use and display.  

- Accessing State: In class components, you access the state using this.state.  

- Changing State: When the state changes, React automatically re-renders the component to show the new state.   

### State Management 
Changing State is a part of State Managmenet which allows state to maintain and update state accordingly . For example in a task management app when we add a task , a task is added and is considered as a change of state or state management . 
State management helps in making the webpage look dynamic .
We can change the component state by using the setState() method and passing a new state object as the argument
In React , state management can be managed within components using 'useState' hook for functional component or 'this.state' for class component .  

- Functional Component with useState  
```jsx
import React, { useState } from 'react';

function Counter() {     //we made a functional called counter
    const [count, setCount] = useState(0);   // count is initial state and setCount is state after changing state and initital state is 0  

    return (
        <div>
            <p>{count}</p>
            <button onClick={() => setCount(count + 1)}>Increment</button> 
        </div>
    );
}
```
In this above code whenever the button will be clicked its count will increase by 1 number. 

- Class Component with this.state
```jsx
import React, { Component } from 'react';

// Define a class component named Counter
class Counter extends Component {
    // Constructor method to initialize state
    constructor(props) {
        super(props); // Call the parent class's constructor
        this.state = { count: 0 }; // Initialize state with a count property set to 0
    }

    // Arrow function to handle incrementing the count
    increment = () => {
        // Update the state with the new count value
        this.setState({ count: this.state.count + 1 });
    }

    // Render method to define what the UI looks like
    render() {
        return (
            <div>
                {/* Display the current count */}
                <p>{this.state.count}</p>
                {/* Button to trigger the increment method on click */}
                <button onClick={this.increment}>Increment</button>
            </div>
        );
    }
}

export default Counter; // Export the Counter component as the default export
```
The above code will also do same thing . When the button will be clicked it will increase the value by 1 number . Initial State is 0

**Note**
- useState is used in class component 
- this.state is used in functional component

### Event Handling 

## Event   
An event is an action that could be triggered as a result of user action or system generated event . For example a mouse click event which is written as `onClick event`  
It captures and responds to user actions within application.

React uses different ways to handle event 
Some of The most common event handling techniques are 
 1) Mouse Events:
- onClick : Triggered when an element is clicked 
- onDoubleClick : Triggered when an action is doubleClicked
- onMouseEnter : Triggered when mouse pointer enters the element
- onMouseLeave : Triggered when mouse pointer leaves the element
2) Keyboard Events:
- onKeyDown : Triggered when a key is pressed down
- onKeyPress : Triggered when a key is pressed and held down
- onKeyUp : Triggered when a key is released
3) Form Events :
- onChange : Triggered when the value of an element changes
- onSubmit : Triggered when a form is submitted.
- onInput : Triggered when the value of an input element is changed.
```jsx
import React, { Component } from 'react';

// Define a React component named ClickButton
class ClickButton extends Component {

  // Define a method to handle the click event
  handleClick = () => {

    // Display an alert when the button is clicked
    alert('Button was clicked!');
  }

  // Render method to output the component's UI
  render() {
    return (
      // Button element with an onClick event handler
      <button onClick={this.handleClick}>
        Click Me
      </button>
    );
  }
}

// Export the component so it can be used in other parts of the application
export default ClickButton;
```
In the above code whenever a button is clicked it shows an alert stating that button was clicked 
















 