
---

## 1. What is React?

- **React** is a **JavaScript library** for building **user interfaces**
    
- Developed by **Facebook (Meta)** in **2013**
    
- Used mainly for **single-page applications (SPAs)**
    
- Focuses on:
    
    - Declarative UI
        
    - Component-based architecture
        
    - Virtual DOM
        
- React is **less opinionated**
    
    - Only handles **view rendering & user interaction**
        
- Encourages **reusable** and **maintainable** UI components
    

---

## 2. Timeline of Front-End JavaScript Frameworks

- jQuery → 2006
    
- AngularJS → 2010
    
- **React → 2013**
    
- Vue → 2014
    
- Angular → 2014
    

---

## 3. Why React?

### 3.1 Virtual DOM

- Virtual DOM is a **lightweight copy** of the real DOM
    
- Traditional approach:
    
    - Direct DOM manipulation → slow
        
- React approach:
    
    - Updates Virtual DOM
        
    - Compares old vs new Virtual DOM (diffing)
        
    - Applies **only changes** to real DOM
        
- Improves:
    
    - Performance
        
    - User experience
        
    - Rendering efficiency
        

---

## 4. Component-Based Architecture

- UI is divided into **small reusable components**
    
- Each component:
    
    - Encapsulates UI logic
        
    - Is independent
        
- Benefits:
    
    - Modularity
        
    - Reusability
        
    - Easier maintenance
        
- Avoids tightly coupled HTML, CSS & JS
    

---

## 5. State Management in React

- **State** → mutable data of a component
    
- React provides multiple state management options:
    
    - Local component state → `useState()`
        
    - Context API
        
    - External libraries:
        
        - Redux
            
        - Zustand
            
        - MobX
            

---

## 6. What is a React Component?

- A **React component** is:
    
    - A **JavaScript function or class**
        
    - That returns **JSX**
        
- Components:
    
    - Encapsulate UI + logic
        
    - Are reusable
        
- Two types:
    
    - **Functional Components (preferred)**
        
    - Class Components
        

---

## 7. Structure of a React Component

### 7.1 Props

- Used to pass data from **parent → child**
    
- Props are:
    
    - Read-only
        
    - Immutable
        

---

### 7.2 State

- Represents dynamic data
    
- Managed using:
    
    - `useState()` (functional components)
        
    - `this.state` (class components)
        

---

### 7.3 Styling

- Styling options:
    
    - CSS classes (`className`)
        
    - Inline styles (`style={{}}`)
        
    - CSS-in-JS libraries
        

---

## 8. React Tool Chain

### Babel

- Transpiles:
    
    - JSX
        
    - Modern JavaScript (ES6+)
        
- Converts into browser-compatible JS
    

### Webpack

- Bundles:
    
    - JavaScript
        
    - CSS
        
    - Images
        
- Outputs optimized bundle (`bundle.js`)
    

---

## 9. What is JSX?

- **JSX (JavaScript XML)** is a syntax extension
    
- Allows writing **HTML-like code inside JavaScript**
    
- JSX:
    
    - Improves readability
        
    - Is NOT HTML
        
- JSX expressions use `{ }`
    
- JSX must be **compiled** (via Babel)
    

---

## 10. JSX Syntax Rules

- Must return **single parent element**
    
- Adjacent elements must be wrapped
    
- All tags must be **closed**
    
- JSX is **case-sensitive**
    
- HTML is NOT case-sensitive
    

---

## 11. JSX vs HTML Differences

|HTML|JSX|
|---|---|
|class|className|
|for|htmlFor|
|Case-insensitive|Case-sensitive|
|Comments: `<!-- -->`|`{/* */}`|

---

## 12. Comments in JSX

- HTML comments do NOT work
    
- Use:
    

```jsx
{/* This is a comment */}
```

---

## 13. React Component Lifecycle

### Phases

1. **Mounting** → component created & inserted into DOM
    
2. **Updating** → state or props change
    
3. **Unmounting** → component removed from DOM
    

---

## 14. Declaring Components (Functions)

- Components are **pure functions**
    
- Receive `props`
    
- Return React element tree
    
- Should be:
    
    - Idempotent
        
    - Side-effect free
        

Example:

```jsx
function Button(props) {
  return <button>{props.label}</button>;
}
```

---

