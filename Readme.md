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

### Steps

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










 