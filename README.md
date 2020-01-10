
```javascript
// Expressions Matter
function expressionMatter(a, b, c) {
  return Math.max(a + b + c, a * b * c, (a + b) * c, a * (b + c))
}

// Lario and Muigi Pipe Problem
function pipeFix(numbers){
let first = numbers [0];
let last = numbers[numbers.length - 1];
let arr = []
  for (let i = first; i <= last; i++){
    arr.push(i);
    };
  return arr;
}

// Binary Addition
function addBinary(a,b) {
  return (a + b).toString(2)
}

// Convert to Binary
function toBinary(n){
  return +n.toString(2);
}

// Calculate Price Excluding VAT
//return price without vat
function excludingVatPrice(price){
  return price === null ? -1 : Number((price / 1.15).toFixed(2))
}

// Bin to Decimal
function binToDec(bin){
 return parseInt(bin,2)
}

// Hex to Decimal
function hexToDec(hexString){
  return parseInt(hexString, 16)
}

// Parse nice int from char problem
function getAge(inputString){
return parseInt(inputString, 10); 
}

// Parse float
function parseF(s) {
  return (Number.isNaN(parseFloat(s)) ? null : parseFloat(s));
}
```