## 15. React Project Folder Structure

### `public/`

- Static files
    
- `index.html` → root template
    

### `src/`

- All JavaScript files
    
- `index.js` → entry point
    
- `App.js` → main application component
    

---

## 16. Importing & Exporting (ES6 Modules)

- Uses:
    

```js
import ... from ...
export ...
```

- Browser uses **ES6 Modules**
    
- Different from Node.js `require()`
    

---

## 17. Example: Hello World

- App returns JSX
    
- Custom components are JS functions
    
- JSX attributes become props
    

---

## 18. Adding Bootstrap in React

Two ways:

1. Load Bootstrap CSS in `index.html`
    
2. Use **react-bootstrap** library
    

Commands:

```bash
npm install bootstrap
npm install react-bootstrap
```

---

# 📝 MCQs (15) – Single Correct

1. React was developed by:
    

- A) Google
    
- B) Facebook
    
- C) Microsoft
    
- D) Twitter  
    **Ans:** B
    

2. React focuses on:
    

- A) Database
    
- B) Styling
    
- C) UI rendering
    
- D) Server logic  
    **Ans:** C
    

3. Virtual DOM is:
    

- A) Real DOM
    
- B) Copy of DOM
    
- C) Database
    
- D) Browser API  
    **Ans:** B
    

4. JSX stands for:
    

- A) Java Syntax XML
    
- B) JavaScript XML
    
- C) JavaScript XHTML
    
- D) Java XML  
    **Ans:** B
    

5. JSX must be compiled by:
    

- A) Webpack
    
- B) Node
    
- C) Babel
    
- D) Browser  
    **Ans:** C
    

6. Preferred React component type:
    

- A) Class
    
- B) Functional
    
- C) Inline
    
- D) Abstract  
    **Ans:** B
    

7. Props are:
    

- A) Mutable
    
- B) Read-only
    
- C) Private
    
- D) Global  
    **Ans:** B
    

8. State represents:
    

- A) Static data
    
- B) Mutable data
    
- C) CSS
    
- D) HTML  
    **Ans:** B
    

9. HTML `class` becomes:
    

- A) class
    
- B) cssClass
    
- C) className
    
- D) htmlClass  
    **Ans:** C
    

10. JSX requires:
    

- A) Multiple roots
    
- B) Single root element
    
- C) No closing tags
    
- D) Inline JS only  
    **Ans:** B
    

11. React is:
    

- A) Framework
    
- B) Library
    
- C) Language
    
- D) Compiler  
    **Ans:** B
    

12. Component lifecycle phase for removal:
    

- A) Mounting
    
- B) Updating
    
- C) Unmounting
    
- D) Rendering  
    **Ans:** C
    

13. Babel is used for:
    

- A) Bundling
    
- B) Styling
    
- C) Transpiling
    
- D) Hosting  
    **Ans:** C
    

14. Webpack is used for:
    

- A) Transpiling
    
- B) Bundling
    
- C) Rendering
    
- D) Compiling JSX  
    **Ans:** B
    

15. React Bootstrap provides:
    

- A) CSS only
    
- B) JS only
    
- C) React components
    
- D) Database  
    **Ans:** C
    

---

# ☑️ Checkbox MCQs (15) – Multiple Correct

1. React features:
    

- ☑ Virtual DOM
    
- ☑ Components
    
- ☑ Declarative UI
    
- ⬜ Database
    

2. Benefits of Virtual DOM:
    

- ☑ Faster updates
    
- ☑ Selective rendering
    
- ⬜ More memory usage
    
- ⬜ Slower UI
    

3. React components:
    

- ☑ Reusable
    
- ☑ Modular
    
- ⬜ Static
    
- ⬜ Tightly coupled
    

4. State management options:
    

- ☑ useState
    
- ☑ Context API
    
- ☑ Redux
    
- ⬜ SQL
    

5. JSX:
    

- ☑ HTML-like syntax
    
- ☑ JavaScript expressions
    
- ⬜ Browser-native
    
- ⬜ CSS replacement
    

6. JSX rules:
    

- ☑ Single root
    
- ☑ Closing tags
    
- ☑ Case-sensitive
    
- ⬜ HTML comments
    

7. Toolchain:
    

- ☑ Babel
    
- ☑ Webpack
    
- ⬜ MongoDB
    
