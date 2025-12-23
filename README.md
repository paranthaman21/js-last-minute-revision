# Last Minute Revision Guide: JavaScript Fundamentals, DOM, and Web Technologies (Enhanced with Examples)

## I. JavaScript Fundamentals

### 1. Variables and Values

| Concept | Description | Example |
| :--- | :--- | :--- |
| **Variable Declaration** | Variables are containers for storing values, created using `let`. | `let message;` |
| **Assignment** | Assign a value using `=`. | `let message = 'Hello Rahul';` |
| **Undefined** | Value of an unassigned variable. | `let message; // undefined` |
| **Primitive Types** | Number, Boolean, String, Undefined, Null. | `typeof(900); // number` |
| **Null** | Intentional empty value. | `let selectedColor = null;` |

### 2. Operators and Conversion

| Operator/Function | Usage | Example |
| :--- | :--- | :--- |
| `typeof()` | Find data type. | `typeof(a);` |
| `parseInt()` | Convert string → integer. | `parseInt('20');` |
| **Comparison** | Equality or strict equality. | `a === b` |
| **Logical Operators** | AND, OR, NOT. | `a && b` |
| **Conditionals** | Branching logic. | `if (conditionA) { ... } else { ... }` |
| **Math.ceil()** | Rounds up to next integer. | `Math.ceil(95.9); // 96` |

---

## II. Data Structures: Arrays and Objects

### 1. Arrays

| Action | Method/Property | Example |
| :--- | :--- | :--- |
| **Creation/Access** | Access by index. | `myArray[1];` |
| **Length** | Count items. | `myArray.length;` |
| **Add Items** | `push()` | `myArray.push(true);` |
| **Remove Items** | `pop()` | `myArray.pop();` |
| **Modify** | `splice()` | `myArray.splice(2, 0, 'one');` |
| **Find Index** | `findIndex()` | `arr.findIndex(fn);` |

### 2. Objects

| Concept | Details | Example |
| :--- | :--- | :--- |
| **Creation** | Key-value pairs. | `let person = { firstName: 'Rahul', age: 28 };` |
| **Dot Notation** | For valid identifiers. | `person.firstName;` |
| **Bracket Notation** | For dynamic or invalid keys. | `person['firstName'];` |
| **Missing Property** | Returns `undefined`. | `person.gender;` |
| **Modify/Add** | Update values. | `person.age = 29;` |
| **Destructuring** | Extract properties. | `let { age } = person;` |

---

## III. DOM and Event Handling

### 1. DOM

| Action | Method/Property | Example |
| :--- | :--- | :--- |
| **Select Element** | `getElementById()` | `document.getElementById('title');` |
| **Text Manipulation** | `textContent` | `title.textContent = 'Updated';` |
| **Style Manipulation** | `style` | `element.style.color = 'blue';` |
| **Set Attributes** | `setAttribute()` | `label.setAttribute('for','id');` |
| **Toggle Class** | `classList.toggle()` | `el.classList.toggle('active');` |
| **Remove Element** | `removeChild()` | `parent.removeChild(child);` |

### 2. Events and Listeners

| Concept | Details | Example |
| :--- | :--- | :--- |
| **Add Listener** | Modern approach. | `btn.addEventListener('click', fn);` |
| **Keyboard Events** | keydown/keyup. | `input.addEventListener('keydown', logKey);` |
| **Event Object** | Info about the event. | `event.key;` |
| **Prevent Default** | Block default browser behavior. | `event.preventDefault();` |

---

## IV. Execution, Callbacks, Schedulers

| Concept | Description | Example |
| :--- | :--- | :--- |
| **Execution Context** | Environment in which JS runs. | (Conceptual) |
| **Callback Function** | Function passed as argument. | `fn(() => console.log('Hi'));` |
| **setInterval()** | Run repeatedly. | `setInterval(() => console.log('Tick'), 1000);` |
| **clearInterval()** | Stop interval. | `clearInterval(id);` |

---

## V. Storage and Networking

### 1. Local Storage & JSON

| Concept | Description | Example |
| :--- | :--- | :--- |
| **Store** | Save key-value pair. | `localStorage.setItem('Key','Value');` |
| **Retrieve** | Get item. | `localStorage.getItem('Key');` |
| **Remove** | Delete by key. | `localStorage.removeItem('Key');` |
| **JSON Keys** | Must use double quotes. | `{"name":"Rahul"}` |
| **stringify()** | Convert to JSON string. | `JSON.stringify(obj);` |

### 2. HTTP & Fetch

| Concept | Details | Example |
| :--- | :--- | :--- |
| **HTTP/HTTPS** | Web communication protocols. | `https://example.com` |
| **HTTP Methods** | GET, POST, PUT, DELETE. | (Conceptual) |
| **Status Codes** | 200, 404, 500. | (Conceptual) |
| **fetch()** | Make a network request. | `fetch(url, options);` |
| **Response Object** | Access response details. | `response.status;` |

## Modern JavaScript Syntax Cheat Sheet


