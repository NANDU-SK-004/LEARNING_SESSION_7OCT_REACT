# LEARNING_SESSION_7OCT_REACT
the whole code is at App.jsx


CODE #1

function App() {
  const name = "NANDU";
  return (
    <div>
      <h1>Hello {name}!</h1>
      <p>Welcome to React 🌊</p>
    </div>
  );
}
export default App;


CODE #2

import { useState } from "react";

function App() {
  const [count, setCount] = useState(0); // initial count = 0

  return (
    <div style={{ textAlign: "center", marginTop: "50px" }}>
      <h1>Counter: {count}</h1>
      <button onClick={() => setCount(count + 1)}>Increase</button>
      <button onClick={() => setCount(count - 1)}>Decrease</button>
      <button onClick={() => setCount(0)}>Reset</button>
    </div>
  );
}

export default App;


CODE #3

import { useState } from "react";

function App() {
  const [isHello, setIsHello] = useState(true);

  return (
    <div style={{ textAlign: "center", marginTop: "50px" }}>
      <h1>{isHello ? "Hello " : "Goodbye "}</h1>
      <button onClick={() => setIsHello(!isHello)}>Toggle Message</button>
    </div>
  );
}

export default App;


CODE #4

import { useState } from "react";

function App() {
  const [text, setText] = useState("");

  return (
    <div style={{ textAlign: "center", marginTop: "50px" }}>
      <input
        type="text"
        placeholder="Type something..."
        value={text}
        onChange={(e) => setText(e.target.value)}
        style={{ padding: "5px", fontSize: "16px" }}
      />
      <h2>You typed: {text}</h2>
    </div>
  );
}

export default App;