- ⬜ Apache
    

8. Props:
    

- ☑ Passed from parent
    
- ☑ Read-only
    
- ⬜ Mutable
    
- ⬜ Global
    

9. Functional components:
    

- ☑ Use props
    
- ☑ Return JSX
    
- ⬜ Must use class
    
- ⬜ Are state-less always
    

10. Lifecycle phases:
    

- ☑ Mounting
    
- ☑ Updating
    
- ☑ Unmounting
    
- ⬜ Compiling
    

11. Folder structure:
    

- ☑ public
    
- ☑ src
    
- ⬜ build.js
    
- ⬜ config.xml
    

12. index.js:
    

- ☑ Entry point
    
- ☑ Mounts App
    
- ⬜ Styles UI
    
- ⬜ Hosts server
    

13. Import/export:
    

- ☑ ES6 modules
    
- ☑ import keyword
    
- ☑ export keyword
    
- ⬜ require()
    

14. React Bootstrap:
    

- ☑ Uses components
    
- ☑ Mimics Bootstrap classes
    
- ⬜ Replaces React
    
- ⬜ Backend library
    

15. JSX comments:
    

- ☑ {/* comment */}
    
- ⬜
    
- ⬜ //
    
- ⬜ #
    

---

# 🛑 ERROR IDENTIFICATION & SYNTAX MCQs (20)

```jsx
function App() {
  return <h1>Hello</h1><p>World</p>;
}
```

Error?

- A) Multiple root elements
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
<div class="box"></div>
```

Error?

- A) class should be className
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
<label for="name"></label>
```

Error?

- A) for should be htmlFor
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
<img src="a.png">
```

Error?

- A) Missing closing slash
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
{/* comment */}
```

Error?

- A) No error
    
- B) Syntax error
    
- C) JSX error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
if (true) {
  return <h1>Hi</h1>;
}
```

Error?

- A) JSX inside condition
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** C
    

---

```jsx
const App = () => {
  <h1>Hello</h1>
}
```

Error?

- A) Missing return
    
- B) Syntax error
    
- C) No error
    
- D) JSX error  
    **Ans:** A
    

---

```jsx
function app() {
  return <div></div>;
}
```

Error?

- A) Component name should be capitalized
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
const x = <div>{}</div>;
```

Error?

- A) Empty expression
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
return (
  <div>
    <p>Hi</p>
);
```

Error?

- A) Missing closing div
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
const App = props => <h1>{props}</h1>;
```

Error?

- A) props is object
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
<button onclick={handleClick}></button>
```

Error?

- A) Event should be camelCase
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
const App = () => <React.Fragment></React>;
```

Error?

- A) Wrong closing tag
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
return <div>Hi</span>;
```

Error?

- A) Mismatched tags
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
<div style="color:red"></div>
```

Error?

- A) style should be object
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
const App = () => (<div/>);
```

Error?

- A) No error
    
- B) Syntax error
    
- C) JSX error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
{ if(true) return <h1>Hi</h1>; }
```

Error?

- A) if not allowed inside JSX
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
const App = () => <></>;
```

Error?

- A) No error
    
- B) Syntax error
    
- C) JSX error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
<div>{props.name, props.age}</div>
```

Error?

