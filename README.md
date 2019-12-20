
```javascript
// Difference Of Squares
function differenceOfSquares(n){
let sum = 0;
let sumSq = 0;
for (let i = 1; i <= n; i++){
  sum += i
  sumSq += i*i
}
sum = sum* sum
return sum - sumSq
}

// The wheat/rice and chessboard problem
function squaresNeeded(grains){
  let sum = 0;
  let x = 1;
  let square = 0 ;
  while (sum < grains){
    sum = sum + x
    square++;
    x = x * 2
  }
  return square;
}

// Powers of 3
function largestPower(n){
let k = 0;
while(3 ** k < n){
  k++ 
}
  return k - 1
}

// Tortoise racing
function race(v1, v2, g) {
    if (v1 >= v2) return null;
    let t = g / (v2- v1); // hours
    let time = t * 3600
    let hour = Math.trunc(time / 3600)
    let min = Math.trunc((time - hour * 3600)/ 60)
    let sec = Math.trunc(time - hour *3600 - min * 60);
    return[hour, min,sec]
    
}

// Factorial
function factorial(n){
let arr=[];
  for (let i = 1; i <= n; i ++)
  arr.push(i)
  return arr.reduce((a, b) => a * b, 1)
}

// Grasshopper - Summation
var summation = function (num) {
let sum = 0;
  for (let i = 1; i <= num; i++)
  sum += i;
  return sum  
}

// Sum of Multiples
function sumMul(n,m){
 if (n >= m) return 'INVALID'
let sum = 0;
for (let i = n; i < m; i = i + n)
  sum += i
  return sum
}

// Sum of the first nth term of Series
function SeriesSum(n) {
  let result = 0;
  let divider = 1;
  for (let i = 0; i < n; i ++) {
    if (i === 0) {
      result = 1;
    } else {
      divider += 3;
      result = result + (1 / divider);
    }
  }
  return result.toFixed(2);
};

// Draw stairs
function drawStairs(n) {
  let s = '';
  for (let i = 1; i <= n; i ++){
    s += i === n ? 'I':'I\n'+' '.repeat(i)
  }
  return s;
}

// Beginner Series #3 Sum of Numbers
function getSum( a,b ){
  let total = 0;  
  if (a === b) {
    return a;
  }
  
  if (a < b) {
    for (let i = a; i <= b; i++) {
      total += i;
    }
    return total;
  }
  
  if (b < a) {
    for (let i = b; i <= a; i++) {
      total += i;
    }
    return total;
  }
}

// Power
function numberToPower(number, power){
let result = 1;
let count = 0;
 while (count !== power) {
   count++;
    result = result * number; 
 }
return result;
}
```