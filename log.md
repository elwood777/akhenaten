# Akhenaten (log)
[akhenaten](https://github.com/elwood777/akhenaten)
A simple applicaion to showcase an solid understanding Jest within ReactJS.

**Objective**   
Deep dive into the world of JEST within the REACTJS concept








## Getting Started


### Create The App
Create a new React component called "akhenaten" (To Do List) 
```
npx create-react-app akhenaten
``` 

### Install packages  
Change directory into the new "akhenaten" direcotry
```
$ cd akhenaten/
```   
Install packages
```
$ npm i
```


### Update The File Structure
Updated the boilerplate project with an updated folder structure.
```
akhenaten/
  |- src/
  |   |- assets/
  |   |- components/
  |   |- context/
  |   |- data/
  |   |- hooks/
  |   |- pages/
  |   |- utils/
  |- package.json
```

### Run The New Project
```
npm starts
```








---  

Let's say we want to build a simple React component and test it using Jest. For this example, let's create a "HelloWorld" component that renders a simple message on the screen.

First, we'll set up our project with the following file structure:

```
akhenaten/
  |- src/
  |   |- HelloWorld.js
  |- __tests__/
  |   |- HelloWorld.test.js
  |- package.json
```

In the "src" directory, we'll create a file called "HelloWorld.js" that defines our component:
```jsx  
// HelloWorld.js

import React from 'react';

function HelloWorld() {
  return (
    <div>
      <h1>Hello World!</h1>
    </div>
  );
}

export default HelloWorld;


```  


In the "tests" directory, we'll create a file called "HelloWorld.test.js" that contains our Jest tests:
```jsx  
// HelloWorld.test.js

import React from 'react';
import { render } from '@testing-library/react';
import HelloWorld from '../src/HelloWorld';

describe('HelloWorld', () => {
  it('renders the message "Hello World!"', () => {
    const { getByText } = render(<HelloWorld />);
    const messageElement = getByText(/Hello World!/i);
    expect(messageElement).toBeInTheDocument();
  });
});


```  

In this test, we're using the "@testing-library/react" package to render our component and interact with its output. We're also using Jest's built-in "expect" function to assert that the rendered message contains the text "Hello World!".

Finally, we'll update our "package.json" file to include the necessary dependencies and scripts:

```json
{
  "name": "my-react-app",
  "version": "1.0.0",
  "dependencies": {
    "react": "^17.0.2",
    "react-dom": "^17.0.2"
  },
  "devDependencies": {
    "@testing-library/react": "^12.1.2",
    "jest": "^27.5.1",
    "babel-jest": "^27.4.5",
    "@babel/preset-env": "^7.16.11",
    "@babel/preset-react": "^7.16.7"
  },
  "scripts": {
    "test": "jest"
  }
}

```  

In this file, we're using Jest to run our tests, as well as several Babel and Jest packages to transpile and configure our code.

To run our tests, we can simply run the following command in the terminal:

```
npm run test
``` 

This will execute our Jest tests and output the results in the terminal. If everything is working correctly, we should see a passing test for our "HelloWorld" component.

---  


## Other Commands
This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

Starts the development server.
```  
$ npm start
```  

Bundles the app into static files for production.
```  
$ npm run build
``` 

Starts the test runner.
```  
$ npm test
``` 

Removes this tool and copies build dependencies, configuration files and scripts into the app directory.
```  
$ npm run eject
``` 

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)