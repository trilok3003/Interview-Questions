<div align="center">
  <h1>Javascript</h1>
</div>

<ol>
  
<li>

**destructure-an-object-to-remove-a-property ?**

 ```const { password: _, ...user } = {
  id: 1,
  username: 'trilok',
  password: 'sddddddd',
};
 
console.log(user);
{ id: 1, username: 'trilok' }
```  

</li>

<li>
  
  **Map vs WeakMap**
  - `WeakMap is “A collection of key/value pairs whose key must be objects`
  - `Map is “A collection of key/value pairs whose key must be objects and primitives`
  - `both have methods like get(),set(),has(),delete()`
</li>

<li>
  
  **distinct or remove duplicacy in array**

  ```
let arr=[2,3,3,2,5,6,2];

arr.filter((ele, index, self) => self.indexOf(ele) === index)
```
 *second way*
```
[...new Set(arr)]
```
</li>

<li>

  **What will be output**
  ```
Promise.reject(1).then(function resolve() {console.log('hello')}).catch(console.log('err'));

Output: err

```
</li>

<li>

  **Count sepecific item of array**

  ```
let arr=[2,3,3,2,5,6,2];
let obj = {};
arr.forEach(ele => obj[ele] = obj[ele] ? obj[ele] + 1 : 1)
console.log(obj) // {2: 3, 3: 2, 5: 1, 6: 1}
```
</li>
 <li>Es6 features</li>
  <li>Arrow function vs regular function</li>
  <li>destructuring</li>
  <li>Default parameter, Rest parameter and Spread operator</li>
  <li>Arrow function advantages and disadvantages</li>
 <li>Promises merge</li>
  <li>Hoisting and its prevent</li>
  <li>
Closure example
</li>
<li>
  Higher order function example
</li>
<li>

 **Shallow Copying vs. Deep Copying**
 
 - `primitive data types  is copied by JavaScript`

```let x = 3
y = x // x is copied into y 
y++ // y is incremented 
console.log(y) // now 4 
console.log(x) // still 3
```

- ` non-primitive data types like arrays and objects, only a reference to the values is passed. So when the copy is mutated, the original also gets mutated. This is also known as shallow copying`

```
let adam = {name: "Adam"};
let jason = adam;
jason.name = "Jason";
console.log(adam.name);  // outputs "Jason" 
console.log(jason.name); // outputs "Jason"
```

- **4 Ways to Deep Copy Objects in JavaScript**

1. `shallow copy with =`
    ```
    const user = {
    name: "Kingsley",
    age: 28,
    job: "Web Developer"
     }
    const clone = user
    console.log(user)
    console.log(clone)
     /*   { 
           age: 28, 
           job: "Web Developer", 
           name: "Kingsley" 
          } 

          { 
           age: 28, 
           job: "Web Developer", 
           name: "Kingsley" 
          } 
     */

         clone.age = 30
         console.log(user)
         console.log(clone)
     /* 
      { 
      age: 30, 
      job: "Web Developer", 
        name: "Kingsley" 
       } 
        { 
       age: 30, 
        job: "Web Developer", 
        name: "Kingsley" 
       } 
       */
    
    ```  
2. **JSON.stringify() and JSON.parse()  (doesn't copy functions)**

```
const user = {
    name: "Kingsley",
    age: 28,
    job: "Web Developer"
}
let clone = JSON.parse(JSON.stringify(user))
console.log(user)
console.log(clone)
/* 
{ 
age: 28, 
job: "Web Developer", 
name: "Kingsley" 
} 
{ 
age: 28, 
job: "Web Developer", 
name: "Kingsley" 
} 
*/

clone.age = 32
console.log(user)
console.log(clone)
/* 
{ 
age: 28, 
job: "Web Developer", 
name: "Kingsley" 
} 
{ 
age: 32, 
job: "Web Developer", 
name: "Kingsley" 
} 
*/

// JSON.stringify() does not copy functions.

const user = {
    name: "Kingsley",
    age: 28,
    job: "Web Developer",
    incrementAge: function() {
  	  this.age++
    }
}
```
 3. **Object.assign()  (doesn't deep copy nested objects)**

```
const user = {
    name: "Kingsley",
    age: 28,
    job: "Web Developer",
    incrementAge: function() {
  	  this.age++
    }
}
let clone = Object.assign({}, user) // Copies user into clone
clone.age = 32
console.log(user)
console.log(clone)
/* 
{ 
age: 28, 
incrementAge: function() { 
this.age++ 
}, 
job: "Web Developer", 
name: "Kingsley" 
} 
{ 
age: 32, 
incrementAge: function() { 
this.age++ 
}, 
job: "Web Developer", 
name: "Kingsley" 
} 
*/

const user = {
    name: "Kingsley",
    age: 28,
    job: "Web Developer",
    location: {
      city: "Lagos",
    }
}
const clone = Object.assign({}, user)

clone.age = 32
clone.location.city = "New York"
console.log(user)
console.log(clone)
/* 
{ 
age: 28, 
job: "Web Developer", 
location: { 
city: "New York" 
}, 
name: "Kingsley" 
} 

{ 
age: 32, 
job: "Web Developer", 
location: { 
city: "New York" 
}, 
name: "Kingsley" 
} 
*/

```

4. **... spread operator  (doesn't deep copy nested objects)**

```
const user = {
    name: "Kingsley",
    age: 28,
    job: "Web Developer"
}
const clone = {...user}
console.log(clone);
/* 
{ 
age: 28, 
job: "Web Developer", 
name: "Kingsley" 
} 
*/

let user = {
    name: "Kingsley",
    age: 28,
    job: "Web Developer",
    location: {
        city: "Lagos",
    }
}
let clone = {...user}

clone = {
    ...clone,
  age: 32,
  location: {
  	...clone.location,
    city: "New York"
  }
}

console.log(user)
console.log(clone)
  /* 
{ 
age: 28, 
job: "Web Developer", 
location: { 
city: "Lagos" 
}, 
name: "Kingsley" 
} 

{ 
age: 32, 
job: "Web Developer", 
location: { 
city: "New York" 
}, 
name: "Kingsley" 
} 
*/

```

</li>

---
</ol>
