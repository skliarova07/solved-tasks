
```javascript
// Filling an array (part 1)
function arr(n){
  var newArr = [];
  for(var i = 0; i < n; i++){
    newArr.push(i);
  }
  return newArr;
}

// Count the Monkeys!
function monkeyCount(n) {
let newArr = [];
  for (let i = 1; i <= n; i++){
    newArr.push(i);
    }
    return newArr;
}

//Sum Arrays
// Sum Numbers
sum = function (numbers) {
  "use strict";
  let s = 0;
  for(let i = 0; i < numbers.length; i++) {
    s += numbers[i];
  }
  return s;
};

//altERnaTIng cAsE <=> ALTerNAtiNG CaSe
String.prototype.toAlternatingCase = function () {
  let newStr = '';
  for (let i = 0; i < this.length; i++){
    if (this[i].toUpperCase() === this[i]){newStr = newStr + this[i].toLowerCase();
    } else {newStr = newStr + this[i].toUpperCase();}
  } return newStr;
}

//sort array by last character
function sortMe(arr){
let a;
for(let i = 0; i < arr.length-1; i++){
  for(let j = i+1; j< arr.length; j++){
    if(arr[i].toString().slice(-1)>arr[j].toString().slice(-1)){
      a = arr[i]; arr[i] = arr[j]; arr[j]=a;
    }
  }
} return arr;
}

//Converting Measures
function convertRecipe(recipe){
  let arr = recipe.split(' ');
  let full;
  for (let i = 1; i < arr.length; i++){
    if (arr[i-1].includes('/')) {
      let n = arr[i-1].split('/')[0]; 
      let m = arr[i-1].split('/')[1];
      full = +n/+m;
    } else full = +arr[i-1];
    if (arr[i] === 'tbsp') {
      arr[i] = arr[i] + ` (${Math.ceil(full * 15)}g)`;
      } else if (arr[i] === 'tsp') {
      arr[i] = arr[i] + ` (${Math.ceil(full * 5)}g)`; 
      }
  }
  return arr.join(' ');
}

//Convert string to camel case
function toCamelCase(str){
  let arr = str.split(/[^a-zA-Z]/g)
  for(let i = 1; i < arr.length; i++){
    arr[i]= arr[i][0].toUpperCase() + arr[i].slice(1);
  }
  return arr.join('')
}

//What is type of variable?
function type(value) {
  if(toString.call(value) == '[object Array]') return 'array';
  if(toString.call(value) == '[object Date]') return 'date';
  if(toString.call(value) == '[object Null]') return 'null';

  else return typeof(value);
}

//A Needle in the Haystack
function findNeedle(array) {
for (let i=0; i<array.length; i++){
  if (array[i] === 'needle')
    return 'found the needle at position ' + i;
  }
}

//Counting sheep...
function countSheeps (arrayOfSheep) {
    let sheepCounter = 0;
    for( let i = 0; i < arrayOfSheep.length; i++) {
      if(arrayOfSheep[i]=== true) {
        sheepCounter++;
      }
    }
    return sheepCounter;
  }

//Enumerable Magic #3 - Does My List Include This?
function include(arr, item){
  for (let i = 0; i <= arr.length; i++) {
    if (arr[i] === item) {
      return true;
    }
  }
  return false;
}

//Total amount of points
function points(games) {
  let count = 0;
  games.forEach(item =>{
    if(item[0] > item[2]) count += 3;
    if(item[0] === item[2]) count += 1;
  })
  return count;
}

//Find the first non-consecutive number
function firstNonConsecutive(arr) {
  for (let i = 0; i < arr.length - 1; ++i) {
    if (arr[i] + 1 !== arr[i + 1]) {
      return arr[i + 1]
    }
  }
  return null
}

//Difference of Volumes of Cuboids
function findDifference(a, b) {
  return Math.abs(a[0]*a[1]*a[2]-b[0]*b[1]*b[2]);
}
```