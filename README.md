# MERN-ASSESSMENT-QUESTIONS-AND-ANSWERS-
## react assessment questions

### Basic Questions

1.  What is React?

    -   React is a JavaScript library for building user interfaces, particularly single-page applications where you need a fast and interactive UI. It was developed by Facebook.
2.  What are the main features of React?

    -   Component-based architecture, Virtual DOM, Unidirectional data flow, JSX syntax, and React Hooks.
3.  What is JSX?

    -   JSX (JavaScript XML) is a syntax extension for JavaScript that allows you to write HTML-like code in your JavaScript files. It gets compiled into `React.createElement()` calls.
4.  Why is React called a "library" and not a "framework"?

    -   React focuses only on the view layer of an application, whereas frameworks like Angular or Vue provide a complete structure including routing, state management, etc.
5.  What is the difference between React and ReactDOM?

    -   `React` is the core library for creating components, while `ReactDOM` is responsible for rendering those components into the DOM.
6.  What is the virtual DOM?

    -   The virtual DOM is a lightweight copy of the real DOM. React uses it to optimize updates by comparing changes before applying them to the actual DOM.
7.  How does React's virtual DOM work?

    -   React creates a virtual DOM tree, compares it with the previous version (diffing), and then updates only the parts of the real DOM that have changed.
8.  What is a component in React?

    -   A component is a reusable piece of UI. It can be either a function or a class that returns JSX.
9.  What are functional components in React?

    -   Functional components are simple JavaScript functions that return JSX. They are stateless unless hooks are used.
10. What are class components in React?

    -   Class components are ES6 classes that extend `React.Component` and have lifecycle methods and state.
11. What is the difference between functional and class components?

    -   Functional components are simpler and use hooks for state and side effects, while class components use `this.state` and lifecycle methods.
12. What is props in React?

    -   Props (short for properties) are inputs passed to components. They are immutable and allow parent components to pass data to child components.
13. What is state in React?

    -   State is an object that holds data that may change over time. It is mutable and managed within the component.
14. How do you update the state in a class component?

    -   Use `this.setState({ key: value })`.
15. How do you update the state in a functional component?

    -   Use the `useState` hook: `setState(newValue)`.
16. What is the difference between props and state?

    -   Props are immutable and passed from parent to child, while state is mutable and managed within the component.
17. What is the purpose of `super()` in a React class component?

    -   `super()` calls the constructor of the parent class (`React.Component`) and initializes `this`.
18. What is the significance of keys in React lists?

    -   Keys help React identify which items have changed, been added, or removed, improving performance.
19. What happens if you don't provide a key to a list of elements in React?

    -   React will warn you in the console, and performance may degrade because React cannot efficiently track elements.
20. What is the difference between `map()` and `forEach()` when rendering lists in React?

    -   `map()` returns a new array of JSX elements, while `forEach()` does not return anything.

* * * * *

### Intermediate Questions

1.  What are React Hooks?

    -   Hooks are functions that let you use state and other React features without writing a class.
2.  What is the `useState` hook?

    -   `useState` allows functional components to manage state. Example: `const [state, setState] = useState(initialValue)`.
3.  What is the `useEffect` hook?

    -   `useEffect` lets you perform side effects (e.g., data fetching, subscriptions) in functional components.
4.  What is the `useContext` hook?

    -   `useContext` allows you to consume context values without wrapping components in a `Context.Consumer`.
5.  What is the `useReducer` hook?

    -   `useReducer` is an alternative to `useState` for managing complex state logic.
6.  What is the `useCallback` hook?

    -   `useCallback` memoizes a function to prevent unnecessary re-renders.
7.  What is the `useMemo` hook?

    -   `useMemo` memoizes a value to optimize performance.
8.  What is the `useRef` hook?

    -   `useRef` provides a mutable reference to a DOM element or a value that persists across renders.
9.  What is the difference between `useState` and `useReducer`?

    -   `useState` is simpler for managing small state, while `useReducer` is better for complex state logic.
10. When should you use `useCallback` and `useMemo`?

    -   Use `useCallback` for functions and `useMemo` for values to avoid unnecessary recalculations.
11. What is React Context?

    -   Context provides a way to pass data through the component tree without passing props manually at every level.
12. How do you create a context in React?

    -   Use `React.createContext(defaultValue)`.
13. How do you consume a context in React?

    -   Use `useContext(MyContext)` or wrap components in `<MyContext.Consumer>`.
14. What is the purpose of `React.memo`?

    -   `React.memo` prevents unnecessary re-renders of functional components by memoizing their output.
15. What is the difference between `React.memo` and `PureComponent`?

    -   `React.memo` is for functional components, while `PureComponent` is for class components.
16. What is prop drilling?

    -   Prop drilling is the process of passing props down multiple levels of nested components.
17. How can you avoid prop drilling?

    -   Use React Context or state management libraries like Redux.
18. What is the React lifecycle?

    -   The lifecycle refers to the stages a component goes through: mounting, updating, and unmounting.
19. What are the different phases of the React lifecycle?

    -   Mounting, Updating, and Unmounting.
20. What are the lifecycle methods in class components?

    -   `componentDidMount`, `componentDidUpdate`, `componentWillUnmount`, etc.
21. What are the equivalent hooks for lifecycle methods in functional components?

    -   `useEffect` replaces most lifecycle methods.
