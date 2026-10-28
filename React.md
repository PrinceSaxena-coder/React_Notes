# React :-
1. Library of the Js
2. Used to build interactive Ui for the web application
3. It updates the page which is called the Rendering of the data
4. React applications are built using small, reusable pieces called components.
5. React commonly uses JSX, a syntax extension that lets you write HTML-like markup inside  JavaScript.

# Need of the React:
We used to do the DOM manually for every event handling in the JS as the web application gets larger work load increases and the pages to render get increase so in that case the DOM manually becomes tricky this is the place where the React comes in role...

# Setting up the React Env:
1. npm create vite@latest my-react-app -- --template react
2. cd my-react-app
3. npm install
4. npm run dev

# Important Project Files:
my-react-app/
├── public/
├── src/
│   ├── assets/
│   ├── App.jsx
│   ├── App.css
│   ├── index.css
│   └── main.jsx
├── index.html
├── package.json
└── vite.config.js

# Rules of React:
1. It Returns the single parent element
function App() {
  return (
    <div>
      <h1>Hello</h1>
      <p>Welcome</p>
    </div>
  );
}
<!-- Here everything is written inside the Div -->
where as we can also use fragments <></> in replacement of the Div what is compulsory to return a single parent element..

2. Close each & every tag
3. Use "className" instead of simply giving them a "class"
4. Usage of the camelCase for the JSX and DOM
5. Use curly braces {} to insert JavaScript expressions.
const name = "Prince";

function App() {
  return <h1>Hello, {name}!</h1>;
}