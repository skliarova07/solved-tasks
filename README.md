
```javascript
// Square(n) Sum
function squareSum(numbers){
 let sum = 0;
 for(let i= 0; i < numbers.length; i++){
   sum = sum + numbers[i] ** 2
 }
 return sum
}

//How good are you really?
function betterThanAverage(classPoints, yourPoints) {
  let classAvg = 0;
  for (let i = 0; i < classPoints.length; i++){
    classAvg += classPoints[i]; 
  }
  classAvg = classAvg/classPoints.length; 
  return yourPoints > classAvg;
}

//Sum of positive
function positiveSum(arr) {
  let sum = 0;
  for(let i = 0; i < arr.length; i++){
    if(arr[i]> 0){
    sum += arr[i]
    }
 }
  return sum
}

//Count of positives / sum of negatives
function countPositivesSumNegatives(input) {
    if (input === null || input.length === 0)
      return [];
    let count = 0;
    let sum = 0;
    for (let i = 0; i < input.length; i++){
      if (input[i] > 0){
       count ++;
      }else{
        sum += input[i];
        }
    }
    return [count, sum];
}

//Calculate average
function find_average(array) {
  let sum = 0;
  for (i = 0; i < array.length; i++){
    sum += array[i];
  }
  return sum/array.length;
}

//Divide and Conquer
function divCon(x){
  let str = 0; 
  let num = 0;
  for (i = 0; i < x.length; i++) {
    if (typeof x[i] === 'string') {
      str += +x[i];
    } else {
      num += x[i];
    }
  }
  return num - str;
}

//Sum of Odd Cubed Numbers
function cubeOdd (arr) {
  let sum = 0;
  for (let num of arr)
    if (num !== +num)
      return;
    else if (num % 2)
      sum += num * num * num;
  return sum;
}

//Odd or Even?
function oddOrEven(array) {
   let sum = 0;
   for(i = 0; i< array.length; i++){
     sum += array[i]
     }
     if(sum % 2 === 0){
     return 'even'
     }
     return'odd'
}

//Find the smallest integer in the array
class SmallestIntegerFinder {
  findSmallestInt(args) {
   return Math.min(... args); 
  }
}

//Sum without highest and lowest number
function sumArray(array) {
  if(array == null || !array.length ) return 0;
  array.sort((a, b) => a-b);
  let sum = 0;
  for(let i = 1; i < array.length-1; i++){
  sum += array[i];
  }
  return sum;
}

//Find Maximum and Minimum Values of a List
let min = function(list){  
    return Math.min(...list);
}
let max = function(list){   
    return Math.max(...list);
}

//Find the divisors!
function divisors(integer) {
  let arr = [];
  for (let i = 2; i < integer; i++) { 
    if (integer % i === 0){ 
     arr.push(i); 
    }
  }
  return (arr.length === 0) ? integer + ' is prime' : arr;
}

//Count by X
function countBy(x, n) {
  let arr = [];
  for(i = 1; i <= n; i++){
  arr.push(i * x);
  }
  return arr;
}

//Unfinished Loop - Bug Fixing #1
function createArray(number){
  let newArray = [];
  for(let i = 1; i <= number; i++){
    newArray.push(i);
  }
  return newArray;
}

//Generate range of integers
function generateRange(min, max, step){
let arr = [];
  for (i = min; i <= max; i += step){
  arr.push(i);
  }
  return arr;
}

//Pre-FizzBuzz Workout #1
function preFizz(n) {
let arr = [];
  for (i= 1; i <= n; i++){
  arr.push(i);
  }
  return arr;
}

//Training JS #10: loop statement --for
function pickIt(arr){
  let odd = [];
  let even = [];
  for(let i = 0; i < arr.length; i++){
  if(arr[i] % 2 === 0){
    even.push(arr[i])
     }else{
    odd.push(arr[i]);
    }
  }
  return [odd,even];
}

//Powers of 2
function powersOfTwo(n){
  let arr = [];
  for (let i = 0; i <= n; i++) {
    arr.push(Math.pow(2, i));
  }
  return arr;
}

//Reversed sequence
const reverseSeq = n => {
let arr = [];
  for(i = n; i > 0; i--){
    arr.push(i)
  }
  return arr;
};

//Training JS #4: Basic data types--Array
function getLength(arr){
  return arr.length;
}
function getFirst(arr){
  return arr[0];
}
function getLast(arr){
  return arr[arr.length-1];
}
function pushElement(arr){
  arr.push(1);
  return arr;
}
function popElement(arr){
  arr.pop()
  return arr;
}

//No Loops 2 - You only need one
function check(a,x){
return a.includes(x)
};

You only need one - Beginner
function check(a, x) {
  return a.includes(x)
}

```