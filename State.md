# State:-

Sate is data that a component remembers between renders and that can change over time.

e.g...

1. Counter values
2. Form input
3. Whether a menu is open
4. Shopping cart items
5. Selected tabs

When state changes, React schedules a re-render so the UI can reflect the new value.

# Hook :-

A Hook is a special React function that lets function components use React features.

Hooks include:

- useState — manages state.
- useEffect — synchronizes with external systems.
- useRef — stores a mutable reference.
- useContext — reads context.
- useMemo — caches a calculated value.
- useCallback — caches a function definition.

# Syntax for the useState:

import { useState } from "react";

const [state, setState] = useState(initialValue);

state - current value
setState - updated value
initial value - initial value assigned

# Counter Example:

import { useState } from "react";

function Counter() {
const [count, setCount] = useState(0); <!-- Here count- current value; setCount - updated value useState - hook; count & setCount - prop-->

return (
<div>
<h1>Count: {count}</h1>

      <button onClick={() => setCount(count + 1)}>
        Increase
      </button>

      <button onClick={() => setCount(count - 1)}>
        Decrease
      </button>
    </div>

);
}

export default Counter;

# Rules for the State:

1. Do not directly modify state variables.
2. Call the setter to request an update.
3. State updates may be batched.
4. A setter does not immediately change the state variable in the currently executing function.
5. Each render sees a snapshot of state.
6. Never call Hooks conditionally, inside loops, or inside ordinary nested functions. Call them at the top level of a function component or a custom Hook.
