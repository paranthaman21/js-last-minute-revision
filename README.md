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