| Concept | Syntax/Key Structure | Description/Usage | Source Example |
| :--- | :--- | :--- | :--- |
| **Spread Operator (`...`)** | `...iterable` or `{...object}` | Unpacks an iterable into individual elements; used for copying, concatenation, or passing function arguments. | **Array:** `let arr3 = [...arr1, ...arr2];`<br>**Object:** `let personDetails = { ...person };`<br>**Function Args:** `add(...numbers);` |
| **Rest Parameter (`...`)** | `...rest` (must be last param) | Packs remaining values into an array in functions or destructuring. | **Function:** `function numbers(a, b, ...rest)`<br>**Array:** `let [a, b, ...rest] = arr;`<br>**Object:** `let { firstName, ...rest } = obj;` |
| **Arrow Functions** | `(param) => {}` | Shorter alternative to function expressions; implicit return when not using `{}`. | **Normal:** `let sum = (a, b) => { return a + b };`<br>**Implicit:** `let sum = (a, b) => a + b;`<br>**Return Object:** `name => ({ firstName: "Rahul" })` |
| **Default Parameters** | `function fn(param = default)` | Sets default parameter values when arguments are missing. | `function numbers(a = 2, b = 5)`<br>Call: `numbers(3);` (b becomes 5) |
| **Template Literals** | `` `Hello ${value}` `` | Backtick strings with embedding + multiline support. | `` console.log(`Hello ${firstName}!`) `` |
| **Ternary Operator** | `condition ? val1 : val2` | Short conditional alternative to `if...else`. | `let msg = speed >= 100 ? "Too Fast" : "OK";` |
| **Switch Statement** | `switch(value){case x:...}` | Multi-branch conditional; `break` prevents fall-through. | `case 1: console.log("Monday"); break;` |

## Object Creation Patterns

| Feature | Example Code | Key Takeaway |
| :--- | :--- | :--- |
| **Factory Function** | `function createCar(color, brand) { return { color, brand, start() { console.log("Car Started"); } }; }` | A function that returns an object directly. Uses shorthand property notation when variable and key names match. |
| **Constructor Function** | `function Car(color, brand) { this.color = color; this.brand = brand; } const carOne = new Car("blue", "Audi");` | Requires the `new` keyword. Properties are assigned using `this`. |
| **Function Properties** | `function Car(color, brand) {}`<br>`Car.name; // "Car"`<br>`Car.length; // 2` | Functions are objects. `name` returns function name, `length` returns parameter count. |

---

## Built-in Objects: Date

| Feature | Example Code | Key Takeaway |
| :--- | :--- | :--- |
| **Constructor Property** | `const dateObj = new Date();`<br>`dateObj.constructor === Date; // true` | Every object has a `constructor` property referencing its creator. |
| **Date Creation** | `new Date();`<br>`new Date(milliseconds);`<br>`new Date("YYYY-MM-DD");`<br>`new Date(year, month, day);` | Shows different ways to instantiate a Date object. |
| **Auto Correction** | `new Date(2006, 13, 32);` | JavaScript auto-corrects invalid month/day values. |
| **Instance Methods** | `let d1 = new Date(2020, 5, 15);`<br>`d1.getFullYear(); // 2020`<br>`d1.setFullYear(2021);` | `get` and `set` methods read and modify date values. |

## More Modern JavaScript Concepts | Part 3 | Cheat Sheet


### 1. `this` Keyword


| Scenario | Description | Example |
| :--- | :--- | :--- |
| **Object Method** | `this` refers to the object calling the method. | `let car = { color: 'blue', start() { console.log(this); } }; car.start();` |
| **Regular Function** | `this` refers to the global object (`window` in browsers). | `function start() { console.log(this); } start();` |
| **Arrow Function (Object Method)** | Arrow functions do not have their own `this`; they inherit from surrounding scope. | `let car = { start: () => console.log(this) }; car.start(); // window` |
| **Arrow Function (Callback)** | Inherits `this` from parent function. | `setTimeout(() => console.log(this), 1000);` |
| **Constructor Function** | `this` refers to the instance created using `new`. | `function Car(){ console.log(this); } new Car();` |
| **Arrow in Constructor** | Arrow inherits `this` from constructor context. | `this.start = () => console.log(this);` |


---


### 2. Immutable vs Mutable Values


| Type | Description | Example |
| :--- | :--- | :--- |
| **Immutable** | Primitive values cannot be changed. | `let x = 5; let y = x; y = 10; // x is still 5` |
| **Mutable** | Objects can be modified via references. | `let x = { v: 5 }; let y = x; y.v = 10; // x.v is 10` |


---


### 3. Declaring Variables


| Keyword | Rules | Example |
| :--- | :--- | :--- |
| **let** | Can be declared without initialization and reassigned. | `let x; x = 10; x = 15;` |
| **const** | Must be initialized and cannot be reassigned. | `const x = 7; // valid` |
| **const (Object Mutation)** | Object properties can change, reference cannot. | `const car = { color: 'blue' }; car.color = 'red';` |
| **Invalid const Reassignment** | Reassigning causes error. | `car = {}; // TypeError` |