22. What is the `componentDidMount` lifecycle method used for?

    -   It runs after the component is mounted and is commonly used for data fetching.
23. What is the `componentDidUpdate` lifecycle method used for?

    -   It runs after the component updates and is used for side effects based on prop or state changes.
24. What is the `componentWillUnmount` lifecycle method used for?

    -   It runs before the component is removed from the DOM and is used for cleanup.
25. What is error boundary in React?

    -   Error boundaries catch JavaScript errors in child components and display a fallback UI.
26. How do you create an error boundary in React?

    -   Define a class component with `componentDidCatch` or `static getDerivedStateFromError`.
27. What is the purpose of `shouldComponentUpdate`?

    -   It determines whether a component should re-render based on prop or state changes.
28. What is the difference between controlled and uncontrolled components?

    -   Controlled components manage form data via state, while uncontrolled components use DOM references.
29. What is a higher-order component (HOC)?

    -   An HOC is a function that takes a component and returns a new component with additional props or behavior.
30. How do you create a higher-order component?

    -   Wrap a component inside another function and return the enhanced component.

* * * * *

### Advanced Questions

1.  What is Redux and how does it integrate with React?

    -   Redux is a state management library. It integrates with React via the `react-redux` package using `Provider` and `connect`.
2.  What is the Flux architecture?

    -   Flux is a unidirectional data flow architecture with actions, dispatcher, store, and view.
3.  What is the difference between Redux and Context API?

    -   Redux is more scalable and feature-rich, while Context API is simpler but less optimized for large-scale apps.
4.  What is middleware in Redux? Give an example.

    -   Middleware intercepts actions before they reach the reducer. Example: Redux Thunk for async actions.
5.  What is Redux Thunk?

    -   Redux Thunk allows you to write action creators that return functions instead of plain objects.
6.  What is Redux Saga?

    -   Redux Saga handles side effects using generator functions.
7.  What is the difference between Redux Thunk and Redux Saga?

    -   Thunk is simpler for basic async logic, while Saga is more powerful for complex workflows.
8.  What is the purpose of `connect()` in Redux?

    -   `connect()` connects a React component to the Redux store.
9.  What is the `Provider` component in Redux?

    -   `Provider` makes the Redux store available to the app.
10. What is the `combineReducers` function in Redux?

    -   It combines multiple reducers into a single root reducer.
11. What is the `store` in Redux?

    -   The store holds the entire state tree of the application.
12. What is the difference between `mapStateToProps` and `mapDispatchToProps`?

    -   `mapStateToProps` maps state to props, while `mapDispatchToProps` maps dispatch actions to props.
13. What is the purpose of `reselect` in Redux?

    -   Reselect creates memoized selectors to compute derived data.
14. What is React Router?

    -   React Router is a library for handling navigation and routing in React apps.
15. What is the difference between `BrowserRouter` and `HashRouter`?

    -   `BrowserRouter` uses the HTML5 history API, while `HashRouter` uses URL hashes.
16. How do you pass parameters via React Router?

    -   Use route params (`:id`) or query strings.
17. What is the difference between `push` and `replace` in React Router?

    -   `push` adds a new entry to the history stack, while `replace` replaces the current entry.
18. What is the purpose of `Switch` in React Router?

    -   `Switch` ensures only one route is rendered at a time.
19. What is lazy loading in React?

    -   Lazy loading delays the loading of non-critical components until they are needed.
20. How do you implement code splitting in React?

    -   Use `React.lazy` and `Suspense`.
21. What is React Suspense?

    -   Suspense allows components to wait for something (e.g., data fetching) before rendering.
22. What is the purpose of `React.lazy()`?

    -   `React.lazy()` dynamically imports components for lazy loading.
23. What is server-side rendering (SSR) in React?

    -   SSR renders React components on the server and sends HTML to the client.
24. What is Next.js and how does it relate to React?

    -   Next.js is a framework built on top of React that supports SSR, static site generation, and routing.
25. What is the difference between client-side rendering and server-side rendering?

    -   CSR renders on the client, while SSR renders on the server.
26. What is React Fiber?

    -   React Fiber is a reimplementation of React's reconciliation algorithm for better performance.
27. What is the difference between `ReactDOM.render()` and `ReactDOM.createRoot()`?

    -   `createRoot` is part of React 18's concurrent mode, while `render` is legacy.
28. What is concurrent mode in React?

    -   Concurrent mode allows React to interrupt rendering for higher-priority updates.
29. What is the difference between `useLayoutEffect` and `useEffect`?

    -   `useLayoutEffect` runs synchronously after DOM mutations, while `useEffect` runs asynchronously.
30. What is batching in React?

    -   Batching groups multiple state updates into a single re-render for performance.
31. What is the purpose of `React.StrictMode`?

    -   `StrictMode` highlights potential problems in the app during development.
32. What is the difference between `React.PureComponent` and `React.Component`?

    -   `PureComponent` implements `shouldComponentUpdate` with shallow comparison.
33. What is the difference between `setState` and `forceUpdate`?

    -   `setState` updates state and triggers re-render, while `forceUpdate` forces a re-render without changing state.
34. What is the difference between `setState` being asynchronous and synchronous?

    -   `setState` is asynchronous for performance optimization.
35. What is the purpose of `defaultProps`?

    -   `defaultProps` defines default values for props.
36. What is the difference between `defaultProps` and `props`?

    -   `defaultProps` provides fallback values, while `props` are passed explicitly.