- A) Comma operator issue
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
export default App();
```

Error?

- A) Exporting function call
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

Below is **the same full, exam-oriented package** for your **`useEffect()` in React PPT**, exactly following the format you’ve been using everywhere:

✔ **Detailed Obsidian-ready notes**  
✔ **15 MCQs (single correct)**  
✔ **15 Checkbox MCQs (multiple correct)**  
✔ **20 Error Identification / Syntax Error MCQs**

All content is **strictly derived from your uploaded `useEffect()` PPT**

---

# 📘 `useEffect()` Hook in React

_(Obsidian-Ready Notes)_

---

## 1. Hooks in React

- **Hooks** allow using React features in **functional components**
    
- Introduced in **React 16.8**
    
- Hooks remove the need for:
    
    - Class components
        
    - Lifecycle methods
        
- Examples:
    
    - `useState()`
        
    - `useEffect()`
        
    - `useContext()`
        

---

## 2. Understanding `useEffect()`

- `useEffect()` is a **React Hook** used to handle **side effects**
    
- Side effects are operations **outside normal rendering**
    
- React functional components:
    
    - Re-render **many times**
        
- Without `useEffect()`:
    
    - Code runs on **every render** → ❌ BAD practice
        

---

## 3. What is a Side Effect?

A **side effect** is any operation that affects something **outside the component UI**

Examples:

- Fetching data from API
    
- Updating `localStorage`
    
- Subscribing to events
    
- Timers (`setTimeout`, `setInterval`)
    
- Manually changing DOM
    

---

## 4. Why `useEffect()` is Needed

- Prevents unnecessary execution of logic
    
- Lets you control:
    
    - ✔ **WHEN** code runs
        
    - ✔ **HOW OFTEN** code runs
        
    - ✔ **WHAT causes** it to run
        
- Keeps rendering **pure and predictable**
    

---

## 5. Basic Syntax of `useEffect()`

```jsx
useEffect(() => {
  // side effect code
}, [dependencies]);
```

### Parts:

- **Effect function** → runs after render
    
- **Dependency array** → controls execution
    

---

## 6. `useEffect()` Execution Timing

- Runs **after component renders**
    
- Runs **after DOM updates**
    
- Never runs during render phase
    

---

## 7. Dependency Array – Key Concept

The behavior of `useEffect()` depends on the **dependency array**

---

## 8. Case 1: No Dependency Array

```jsx
useEffect(() => {
  console.log("Runs every render");
});
```

Behavior:

- ✔ Runs after **every render**
    
- ❌ Rarely used
    
- ⚠ Can cause **infinite loops** if state is updated inside effect
    

---

## 9. Case 2: Empty Dependency Array `[]`

```jsx
useEffect(() => {
  console.log("Runs once");
}, []);
```

Behavior:

- ✔ Runs **only once**
    
- ✔ Runs when component **mounts**
    

Used for:

- Fetching initial data
    
- Loading data from `localStorage`
    
- Adding event listeners
    

---

## 10. Case 3: Dependency Array with Values

```jsx
useEffect(() => {
  console.log("Runs when count changes");
}, [count]);
```

Behavior:

- ✔ Runs **only when dependency changes**
    
- ✔ React compares previous and current values
    

Used for:

- Saving data
    
- Calculations
    
- Watching specific state changes
    

---

## 11. Example: Auto-Saving to LocalStorage

```jsx
useEffect(() => {
  localStorage.setItem("subs", JSON.stringify(subs));
}, [subs]);
```

Explanation:

- Effect runs **only when `subs` changes**
    
- Prevents unnecessary writes
    
- Efficient and clean design
    

---

## 12. PhoneBook App – Demo Use Case

- Subscribers data stored in **state**
    
- On change:
    
    - Data saved to **localStorage**
        
- Achieved using:
    
    - `useState()` + `useEffect()`
        
- Demonstrates **real-world usage**
    

---

## 13. Common Mistakes with `useEffect()`

- Forgetting dependency array
    
- Updating state inside effect without dependencies
    
- Incorrect dependencies causing extra renders
    
- Ignoring cleanup functions
    

---

## 14. Cleanup in `useEffect()`

- Used to clean side effects
    
- Prevents memory leaks
    

```jsx
useEffect(() => {
  return () => {
    // cleanup code
  };
}, []);
```

Used for:

- Removing event listeners
    
- Clearing intervals / timeouts
    

---

## 15. Best Practices

- Keep effects **small & focused**
    
- Always specify dependencies
    
- Avoid unnecessary effects
    
- Prefer multiple effects instead of one big effect
    

---

# 📝 MCQs (15) – Single Correct

1. `useEffect()` is used to handle:
    

- A) State
    
- B) Props
    
- C) Side effects
    
- D) JSX  
    **Ans:** C
    

2. `useEffect()` runs:
    

- A) Before render
    
- B) During render
    
- C) After render
    
- D) Before DOM loads  
    **Ans:** C
    

3. Side effects include:
    

- A) JSX rendering
    
- B) Variable declaration
    
- C) API calls
    
- D) Returning JSX  
    **Ans:** C
    

4. Which hook replaces lifecycle methods?
    

- A) useState
    
- B) useEffect
    
- C) useRef
    
- D) useMemo  
    **Ans:** B
    

5. No dependency array causes effect to run:
    

- A) Once
    
- B) Never
    
- C) On dependency change
    
- D) After every render  
    **Ans:** D
    

6. Empty dependency array means:
    

- A) Runs every time
    
- B) Runs once on mount
    
- C) Runs on unmount
    
- D) Never runs  
    **Ans:** B
    

7. Dependency array controls:
    

- A) Styling
    
- B) JSX
    
- C) Execution timing
    
- D) Props  
    **Ans:** C
    

8. Which can cause infinite loop?
    

- A) useState
    
- B) Updating state in effect without deps
    
- C) JSX
    
- D) Props  
    **Ans:** B
    

9. useEffect() is available in:
    

- A) Class components
    
- B) Functional components
    
- C) HTML
    
- D) CSS  
    **Ans:** B
    

10. Correct syntax is:
    

- A) useEffect[]
    
- B) useEffect()
    
- C) useEffect{}
    
- D) useEffect<>  
    **Ans:** B
    

11. Cleanup function runs:
    

- A) Before render
    
- B) After render
    
- C) On unmount
    
- D) On mount only  
    **Ans:** C
    

12. LocalStorage save example should depend on:
    

- A) All state
    
- B) No state
    
- C) Specific variable
    
- D) Props only  
    **Ans:** C
    

13. Dependency values are compared using:
    

- A) Deep comparison
    
- B) Strict equality
    
- C) JSON comparison
    
- D) Reference only  
    **Ans:** B
    

14. useEffect() replaces:
    

- A) constructor
    
- B) componentDidMount
    
- C) componentDidUpdate
    
- D) All  
    **Ans:** D
    

15. Best practice is to:
    

- A) Avoid useEffect
    
- B) Use many effects
    
- C) Ignore dependencies
    
- D) Put all logic in one effect  
    **Ans:** B
    

---

# ☑️ Checkbox MCQs (15) – Multiple Correct

1. Side effects include:
    

- ☑ API calls
    
- ☑ LocalStorage
    
- ☑ Timers
    
- ⬜ JSX
    

2. useEffect():
    

- ☑ Runs after render
    
- ☑ Handles side effects
    
- ⬜ Runs during render
    
- ⬜ Replaces JSX
    

3. Dependency array:
    

- ☑ Controls execution
    
- ☑ Improves performance
    
- ⬜ Styles component
    
- ⬜ Is optional always
    

4. Empty dependency array:
    

- ☑ Runs once
    
- ☑ Good for data fetch
    
- ⬜ Runs every render
    
- ⬜ Runs on state change
    

5. No dependency array:
    

- ☑ Runs every render
    
- ⬜ Runs once
    
- ⬜ Runs on unmount
    
- ⬜ Recommended
    

6. useEffect() can:
    

- ☑ Save data
    
- ☑ Fetch data
    
- ☑ Add listeners
    
- ⬜ Return JSX
    

7. Cleanup function:
    

- ☑ Prevents memory leaks
    
- ☑ Removes listeners
    
- ⬜ Updates state
    
- ⬜ Renders UI
    

8. Dependency values:
    

- ☑ Compared using ===
    
- ⬜ Deep compared
    
- ⬜ Ignored
    
- ⬜ Random
    

9. useEffect() belongs to:
    

- ☑ React Hooks
    
- ⬜ Lifecycle only
    
- ⬜ DOM API
    
- ⬜ CSS
    

10. Multiple useEffect():
    

- ☑ Allowed
    
- ☑ Recommended
    
- ⬜ Forbidden
    
- ⬜ Deprecated
    

11. Real-world use cases:
    

- ☑ Auto-save
    
- ☑ API fetch
    
- ☑ Event handling
    
- ⬜ JSX formatting
    

12. Infinite loops occur when:
    

- ☑ State updated without deps
    
- ⬜ Empty deps
    
- ⬜ Cleanup used
    
- ⬜ JSX returned
    

13. Cleanup runs:
    

- ☑ On unmount
    
- ☑ Before next effect
    
- ⬜ During render
    
- ⬜ On state init
    

14. useEffect() improves:
    

- ☑ Control
    
- ☑ Performance
    
- ☑ Predictability
    
- ⬜ Compilation
    

15. Best practices:
    

- ☑ Small effects
    
- ☑ Correct deps
    
- ⬜ One big effect
    
- ⬜ Ignore warnings
    

---

# 🛑 ERROR IDENTIFICATION & SYNTAX MCQs (20)

```jsx
useEffect(() => {
  setCount(count + 1);
});
```

Error?

- A) Infinite loop
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
useEffect(() => {
}, count);
```

