
```javascript
// To square(root) or not to square(root)
function squareOrSquareRoot(array) {
  return array.map (el => {
    if (Number.isInteger(Math.sqrt(el))){
      return Math.sqrt(el);
      }else{
      return Math.pow(el, 2);
    }
  });  
}

// You're a square!
var isSquare = function(n){
  let r = Math.sqrt(n);
  return r === Math.floor(r); 
}

// Find the next perfect square!
function findNextSquare(sq) {
return Math.sqrt(sq) % 1? -1: Math.pow(Math.sqrt(sq) + 1, 2);
}

//Beginner Series #4 Cockroach
function cockroachSpeed(s) {
 return Math.floor(s * (100000 / 3600))
}

// Price of Mangoes
function mango(quantity, price){
return (quantity - Math.floor(quantity / 3)) * price
}

// Holiday VIII - Duty Free
function dutyFree(normPrice, discount, hol){
return   Math.floor(hol / (normPrice * discount / 100))
}

// All Star Code Challenge #22
function toTime(seconds) {
 let hour = Math.floor (seconds/ 3600);
 let min = Math.floor((seconds - hour * 3600)/ 60);
return `${hour} hour(s) and ${min} minute(s)`;
}

// Formatting decimal places #1
function twoDecimalPlaces(number) {
  return Math.trunc(number * 100) / 100
}
```