37. What is the purpose of `PropTypes`?

    -   `PropTypes` validates the types of props passed to components.
38. How do you validate props using `PropTypes`?

    -   Example: `MyComponent.propTypes = { name: PropTypes.string }`.
39. What is the difference between `PropTypes` and TypeScript?

    -   `PropTypes` is runtime validation, while TypeScript is compile-time type checking.
40. What is the purpose of `React.Fragment`?

    -   `Fragment` groups children without adding extra nodes to the DOM.
41. What is the difference between `React.Fragment` and a `div`?

    -   `Fragment` doesn't create a DOM node, while `div` does.
42. What is the purpose of `React.Children`?

    -   `React.Children` provides utilities for working with `this.props.children`.
43. What is the difference between `React.Children.map` and `Array.prototype.map`?

    -   `React.Children.map` works with opaque data structures like `children`.
44. What is the purpose of `React.cloneElement`?

    -   `cloneElement` clones and modifies an element with new props.
45. What is the difference between `React.cloneElement` and `React.createElement`?

    -   `cloneElement` modifies existing elements, while `createElement` creates new ones.
46. What is the purpose of `React.forwardRef`?

    -   `forwardRef` forwards refs to child components.
47. What is the difference between `React.forwardRef` and `React.createRef`?

    -   `forwardRef` passes refs to child components, while `createRef` creates refs.
48. What is the purpose of `React.SuspenseList`?

    -   `SuspenseList` coordinates the loading order of multiple `Suspense` components.
49. What is the difference between `React.Suspense` and `React.SuspenseList`?

    -   `Suspense` handles individual components, while `SuspenseList` manages groups.
50. What is the future of React? 
    - Future trends include React Server Components, improved concurrent mode, and better developer tools.

## Node.js assessment quetions

### Basic Questions (20)

1.  What is Node.js?

    -   Node.js is a JavaScript runtime built on Chrome's V8 engine, allowing developers to run JavaScript on the server-side.
    -   It uses an event-driven, non-blocking I/O model, making it lightweight and efficient.
2.  What is NPM?

    -   NPM (Node Package Manager) is the default package manager for Node.js, used to install and manage libraries.
    -   It also provides a registry of reusable open-source packages.
3.  What is the difference between Node.js and JavaScript?

    -   JavaScript is a programming language primarily used in browsers, while Node.js is a runtime environment for executing JavaScript on the server.
    -   Node.js extends JavaScript's capabilities to handle file systems, networking, and other server-side tasks.
4.  What is an event loop in Node.js?

    -   The event loop allows Node.js to perform non-blocking I/O operations by offloading tasks to the system kernel.
    -   It continuously checks the call stack and processes asynchronous callbacks when the stack is empty.
5.  What is REPL in Node.js?

    -   REPL (Read-Eval-Print-Loop) is an interactive shell for executing JavaScript code in real-time.
    -   It's useful for testing small snippets of code without creating files.
6.  What is the purpose of the `module.exports` object?

    -   `module.exports` is used to export functions, objects, or values from a module so they can be imported elsewhere.
    -   It enables modularity and code reuse in Node.js applications.
7.  What is the difference between `require` and `import`?

    -   `require` is CommonJS syntax for importing modules, while `import` is ES6 syntax.
    -   `import` supports static analysis and tree-shaking, whereas `require` is dynamic.
8.  What is a callback function in Node.js?

    -   A callback is a function passed as an argument to another function and executed after an asynchronous operation completes.
    -   It helps manage asynchronous behavior in Node.js.
9.  What is the purpose of the `process` object?

    -   The `process` object provides information about the current Node.js process, such as environment variables and command-line arguments.
    -   It also allows interaction with the system, like exiting the process or handling signals.
10. What is the `__dirname` variable?

    -   `__dirname` contains the absolute path of the directory containing the currently executing file.
    -   It's commonly used to construct file paths dynamically.
11. What is the `fs` module used for?

    -   The `fs` module provides APIs for interacting with the file system, such as reading, writing, and deleting files.
    -   It supports both synchronous and asynchronous methods.
12. What is the difference between synchronous and asynchronous methods in Node.js?

    -   Synchronous methods block the execution of subsequent code until the operation completes, while asynchronous methods do not.
    -   Asynchronous methods improve performance by avoiding blocking behavior.
13. What is the `http` module in Node.js?

    -   The `http` module allows you to create HTTP servers and clients for handling web requests and responses.
    -   It's the foundation for building web servers in Node.js.
14. What is middleware in Node.js?

    -   Middleware functions process requests and responses in the request-response cycle.
    -   They are commonly used in frameworks like Express.js for tasks like logging, authentication, and error handling.
15. What is the purpose of the `package.json` file?

    -   The `package.json` file defines metadata about a Node.js project, including dependencies, scripts, and versioning.
    -   It serves as the blueprint for managing the project and its dependencies.
16. What is the difference between `dependencies` and `devDependencies` in `package.json`?

    -   `dependencies` are required for production, while `devDependencies` are only needed during development.
    -   Example: Testing libraries like Jest are typically listed under `devDependencies`.
17. What is the `os` module used for?

    -   The `os` module provides utilities for interacting with the operating system, such as retrieving CPU, memory, and network information.
    -   It's useful for system-level monitoring and diagnostics.
18. What is the purpose of the `path` module?

    -   The `path` module provides utilities for working with file and directory paths, such as joining or normalizing paths.
    -   It ensures cross-platform compatibility for file paths.
