
```markdown

# My Custom React Package : "pack-to-vui"

A simple React package providing a custom hook `useCount` for state management and a `Button` component for UI. Easily add these components to enhance your React projects.

## Installation

To install this package, run the following command:

```bash

npm install pack-to-vui or npm i pack-to-vui

```

or, if using yarn:

```bash

yarn add pack-to-vui

```

# Components and Hooks

## `useCount`

A custom React hook that provides an easy counter functionality.

### Usage

```javascript

import { useCount } from 'pack-to-vui';

function CounterComponent() {

const { count, increment, decrement, reset } = useCount();

return (

<div>

<p>Current count: {count}</p>

<button onClick={increment}>Increment</button>

<button onClick={decrement}>Decrement</button>

<button onClick={reset}>Reset</button>

</div>

);

}

```

### API

- **`count`**: The current count value.

- **`increment()`**: Increments the count by 1.

- **`decrement()`**: Decrements the count by 1.

- **`reset()`**: Resets the count to the initial value.

## `Button`

A customizable button component for consistent UI styling across your application.

### Usage

```javascript

import { Button } from 'pack-to-vui';

function App() {

return (

<Button onClick={() => alert('Button Clicked!')} label="Click Me" />

);

}

```

### Props

- **`label`**: The text displayed on the button.

- **`onClick`**: Function to call when the button is clicked.

- **`style`** (optional): Custom styles for the button.

# Example Project

Here's an example project that uses both `useCount` and the `Button` component:

```javascript

import React from 'react';

import { useCount, Button } from 'pack-to-vui';

function ExampleApp() {

const { count, increment, decrement, reset } = useCount();

return (

<div style={{ textAlign: 'center', padding: '20px' }}>

<h1>Custom Hook and Button Demo</h1>

<p>Current count: {count}</p>

<Button onClick={increment} label="Increment" />

<Button onClick={decrement} label="Decrement" />

<Button onClick={reset} label="Reset" />

</div>

);

}

export default ExampleApp;

```

---

Developed with ❤️ by **Viraj Walavalkar**. Happy coding!

```