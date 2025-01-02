
# 1. Set
### A Set in JavaScript is a collection of unique values. It prevents duplicate entries.

### Creating a New Set
``` javascript
// Create an empty Set
const mySet = new Set();

// Create a Set with initial values
const mySetWithValues = new Set([1, 2, 3, 4]);
```
## Common Methods
- add(value): Adds a value to the Set.
- delete(value): Removes a value.
- has(value): Checks if a value exists.
- size: Returns the number of values.
- clear(): Removes all values.
## Example
``` javascript
const mySet = new Set();
mySet.add(1);
mySet.add(2);
mySet.add(2); // Duplicate, won't be added
console.log(mySet.has(1)); // true
console.log(mySet.size); // 2
mySet.delete(1);
console.log(mySet.size); // 1
```
# 2. Date
### The Date object is used to work with dates and times.

### Creating a New Date
``` javascript
// Current date and time
const now = new Date();

// Specific date and time
const specificDate = new Date(2025, 0, 1, 10, 30); // Jan 1, 2025, 10:30 AM

// Parse a date string
const parsedDate = new Date('2025-01-01T10:30:00');
```
## Common Methods
- getFullYear(): Returns the year.
- getMonth(): Returns the month (0-11).
- getDate(): Returns the day of the month (1-31).
- toDateString(): Returns a readable date string.
- toISOString(): Returns a string in ISO format.
## Example
``` javascript
const date = new Date(2025, 0, 1);
console.log(date.getFullYear()); // 2025
console.log(date.getMonth()); // 0 (January)
console.log(date.toDateString()); // "Wed Jan 01 2025"
```
# 3. Map
### A Map in JavaScript stores key-value pairs. Unlike objects, Map keys can be of any type.

## Creating a New Map
``` javascript
// Create an empty Map
const myMap = new Map();

// Create a Map with initial values
const myMapWithValues = new Map([
  ['key1', 'value1'],
  ['key2', 'value2'],
]);
```
## Common Methods
- set(key, value): Adds or updates a key-value pair.
- get(key): Retrieves the value for a key.
- has(key): Checks if a key exists.
- delete(key): Removes a key-value pair.
- size: Returns the number of key-value pairs.
- clear(): Removes all key-value pairs.
## Example
```javascript
const myMap = new Map();
myMap.set('name', 'Alice');
myMap.set('age', 25);
console.log(myMap.get('name')); // "Alice"
console.log(myMap.size); // 2
myMap.delete('age');
console.log(myMap.size); // 1
```