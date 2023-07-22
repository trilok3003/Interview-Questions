1. Condition true
//Longhand
if(booleanVar === true){}
//Shorthand
if(booleanVar){}
2.Arrow Function :

//Longhand
function data(name){
console.log(name)
}
//Shorthand
const data = name =>console.log(name)
3.Template Literals :

const name = "Rajesh";
const day = "Sunday";
const data = "Hello " + name + "Have a wonderful " + day + "!";
const name = "Rajesh";
const day = "Sunday";
const data = `Hello ${name} Have a wonderful  ${day} !`;
4.Power of any number :

//Longhand
Math.pow(3,6)
//Shorthand
3**6
5.Assignment operator :

//Longhand
x = x+y;
x = x-y;  
//Shorthand
x += y;
x -= y;
6.Declaring Variables :

//Longhand
let x;
let y;
let z = 'a';
//Shorthand
let x,y,z = 'a';
7.Ternary Operator :

//Longhand
let isAdult;
if(age>17){
  isAdult = true;
}else {
isAdult = false;
}  
//Shorthand
let isAdult = age >17 ? true :false;   