Error?

- A) Dependency not array
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
useEffect(() => {
  console.log("Hi");
}, []);
```

Error?

- A) No error
    
- B) Runs infinitely
    
- C) Syntax error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
useEffect(() => {
  localStorage.setItem("x", x);
}, []);
```

Error?

- A) Missing dependency
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
useEffect(() => {
  return console.log("cleanup");
}, []);
```

Error?

- A) Cleanup must be function
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
useEffect(() => {
}, {});
```

Error?

- A) Dependency must be array
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
useEffect(() => {
  fetchData();
}, [fetchData()]);
```

Error?

- A) Function invoked in deps
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
useEffect(() => {
  if (count > 0) return;
}, [count]);
```

Error?

- A) Cleanup misuse
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
useEffect(() => {
  setCount(count + 1);
}, [count]);
```

Error?

- A) Infinite loop
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
useEffect(() => {
  console.log("Run");
});
```

Error?

- A) Runs every render
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
useEffect(() => {
  return () => console.log("cleanup");
}, [x]);
```

Error?

- A) No error
    
- B) Cleanup wrong
    
- C) Syntax error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
useEffect(() => {
}, [a, b,]);
```

Error?

- A) No error
    
- B) Trailing comma invalid
    
- C) Syntax error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
useEffect(() => {
  localStorage.setItem("x", x);
});
```

Error?

- A) Missing dependency
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
useEffect(() => {
  return {};
}, []);
```

