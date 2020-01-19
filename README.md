
```javascript
// Enumerable Magic #1 - True for All?
function all( arr, fun ) {
 return arr.every(fun);
}

//Grasshopper - Array Mean
var findAverage = function (nums) {
  return (nums.reduce ((acc, curr) => acc + curr))/ nums.length;
}

//SpeedCode #2 - Array Madness
const arrayMadness = (a, b) =>
  a.reduce((total, num) => total + num ** 2, 0) >
  b.reduce((total, num) => total + num ** 3, 0)

//Beginner - Reduce but Grow
function grow(x){
return x.reduce((acc, curr) => acc * curr, 1)
}

//Array plus array
function arrayPlusArray(arr1, arr2) {
  return arr1.concat(arr2).reduce((arr1,arr2)=>arr1+arr2)
}

//Beginner - Lost Without a Map
function maps(x){
return x.map(el => el * 2);
}

//Enumerable Magic #25 - Take the First N Elements
function take(arr, n) {
  return arr.splice(0, n);
}

//Remove First and Last Character Part Two
const array = arr =>
  arr
    .split(',')
    .slice(1, -1)
    .join(' ') || null
```