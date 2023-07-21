#  Event loop

```
setTimeout(() => console.log(1), 0);

console.log(2);

new Promise(res => {
  console.log(3)
  res();
}).then(() => console.log(4));

console.log(5);


// output :  2,3,5,4,1
```

# Context

```

'use strict';

function foo() {
  console.log(this);
}

function callFoo(fn) {
  fn();
}

let obj = { foo };

callFoo(obj.foo);

output: undefined
```
# Arrow functions.
- Arrow functions do not have their own arguments object
- Arrow functions cannot be used as constructors 

```
function Operations(coef) {
  return {
    sum: (...args) => arguments[0] + coef
  }
}

const ops = Operations(0.1);

console.log(ops.sum(1, 2, 3));

const Num = () => {
  this.getNum = () => 10;
}

Num.prototype.getNum = () => 20;

const num = new Num();

console.log(num.getNum());
```

# Variable scope

```
'use strict';

console.log(foo());

let bar = 'bar';

function foo() {
  return bar;
}

bar = 'baz';
// ReferenceError: Cannot access ‘bar’ before initialization because temporary dead zone.
```
# ES6 modules

```
console.log('index.js');

import { sum } from './helper.js';

console.log(sum(1, 2));

console.log('helper.js');
export const sum = (x, y) => x + y;

// output:: helper.js index.js 3
// Hoisting is a mechanism in JS where variables and function declarations are moved to the top of their scope before the code is executed.

```
# Hoisting

```
var num = 8;

function num() {
  return 10;
}

console.log(num);

// output : 8
// Function and variable declarations are placed at the top of their scope, and the initialization of variables occurs at the time of script execution.

// Repeated declarations of a variable with the same name are skipped.

// Functions are always hoisted first. In whatever order the declarations of a function and a variable with the same name occur in your code, the function takes precedence, because it rises higher.

```

# Promises

```
Promise.resolve(1)
  .then(x => { throw x })
  .then(x => console.log(`then ${x}`))
  .catch(err => console.log(`error ${err}`))
  .then(() => Promise.resolve(2))
  .catch(err => console.log(`error ${err}`))
  .then(x => console.log(`then ${x}`));
// output :: error 1
// then 2

```