Error?

- A) Cleanup must be function
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
useEffect(async () => {
  await fetchData();
}, []);
```

Error?

- A) async directly in effect
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
useEffect(() => {
  setState();
}, []);
```

Error?

- A) Missing value
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** C
    

---

```jsx
useEffect(() => console.log("Hi"), []);
```

Error?

- A) No error
    
- B) Syntax error
    
- C) Logical error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
useEffect(() => {
  return () => {};
});
```

Error?

- A) No dependency array
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
useEffect(() => {
  document.addEventListener("click", fn);
}, []);
```

Error?

- A) Missing cleanup
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
useEffect(() => {
  setCount(prev => prev + 1);
}, []);
```

Error?

- A) No error
    
- B) Infinite loop
    
- C) Syntax error
    
- D) Logical error  
    **Ans:** A
    

---


---

# 📘 `useState()` & `useRef()` in React

_(Obsidian-Ready Notes)_

---

## 🔹 PART A — `useState()` Hook

---

## 1. What is `useState()`?

- `useState()` is a **React Hook**
    
- Used to add **state** to **functional components**
    
- Introduced in **React 16.8**
    
- Replaces `this.state` and `setState()` from class components
    

---

## 2. What is State?

- **State** is mutable data that controls component behavior
    
- When state changes:
    
    - Component **re-renders**
        
- State is **local** to a component
    

---

## 3. Basic Syntax of `useState()`

```jsx
const [state, setState] = useState(initialValue);
```

- `state` → current value
    
- `setState` → function to update value
    
- `initialValue` → used only on first render
    

---

## 4. Example

```jsx
const [count, setCount] = useState(0);

<button onClick={() => setCount(count + 1)}>
  Increment
</button>
```

- Clicking button updates state
    
- Component re-renders automatically
    

---

## 5. Rules of `useState()`

- Must be called:
    
    - At **top level**
        
    - Inside **functional component**
        
- ❌ Cannot be called inside:
    
    - Loops
        
    - Conditions
        
    - Nested functions
        

---

## 6. Updating State Correctly

### ❌ Wrong (stale state)

```jsx
setCount(count + 1);
```

### ✅ Correct (functional update)

```jsx
setCount(prev => prev + 1);
```

Used when new state depends on previous state.

---

## 7. Multiple State Variables

```jsx
const [name, setName] = useState("");
const [age, setAge] = useState(0);
```

- Better than using one large state object
    
- Improves readability
    

---

## 8. State with Objects

```jsx
const [user, setUser] = useState({ name: "", age: 0 });