19. What is the difference between `setImmediate` and `setTimeout`?

    -   `setImmediate` executes a callback immediately after the current poll phase, while `setTimeout` schedules execution after a delay.
    -   Their order depends on the event loop phase.
20. What is the purpose of the `Buffer` class?

    -   The `Buffer` class handles binary data directly in Node.js, such as reading/writing files or network streams.
    -   It's essential for working with raw data like images or protocols.

* * * * *

### Intermediate Questions (50)

1.  What is the event emitter in Node.js?

    -   The `EventEmitter` class allows objects to emit and listen for custom events.
    -   It's widely used in Node.js core modules like `http` and `stream`.
2.  How does the `cluster` module work?

    -   The `cluster` module enables multi-threading in Node.js by creating child processes that share the same server port.
    -   It improves performance by utilizing multiple CPU cores.
3.  What is the purpose of the `child_process` module?

    -   The `child_process` module allows spawning new processes and executing system commands.
    -   It's useful for running external scripts or programs.
4.  What is the difference between `spawn` and `exec` in the `child_process` module?

    -   `spawn` streams data in real-time and is better for large outputs, while `exec` buffers the output and is simpler for small tasks.
    -   Use `spawn` for long-running processes and `exec` for short commands.
5.  What is the purpose of the `crypto` module?

    -   The `crypto` module provides cryptographic functionality like hashing, encryption, and decryption.
    -   It's commonly used for securing sensitive data.
6.  What is the `zlib` module used for?

    -   The `zlib` module compresses and decompresses data using algorithms like gzip and deflate.
    -   It's useful for optimizing file sizes and network bandwidth.
7.  What is the purpose of the `net` module?

    -   The `net` module creates TCP servers and clients for low-level networking.
    -   It's used for custom protocols and communication between servers.
8.  What is the difference between `http` and `https` modules?

    -   The `http` module handles unencrypted HTTP traffic, while the `https` module adds SSL/TLS encryption for secure communication.
    -   `https` requires certificates for encryption.
9.  What is the purpose of the `dns` module?

    -   The `dns` module resolves domain names to IP addresses and performs reverse lookups.
    -   It's essential for network communication and DNS-based services.
10. What is the `stream` module used for?

    -   The `stream` module handles streaming data, such as reading/writing files or network sockets.
    -   It improves performance by processing data in chunks rather than loading everything into memory.
11. What are the types of streams in Node.js?

    -   There are four types: Readable, Writable, Duplex (both readable and writable), and Transform (modifies data as it passes through).
    -   Streams enable efficient handling of large datasets.
12. What is the purpose of the `util` module?

    -   The `util` module provides utility functions for debugging, inheritance, and type checking.
    -   Example: `util.promisify` converts callback-based functions into promises.
13. What is the difference between `console.log` and `process.stdout.write`?

    -   `console.log` appends a newline character after output, while `process.stdout.write` does not.
    -   Use `stdout.write` for custom formatting without newlines.
14. What is the purpose of the `assert` module?

    -   The `assert` module provides assertion functions for testing conditions in your code.
    -   It throws errors if assertions fail, helping with debugging.
15. What is the difference between `throw` and `process.exit`?

    -   `throw` raises an exception that can be caught, while `process.exit` terminates the Node.js process immediately.
    -   Use `process.exit` sparingly, as it prevents cleanup.
16. What is the purpose of the `global` object?

    -   The `global` object provides global variables accessible across all modules in a Node.js application.
    -   Example: `global.setTimeout` is equivalent to `setTimeout`.
17. What is the difference between `null` and `undefined` in Node.js?

    -   `null` represents an intentional absence of value, while `undefined` indicates an uninitialized or missing value.
    -   Always use `null` explicitly when clearing variables.
18. What is the purpose of the `vm` module?

    -   The `vm` module allows running JavaScript code in a sandboxed environment.
    -   It's useful for evaluating untrusted code securely.
19. What is the difference between `readFile` and `createReadStream`?

    -   `readFile` reads the entire file into memory, while `createReadStream` reads data in chunks.
    -   Use `createReadStream` for large files to avoid memory issues.
20. What is the purpose of the `worker_threads` module?

    -   The `worker_threads` module enables multithreading in Node.js by running JavaScript code in parallel threads.
    -   It's ideal for CPU-intensive tasks like image processing.
21. What is the difference between `Promise.all` and `Promise.race`?

    -   `Promise.all` waits for all promises to resolve, while `Promise.race` resolves as soon as one promise resolves or rejects.
    -   Use `Promise.all` for batch operations and `Promise.race` for timeouts.
22. What is the purpose of the `async_hooks` module?

    -   The `async_hooks` module tracks asynchronous resources and their lifecycle events.
    -   It's useful for debugging and profiling asynchronous workflows.
23. What is the difference between `uncaughtException` and `unhandledRejection`?

    -   `uncaughtException` handles uncaught synchronous errors, while `unhandledRejection` handles unhandled promise rejections.
    -   Both should be handled carefully to avoid crashing the application.
24. What is the purpose of the `perf_hooks` module?

    -   The `perf_hooks` module measures performance metrics like execution time and resource usage.
    -   It's useful for optimizing critical parts of the application.
25. What is the difference between `setTimeout` and `setInterval`?

    -   `setTimeout` executes a callback once after a delay, while `setInterval` executes it repeatedly at intervals.
    -   Clear intervals/timers to prevent memory leaks.
