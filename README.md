# Keeper-App-Part-2

## App.js
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
```
## Note.js
```js
import React from "react";

function Note(props) {
  return (
    <div className="note">
      <h1>{props.title}</h1>
      <p>{props.description}</p>
    </div>
  );
}

export default Note;
```

Created with CodeSandbox