setUser({ ...user, age: 21 });
```

⚠ State updates **do not merge automatically**

---

## 9. Why State Updates are Asynchronous

- React batches state updates for performance
    
- State update is **scheduled**, not immediate
    

---

## 🔹 PART B — `useRef()` Hook

---

## 10. What is `useRef()`?

- `useRef()` is a React Hook
    
- Used to store **mutable values**
    
- Does **NOT** trigger re-render on change
    

```jsx
const ref = useRef(initialValue);
```

---

## 11. Structure of `useRef()`

- Returns an object:
    

```js
{ current: value }
```

- Value stored in `.current`
    

---

## 12. Accessing DOM Elements (Main Use Case)

```jsx
const inputRef = useRef(null);

<input ref={inputRef} />

<button onClick={() => inputRef.current.focus()}>
  Focus
</button>
```

- Provides **direct DOM access**
    
- Replaces `document.getElementById()`
    

---

## 13. useRef vs useState

|Feature|useState|useRef|
|---|---|---|
|Triggers re-render|✅ Yes|❌ No|
|Mutable value|❌|✅|
|DOM access|❌|✅|
|UI updates|✅|❌|

---

## 14. Persisting Values Across Renders

- `useRef()` keeps value **between renders**
    
- Ideal for:
    
    - Timers
        
    - Previous values
        
    - Counters without UI change
        

```jsx
const renderCount = useRef(0);
renderCount.current++;
```

---

## 15. Common useRef Use Cases

- DOM manipulation
    
- Storing interval IDs
    
- Tracking previous state
    
- Avoiding unnecessary re-renders
    

---

## 16. When NOT to Use useRef

- When UI must update
    
- When value affects rendering
    

👉 Use `useState()` instead

---

# 📝 MCQs (15) – Single Correct

1. `useState()` is used to:
    

- A) Access DOM
    
- B) Manage state
    
- C) Handle effects
    
- D) Create refs  
    **Ans:** B
    

2. Updating state causes:
    

- A) No change
    
- B) Re-render
    
- C) Page reload
    
- D) DOM reset  
    **Ans:** B
    

3. `useState()` returns:
    

- A) Object
    
- B) Value only
    
- C) Array
    
- D) Function  
    **Ans:** C
    

4. `useRef()` returns:
    

- A) Value
    
- B) Array
    
- C) Object with current
    
- D) Function  
    **Ans:** C
    

5. Changing `useRef().current`:
    

- A) Re-renders component
    
- B) Throws error
    
- C) Does nothing
    
- D) Does NOT re-render  
    **Ans:** D
    

6. Which hook accesses DOM?
    

- A) useState
    
- B) useEffect
    
- C) useRef
    
- D) useMemo  
    **Ans:** C
    

7. Correct state update when dependent on previous:
    

- A) setState(value)
    
- B) setState(prev => …)
    
- C) state++
    
- D) updateState()  
    **Ans:** B
    

8. useState must be called:
    

- A) Anywhere
    
- B) Inside loops
    
- C) At top level
    
- D) Inside if  
    **Ans:** C
    

9. State updates are:
    

- A) Synchronous
    
- B) Immediate
    
- C) Asynchronous
    
- D) Blocking  
    **Ans:** C
    

10. Best hook for form input value:
    

- A) useRef
    
- B) useState
    
- C) useEffect
    
- D) useContext  
    **Ans:** B
    

11. useRef is mainly used for:
    

- A) UI rendering
    
- B) State updates
    
- C) DOM access
    
- D) Styling  
    **Ans:** C
    

12. Initial value of useState is used:
    

- A) Every render
    
- B) First render only
    
- C) On unmount
    
- D) On update  
    **Ans:** B
    

13. useRef value persists:
    

- A) Per render
    
- B) Per update
    
- C) Across renders
    
- D) Per function call  
    **Ans:** C
    

14. Which does NOT cause re-render?
    

- A) useState
    
- B) props change
    
- C) useRef
    
- D) context update  
    **Ans:** C
    

15. Best hook to store interval ID:
    

- A) useState
    
- B) useRef
    
- C) useEffect
    
- D) useMemo  
    **Ans:** B
    

---

# ☑️ Checkbox MCQs (15) – Multiple Correct

1. useState():
    

- ☑ Manages state
    
- ☑ Causes re-render
    
- ⬜ Accesses DOM
    
- ⬜ Stores mutable ref
    

2. State:
    

- ☑ Mutable
    
- ☑ Local
    
- ⬜ Global
    
- ⬜ Static
    

3. useState rules:
    

- ☑ Top level only
    
- ☑ Inside functional component
    
- ⬜ Inside loops
    
- ⬜ Inside conditions
    

4. useRef():
    

- ☑ Stores mutable value
    
- ☑ Does not re-render
    
- ☑ Accesses DOM
    
- ⬜ Manages UI state
    

5. useRef().current:
    

- ☑ Mutable
    
- ☑ Persistent
    
- ⬜ Triggers render
    
- ⬜ Read-only
    

6. State update:
    

- ☑ Asynchronous
    
- ☑ Batched
    
- ⬜ Immediate
    
- ⬜ Blocking
    

7. Good useState cases:
    

- ☑ Counter
    
- ☑ Form input
    
- ☑ Toggle UI
    
- ⬜ Interval ID
    

8. Good useRef cases:
    

- ☑ DOM focus
    
- ☑ Timer storage
    
- ☑ Previous value
    
- ⬜ UI rendering
    

9. useState with objects:
    

- ☑ Requires spread
    
- ⬜ Auto merge
    
- ☑ Replaces object
    
- ⬜ Immutable internally
    

10. useRef replaces:
    

- ☑ getElementById
    
- ⬜ querySelectorAll
    
- ⬜ useEffect
    
- ⬜ setState
    

11. Multiple states:
    

- ☑ Allowed
    
- ☑ Recommended
    
- ⬜ Forbidden
    
- ⬜ Deprecated
    

12. useRef value change:
    

- ☑ Silent
    
- ☑ No re-render
    
- ⬜ Causes update
    
- ⬜ Triggers effect
    

13. useState initial value:
    

- ☑ Used once
    
- ⬜ Used every render
    
- ⬜ Dynamic always
    
- ⬜ Optional
    

14. Hooks are:
    

- ☑ Functions
    
- ☑ React API
    
- ⬜ Classes
    
- ⬜ HTML
    

15. Correct choice:
    

- ☑ useState for UI
    
- ☑ useRef for non-UI
    
- ⬜ useRef for forms
    
- ⬜ useState for DOM
    

---

# 🛑 ERROR IDENTIFICATION & SYNTAX MCQs (20)

```jsx
const [count, setCount] = useState();
```

Error?

- A) Missing initial value
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** C
    

---

```jsx
setCount = count + 1;
```

Error?

- A) Wrong assignment
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
useState(0);
```