26. What is the purpose of the `domain` module?

    -   The `domain` module groups related I/O operations and handles errors within them.
    -   It's deprecated but was used for centralized error handling.
27. What is the difference between `writeFileSync` and `writeFile`?

    -   `writeFileSync` blocks the event loop until the file is written, while `writeFile` is asynchronous.
    -   Prefer `writeFile` for non-blocking behavior.
28. What is the purpose of the `tls` module?

    -   The `tls` module implements Transport Layer Security (TLS) for secure communication.
    -   It's used for encrypted connections like HTTPS.
29. What is the difference between `nextTick` and `setImmediate`?

    -   `process.nextTick` runs before the event loop continues, while `setImmediate` runs after the current poll phase.
    -   Use `nextTick` for immediate execution within the current phase.
30. What is the purpose of the `v8` module?

    -   The `v8` module exposes V8 engine APIs for memory statistics and garbage collection.
    -   It's useful for monitoring and optimizing memory usage.

* * * * *

### Advanced Questions (30)

1.  What is the difference between `fork` and `spawn` in the `child_process` module?

    -   `fork` creates a new Node.js process with IPC communication, while `spawn` starts a generic process.
    -   Use `fork` for Node.js-specific tasks and `spawn` for system commands.
2.  What is the purpose of the `inspector` module?

    -   The `inspector` module integrates with debugging tools like Chrome DevTools.
    -   It's useful for diagnosing performance bottlenecks and runtime errors.
3.  What is the difference between `readline` and `stdin`?

    -   `readline` provides an interface for reading input line-by-line, while `stdin` is a raw stream.
    -   Use `readline` for interactive CLI applications.
4.  What is the purpose of the `diagnostics_channel` module?

    -   The `diagnostics_channel` module enables publishing and subscribing to diagnostic events.
    -   It's useful for monitoring internal application events.
5.  What is the difference between `AbortController` and `clearTimeout`?

    -   `AbortController` cancels ongoing operations like fetch requests, while `clearTimeout` stops scheduled timers.
    -   Use `AbortController` for modern async cancellation.
6.  What is the purpose of the `trace_events` module?

    -   The `trace_events` module generates trace logs for performance analysis.
    -   It's useful for profiling and identifying bottlenecks.
7.  What is the difference between `EventEmitter` and `Stream`?

    -   `EventEmitter` emits custom events, while `Stream` handles data flow in chunks.
    -   Streams extend `EventEmitter` for data processing.
8.  What is the purpose of the `report` module?

    -   The `report` module generates diagnostic reports for crashes, memory leaks, and performance issues.
    -   It's useful for post-mortem debugging.
9.  What is the difference between `Buffer.alloc` and `Buffer.from`?

    -   `Buffer.alloc` creates a zero-filled buffer, while `Buffer.from` initializes it with provided data.
    -   Use `Buffer.alloc` for safe allocations.
10. What is the purpose of the `policy` module?

    -   The `policy` module enforces security policies like CSP (Content Security Policy).
    -   It's useful for hardening applications against vulnerabilities.
11. What is the difference between `URLSearchParams` and `querystring`?

    -   `URLSearchParams` is part of the WHATWG URL API, while `querystring` is Node.js-specific.
    -   Prefer `URLSearchParams` for modern applications.
12. What is the purpose of the `wasi` module?

    -   The `wasi` module provides WebAssembly System Interface (WASI) bindings.
    -   It's useful for running WebAssembly modules with system access.
13. What is the difference between `TextDecoder` and `StringDecoder`?

    -   `TextDecoder` is part of the WHATWG Encoding API, while `StringDecoder` is Node.js-specific.
    -   Use `TextDecoder` for modern encoding/decoding.
14. What is the purpose of the `addons` module?

    -   The `addons` module allows integrating C++ code with Node.js for performance-critical tasks.
    -   It's useful for extending Node.js functionality.
15. What is the difference between `MessageChannel` and `EventEmitter`?

    -   `MessageChannel` facilitates inter-process communication, while `EventEmitter` handles custom events.
    -   Use `MessageChannel` for structured messaging.
16. What is the purpose of the `dgram` module?

    -   The `dgram` module implements UDP (User Datagram Protocol) for lightweight communication.
    -   It's useful for real-time applications like gaming.
17. What is the difference between `Readable` and `Writable` streams?

    -   `Readable` streams produce data, while `Writable` streams consume data.
    -   Combine them for data pipelines.
18. What is the purpose of the `punycode` module?

    -   The `punycode` module encodes/decodes Unicode domain names for compatibility.
    -   It's deprecated but still relevant for legacy systems.
19. What is the difference between `BigInt` and `Number`?

    -   `BigInt` supports arbitrary-precision integers, while `Number` has limited precision.
    -   Use `BigInt` for calculations exceeding `Number.MAX_SAFE_INTEGER`.
20. What is the purpose of the `constants` module?

    -   The `constants` module provides predefined constants for error codes, file modes, etc.
    -   It simplifies working with system-level configurations.
21. What is the difference between `Error.captureStackTrace` and `new Error`?

    -   `Error.captureStackTrace` captures the stack trace without creating a new error instance.
    -   Use it for custom error classes.
22. What is the purpose of the `repl` module?

    -   The `repl` module creates custom REPL environments programmatically.
    -   It's useful for building interactive tools.
