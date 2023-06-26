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
---
</ol>