Error?

- A) Value not captured
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
if (x) {
  useState(0);
}
```

Error?

- A) Hook inside condition
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
const ref = useRef();
ref = 10;
```

Error?

- A) Should use ref.current
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
ref.current = ref.current + 1;
```

Error?

- A) No error
    
- B) Syntax error
    
- C) Logical error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
<input ref="myRef" />
```

Error?

- A) Invalid ref usage
    
- B) Syntax error
    
- C) No error
    
- D) Logical error  
    **Ans:** A
    

---

```jsx
const [state] = useState(0);
```

Error?

- A) Missing setter
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** C
    

---

```jsx
setCount(prev + 1);
```

Error?

- A) prev not defined
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
const ref = useRef(null);
ref.focus();
```

Error?

- A) Should use ref.current
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
const [a, b, c] = useState(0);
```

Error?

- A) Too many destructures
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
useRef(0, 1);
```

Error?

- A) Too many arguments
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
setState(state++);
```

Error?

- A) Mutating state
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
const ref = useRef();
ref.current();
```

Error?

- A) current is not function
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
const [x, setX] = useState;
```

Error?

- A) useState not invoked
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
const ref = useRef(null);
<input ref={ref.current} />
```

Error?

- A) Wrong ref binding
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
setCount(count + 1);
setCount(count + 1);
```

Error?

- A) Stale state issue
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
useRef = 10;
```

Error?

- A) Overwriting hook
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
const ref = useRef();
console.log(ref.value);
```

Error?

- A) Should use current
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** A
    

---

```jsx
const [state, setState] = useState(null);
setState();
```

Error?

- A) Missing value
    
- B) Syntax error
    
- C) No error
    
- D) Runtime error  
    **Ans:** C
    

---

