# Props:-

Props (short for properties) allow a parent component to pass data to a child component.
function Welcome(props) {
return <h1>Hello, {props.name}!</h1>;
}

function App() {
return (
<>
<Welcome name="Prince" />
<Welcome name="Rahul" />
</>
);
}
In short props basically works as an input for the other functions as we can see above (props) in the function Welcome is passed as an parameter and that function is used as an argument in the function App.

The children Prop:
The special children prop contains the content placed between a component's opening and closing tags.
function Card({ children }) {
return <div className="card">{children}</div>;
}

function App() {
return (
<Card>

<h2>My Card</h2>
<p>This content appears inside the card.</p>
</Card>
);
}
so here the prop is being used as the parent tag.

# Rules of the Prop:

1. Props are read-only from the receiving component's perspective.
2. A child should not mutate its props.
3. Props can contain strings, numbers, arrays, objects, functions, and JSX.
4. Props support reusable components with different data.
