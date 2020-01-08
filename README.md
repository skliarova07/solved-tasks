
```javascript
// isReallyNaN
const isReallyNaN = (val) => {
  return Number.isNaN(val);
};

//Filter the number
var FilterString = function(value) {
return parseInt(value.replace(/[a-z]/gi,''))
}

//Is integer safe to use?
function SafeInteger(n) {
return Number.isSafeInteger(n)
}

//Return Negative
function makeNegative(num) {
  return - Math.abs(num)
}

//Opposite number
function opposite(number) {
  return (- number);
}

//Invert values
function invert(array) {
let newArr = [];
for (let i = 0; i < array.length; i++){
  newArr.push(- array[i]);
}
   return newArr;
}

//Closest elevator
function elevator(left, right, call){
  return Math.abs (call - left) < Math.abs(call - right) ? 'left': 'right';
}

//BASIC: Making Six Toast.
function sixToast(num) {
   return num > 6 ? num - 6 : 6 - num;
}

//Square Every Digit
function squareDigits(num){
    const digits = num.toString().split('')
    const squaredDigits = digits.map(n => n * n)
    const squaredNumber = squaredDigits.join('')
    return +squaredNumber
}

//Squares sequence
function squares(x, n) {
 let arr = [];
  for(let i = 0; i < n; i++){
    arr.push(x);
    x*= x;
  }
  return arr;
}
```