23. What is the difference between `Object.freeze` and `Object.seal`?

    -   `Object.freeze` prevents modifications entirely, while `Object.seal` allows property updates but disallows additions/removals.
    -   Use them for immutability.
24. What is the purpose of the `timers/promises` module?

    -   The `timers/promises` module provides promise-based timers like `setTimeout` and `setInterval`.
    -   It's useful for modern async workflows.
25. What is the difference between `WeakMap` and `Map`?

    -   `WeakMap` holds weak references to keys, allowing garbage collection, while `Map` retains strong references.
    -   Use `WeakMap` for memory-efficient caching.
26. What is the purpose of the `intl` module?

    -   The `intl` module provides internationalization APIs for formatting dates, numbers, and strings.
    -   It's useful for localization.
27. What is the difference between `Proxy` and `Reflect`?

    -   `Proxy` intercepts and customizes operations on objects, while `Reflect` provides low-level methods for those operations.
    -   Use them together for advanced metaprogramming.
28. What is the purpose of the `worker_data` property?

    -   The `worker_data` property passes initial data to worker threads.
    -   It's useful for initializing thread-specific configurations.
29. What is the difference between `SharedArrayBuffer` and `ArrayBuffer`?

    -   `SharedArrayBuffer` allows shared memory access across threads, while `ArrayBuffer` is isolated.
    -   Use `SharedArrayBuffer` for thread-safe operations.
30. What is the purpose of the `finalizationRegistry` API?

    -   The `FinalizationRegistry` API registers callbacks for objects when they are garbage collected.
    -   It's useful for cleanup tasks.
31. What is the difference between `Atomics` and `Mutex`?

    -   `Atomics` provides low-level atomic operations for shared memory, while `Mutex` ensures mutual exclusion.
    -   Use `Atomics` for fine-grained control.
32. What is the purpose of the `structuredClone` API?

    -   The `structuredClone` API deep clones objects, including complex types like arrays and maps.
    -   It's useful for copying immutable data structures.
33. What is the difference between `AbortSignal` and `AbortController`?

    -   `AbortSignal` represents the signal state, while `AbortController` manages the signal.
    -   Use them together for canceling operations.
34. What is the purpose of the `queueMicrotask` API?

    -   The `queueMicrotask` API schedules microtasks for execution after the current script.
    -   It's useful for prioritizing tasks.
35. What is the difference between `Blob` and `Buffer`?

    -   `Blob` represents immutable binary data, while `Buffer` is mutable and Node.js-specific.
    -   Use `Blob` for modern APIs.
36. What is the purpose of the `performance` module?

    -   The `performance` module measures high-resolution timestamps for performance analysis.
    -   It's useful for benchmarking.
37. What is the difference between `TextEncoder` and `Buffer`?

    -   `TextEncoder` encodes strings into `Uint8Array`, while `Buffer` provides Node.js-specific encoding/decoding.
    -   Use `TextEncoder` for browser-compatible code.
38. What is the purpose of the `WebSocket` module?

    -   The `WebSocket` module enables bidirectional communication over a single connection.
    -   It's useful for real-time applications.
39. What is the difference between `BroadcastChannel` and `MessageChannel`?

    -   `BroadcastChannel` broadcasts messages across browsing contexts, while `MessageChannel` facilitates direct communication.
    -   Use `BroadcastChannel` for multi-tab apps.
40. What is the purpose of the `crypto.randomUUID` method?

    -   The `crypto.randomUUID` method generates universally unique identifiers (UUIDs).
    -   It's useful for generating IDs securely.
41. What is the difference between `Symbol.asyncIterator` and `Symbol.iterator`?

    -   `Symbol.asyncIterator` defines asynchronous iteration, while `Symbol.iterator` defines synchronous iteration.
    -   Use `Symbol.asyncIterator` for async generators.
42. What is the purpose of the `Intl.Segmenter` API?

    -   The `Intl.Segmenter` API segments text into graphemes, words, or sentences based on locale.
    -   It's useful for text processing.
43. What is the difference between `AbortController.abort()` and `AbortSignal.throwIfAborted()`?

    -   `AbortController.abort()` triggers the abort signal, while `AbortSignal.throwIfAborted()` throws an error if aborted.
    -   Use them together for robust cancellation.
44. What is the purpose of the `Intl.DateTimeFormat` API?

    -   The `Intl.DateTimeFormat` API formats dates and times based on locale.
    -   It's useful for localization.
45. What is the difference between `BigInt.asIntN` and `BigInt.asUintN`?

    -   `BigInt.asIntN` clamps to signed integers, while `BigInt.asUintN` clamps to unsigned integers.
    -   Use them for bitwise operations.
46. What is the purpose of the `Intl.NumberFormat` API?

    -   The `Intl.NumberFormat` API formats numbers based on locale.
    -   It's useful for currency and unit formatting.
47. What is the difference between `Intl.PluralRules` and `Intl.RelativeTimeFormat`?

    -   `Intl.PluralRules` determines plural categories, while `Intl.RelativeTimeFormat` formats relative times.
    -   Use them for localization.
48. What is the purpose of the `Intl.ListFormat` API?

    -   The `Intl.ListFormat` API formats lists of items based on locale.
    -   It's useful for displaying localized lists.
49. What is the difference between `Intl.Collator` and `Intl.Locale`?

    -   `Intl.Collator` compares strings based on locale, while `Intl.Locale` represents locale information.
    -   Use them for sorting and locale handling.
