# Keeper-App-Part-2

## App.jsx
```js
import React from "react";
import Header from "./Header";
import Footer from "./Footer";
import Note from "./Note";
import notes from "../notes";

function App() {
  return (
    <div>
      <Header />
      {notes.map((entry) => (
        <Note key={entry.key} title={entry.title} description={entry.content} />
      ))}
      <Footer />
    </div>
  );
}

export default App;


Created with CodeSandbox
