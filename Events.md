# Event handling:-
Event handling allows your application to respond to user actions such as clicking buttons, typing into inputs, submitting forms, and moving the mouse.
e.g...
function App() {
  function handleClick() {
    alert("Button clicked!");
  }

  return <button onClick={handleClick}>Click Me</button>;
}
<!-- handleClick is working as an Event Handling -->

# Common React Events are as follows:
1. onClick	- Mouse click or button activation
2. onChange - Detect changes to form controls
3. onSubmit - Form submission
4. onMouseEnter - Pointer enters an element
5. onKeyDown - Keyboard key is pressed
6. onFocus - Element receives focus
7. onBlur - Element loses focus

# Ways to handle event :
1. Incorrect :
<button onClick={handleClick()}>Click</button> <!-- Cant pass the arguments  -->

2. Correct :
<button onClick={handleClick}>Click</button>

3. If need to pass argument use Arrow Function:
function App() {
  function greet(name) {
    alert(`Hello, ${name}`);
  }

  return (
    <button onClick={() => greet("Prince")}>
      Greet
    </button>
  );
}