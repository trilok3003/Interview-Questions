```
// Find

const numbers = [1, 3, 5, 7, 9];
const found = numbers.find(element => element > 3);
console.log(found); // Output: 5

// findIndex()

const foundIndex = numbers.findIndex(element => element > 3);
console.log(foundIndex); // Output: 2

// map

const doubled = numbers.map(element => element * 2);
console.log(doubled); // Output: [2, 4, 6, 8, 10]

// filter

const evenNumbers = numbers.filter(element => element % 2 === 0);
console.log(evenNumbers); // Output: [2, 4]

// fill


numbers.fill(0, 1, 4);
console.log(numbers); // Output: [1, 0, 0, 0, 5]


// some

const hasEven = numbers.some(element => element % 2 === 0);
console.log(hasEven); // Output: true

// every

const areAllEven = numbers.every(element => element % 2 === 0);
console.log(areAllEven); // Output: true

```