50. What is the future of Node.js? 
    - Node.js continues to evolve with features like WebAssembly integration, improved performance, and enhanced security. 
    - Expect more alignment with modern JavaScript standards and broader adoption in enterprise application

## MongoDB and Mongoose assessment questions

### Basic Questions (15)

1.  What is MongoDB?

    -   MongoDB is a NoSQL database that stores data in flexible, JSON-like documents.
    -   It is schema-less and supports dynamic queries, making it ideal for unstructured or semi-structured data.
2.  What is a document in MongoDB?

    -   A document is a BSON (Binary JSON) object that represents a single record in MongoDB.
    -   Documents are stored in collections, similar to rows in relational databases.
3.  What is a collection in MongoDB?

    -   A collection is a group of documents stored in MongoDB, analogous to tables in relational databases.
    -   Collections do not enforce a strict schema, allowing flexibility in document structure.
4.  What is Mongoose?

    -   Mongoose is an ODM (Object Data Modeling) library for MongoDB and Node.js.
    -   It provides schema validation, middleware, and easier querying for MongoDB.
5.  What is the difference between SQL and NoSQL databases?

    -   SQL databases use structured tables with predefined schemas, while NoSQL databases like MongoDB store data in flexible documents.
    -   NoSQL databases are better suited for scalability and handling unstructured data.
6.  What is BSON in MongoDB?

    -   BSON (Binary JSON) is a binary-encoded serialization of JSON-like documents used by MongoDB.
    -   It supports additional data types like dates and binary data, which are not natively supported in JSON.
7.  How do you connect to a MongoDB database using Mongoose?

    -   Use `mongoose.connect('mongodb://<connection-string>')` to establish a connection.
    -   Example: `mongoose.connect('mongodb://localhost:27017/mydb')`.
8.  What is the purpose of the `_id` field in MongoDB?

    -   The `_id` field is a unique identifier for each document in a collection.
    -   If not provided, MongoDB automatically generates an ObjectId for the `_id`.
9.  What is an ObjectId in MongoDB?

    -   An ObjectId is a 12-byte identifier used as the default value for the `_id` field.
    -   It consists of a timestamp, machine identifier, process ID, and random value.
10. How do you insert a document into a MongoDB collection?

    -   Use the `insertOne()` or `insertMany()` methods.
    -   Example: `db.collection.insertOne({ name: "John", age: 30 })`.
11. How do you query documents in MongoDB?

    -   Use the `find()` method with optional filter criteria.
    -   Example: `db.collection.find({ age: { $gt: 25 } })`.
12. What is the `find()` method in MongoDB?

    -   The `find()` method retrieves all documents that match a query.
    -   It returns a cursor, which can be iterated to access results.
13. What is the `findOne()` method in MongoDB?

    -   The `findOne()` method retrieves the first document that matches a query.
    -   Example: `db.collection.findOne({ name: "John" })`.
14. How do you update a document in MongoDB?

    -   Use the `updateOne()` or `updateMany()` methods with a filter and update operation.
    -   Example: `db.collection.updateOne({ name: "John" }, { $set: { age: 35 } })`.
15. How do you delete a document in MongoDB?

    -   Use the `deleteOne()` or `deleteMany()` methods with a filter.
    -   Example: `db.collection.deleteOne({ name: "John" })`.

* * * * *

### Intermediate Questions (20)

1.  What is indexing in MongoDB?

    -   Indexing improves query performance by creating a data structure that allows faster lookups.
    -   Example: `db.collection.createIndex({ name: 1 })`.
2.  What is the difference between `createIndex` and `ensureIndex`?

    -   `createIndex` creates a new index if it doesn't exist, while `ensureIndex` is deprecated and replaced by `createIndex`.
    -   Always use `createIndex` in modern MongoDB versions.
3.  What is aggregation in MongoDB?

    -   Aggregation processes data records and returns computed results, such as sums, averages, or grouped data.
    -   Example: `db.collection.aggregate([{ $group: { _id: "$category", total: { $sum: "$price" } } }])`.
4.  What is the `$match` stage in aggregation?

    -   The `$match` stage filters documents based on specified criteria.
    -   Example: `{ $match: { age: { $gt: 25 } } }`.
5.  What is the `$group` stage in aggregation?

    -   The `$group` stage groups documents by a specified key and performs calculations like sum or average.
    -   Example: `{ $group: { _id: "$category", total: { $sum: "$price" } } }`.
6.  What is sharding in MongoDB?

    -   Sharding distributes data across multiple servers to improve scalability and performance.
    -   It splits large datasets into smaller chunks called shards.
7.  What is replication in MongoDB?

    -   Replication maintains multiple copies of data across different servers for fault tolerance.
    -   A replica set consists of primary and secondary nodes.
8.  What is the role of the primary node in a replica set?

    -   The primary node handles all write operations and replicates changes to secondary nodes.
    -   Secondary nodes can serve read operations if configured.
9.  What is the `populate()` method in Mongoose?

    -   The `populate()` method replaces references (e.g., ObjectIds) with actual documents from another collection.
    -   Example: `User.findById(id).populate('posts')`.
10. What is a schema in Mongoose?

    -   A schema defines the structure of documents, including fields, data types, and validation rules.
    -   Example: `const userSchema = new mongoose.Schema({ name: String, age: Number })`.
