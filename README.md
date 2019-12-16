
```javascript

// Типы данных. Определение типа данных
// Convert boolean values to strings 'Yes' or 'No'.

function boolToWord( bool ){
  if (bool == true){
        return "Yes"
    } else {
        return "No"}
}

// Super Duper Easy
function problem(x){
let a = x * 50 + 6;
  if(typeof (x) === 'number') {
  return a;
  } else { return 'Error'}
}
// Type of sum
function typeOfSum(a, b) {
  return typeof (a + b)
}

// Convert a Number to a String!
function numberToString(num) {
  return String(num)
}
// Number toString
let a = 123;
a = a.toString();
console.log(a)

//Convert a String to a Number!
let stringToNumber = function(str){
  if(typeof str === 'string'){
  return + str
  } else {
  return null;
  }
}

//Convert a Boolean to a String
function booleanToString(b){
  if (Boolean (b) === true) {
    return 'true'
  } else{
    return 'false'
  }
}

// Sum The Strings
function sumStr(a,b) {
  return String(Number(a) + Number(b))
}

// Formatting decimal places #0
function twoDecimalPlaces(n) {
  return +(n.toFixed(2))
}

// Area of a Square
function squareArea(A){
  return + (Math.pow((4 * A) / (2 * Math.PI), 2)).toFixed(2)
}

// Keep Hydrated!
function litres(time) {
const waterPerHour = 0.5;
return Math.floor(time * waterPerHour)
  return 0;
}

// Count Odd Numbers below n
function oddCount(n){
  return Math.floor(n/2)
}

// Century From Year
function century(year) {
  return Math.ceil(year / 100);
}

// Discover The Original Price
function discoverOriginalPrice(discountedPrice, salePercentage){
  return +((discountedPrice*100)/(100-salePercentage)).toFixed(2);
} 

// How many times should I go?
function howManyTimes(annualPrice, individualPrice) {
  return Math.ceil(annualPrice / individualPrice);
}

// Return the closest number multiple of 10
const closestMultiple10 = num => {
  return ((num / 10).toFixed(0)) * 10;
}


```