11. What is middleware in Mongoose?

    -   Middleware are functions executed before or after certain lifecycle events, such as saving or validating a document.
    -   Example: `schema.pre('save', function(next) { ... })`.
12. What are virtuals in Mongoose?

    -   Virtuals are document properties that are not stored in the database but computed dynamically.
    -   Example: `userSchema.virtual('fullName').get(() =>` this.firstName{this.lastName}`)`.
13. What is the difference between `save()` and `insertMany()` in Mongoose?

    -   `save()` persists a single document instance, while `insertMany()` inserts multiple documents at once.
    -   Use `insertMany()` for bulk inserts to improve performance.
14. What is the purpose of the `timestamps` option in Mongoose?

    -   The `timestamps` option automatically adds `createdAt` and `updatedAt` fields to documents.
    -   Example: `const schema = new Schema({}, { timestamps: true })`.
15. What is the difference between `findByIdAndUpdate` and `findOneAndUpdate`?

    -   `findByIdAndUpdate` updates a document by its `_id`, while `findOneAndUpdate` uses any filter criteria.
    -   Example: `Model.findByIdAndUpdate(id, { $set: { name: "John" } })`.
16. What is the `lean()` method in Mongoose?

    -   The `lean()` method returns plain JavaScript objects instead of Mongoose documents, improving performance.
    -   Example: `Model.find().lean()`.
17. What is the `distinct()` method in MongoDB?

    -   The `distinct()` method retrieves unique values for a specified field.
    -   Example: `db.collection.distinct("category")`.
18. What is the `$lookup` stage in aggregation?

    -   The `$lookup` stage performs a left outer join with another collection.
    -   Example: `{ $lookup: { from: "orders", localField: "userId", foreignField: "_id", as: "userOrders" } }`.
19. What is the `$unwind` stage in aggregation?

    -   The `$unwind` stage deconstructs an array field into separate documents for each element.
    -   Example: `{ $unwind: "$tags" }`.
20. What is the difference between `drop()` and `deleteMany()`?

    -   `drop()` deletes an entire collection, while `deleteMany()` removes specific documents.
    -   Use `drop()` with caution, as it cannot be undone.

* * * * *

### Advanced Questions (15)

1.  What is TTL (Time-To-Live) in MongoDB?

    -   TTL indexes automatically remove documents after a specified duration.
    -   Example: `db.collection.createIndex({ createdAt: 1 }, { expireAfterSeconds: 3600 })`.
2.  What is the `explain()` method in MongoDB?

    -   The `explain()` method provides detailed information about query execution plans.
    -   Example: `db.collection.find().explain("executionStats")`.
3.  What is the difference between `capped collections` and regular collections?

    -   Capped collections have a fixed size and overwrite old documents when full, while regular collections grow indefinitely.
    -   Use capped collections for logging or caching.
4.  What is the `bulkWrite()` method in MongoDB?

    -   The `bulkWrite()` method performs multiple write operations in a single request.
    -   Example: `db.collection.bulkWrite([{ insertOne: { document: { name: "John" } } }])`.
5.  What is the `changeStream` API in MongoDB?

    -   The `changeStream` API listens for real-time changes to documents in a collection.
    -   Example: `const changeStream = db.collection.watch()`.
6.  What is the difference between `embedded` and `referenced` relationships in MongoDB?

    -   Embedded relationships store related data within the same document, while referenced relationships link documents via ObjectIds.
    -   Use embedding for one-to-few relationships and referencing for one-to-many.
7.  What is the `text` index in MongoDB?

    -   A `text` index enables full-text search on string fields.
    -   Example: `db.collection.createIndex({ description: "text" })`.
8.  What is the `hint()` method in MongoDB?

    -   The `hint()` method forces MongoDB to use a specific index for a query.
    -   Example: `db.collection.find().hint({ name: 1 })`.
9.  What is the `collation` option in MongoDB?

    -   The `collation` option specifies language-specific rules for string comparison, such as case insensitivity.
    -   Example: `db.collection.find({}, { collation: { locale: "en", strength: 2 } })`.
10. What is the `gridfs` module in MongoDB?

    -   GridFS is a specification for storing and retrieving large files, such as images or videos, exceeding the BSON size limit.
    -   It splits files into chunks and stores them in separate collections.
11. What is the `pre` and `post` middleware in Mongoose?

    -   `pre` middleware runs before an operation (e.g., save), while `post` middleware runs after.
    -   Example: `schema.post('save', function(doc) { console.log('Saved:', doc) })`.
12. What is the `discriminator` feature in Mongoose?

    -   Discriminators allow multiple schemas to share the same collection but differ in structure.
    -   Example: `const subSchema = new Schema({ type: String }); const SubModel = Base.discriminator('Sub', subSchema)`.
13. What is the `versionKey` in Mongoose?

    -   The `versionKey` (`__v`) tracks the version of a document to handle optimistic concurrency control.
    -   You can disable it using `versionKey: false` in the schema options.
14. What is the `aggregate()` method in Mongoose?

    -   The `aggregate()` method performs complex data transformations using the MongoDB aggregation pipeline.
    -   Example: `Model.aggregate([{ $group: { _id: "$category", total: { $sum: "$price" } } }])`.
15. What is the future of MongoDB and Mongoose?

    -   MongoDB continues to evolve with features like serverless deployments, enhanced analytics, and improved security.
    -   Mongoose is expected to support more advanced TypeScript integrations and performance optimizations.

