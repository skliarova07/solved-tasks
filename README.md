
```javascript
// Find Duplicates
function duplicates(arr) {
  return arr.filter(function(v, i) {return arr.indexOf(v) != i && arr.lastIndexOf(v) == i;});
}

// Train to remove duplicates from an array with filter()
function unique(arr) {
  return arr.filter((x, i) => arr.indexOf(x) === i);
}

//Santa's Naughty List
const findChildren = (santasList, children) => {
  const arr = [];
  for (const item of santasList) {
    for (const child of children) {
      if (item === child && !arr.includes(item)) {
        arr.push(item)
      }
    }
  }
  return arr.sort();
}

//Convert number to reversed array of digits
function digitize(n) {
  return (n+'').split('').reverse().map(n => +n);
}

//My head is at the wrong end!
function fixTheMeerkat(arr) {
	 return arr.reverse();
}

//Two Oldest Ages
function twoOldestAges(ages) { 
   ages.sort(function(a, b) {
  return a - b;
});
  let oldest = ages.pop()
   let secondOldest = ages.pop() 
   return [secondOldest,oldest]
}

//Sum of two lowest positive integers
function sumTwoSmallestNumbers(numbers) {  
  numbers.sort(function(a,b){
  return a - b;
  })
  numbers.reverse()
  let lowNum1 = numbers.pop()
  let lowNum2 = numbers.pop()
  return lowNum1 + lowNum2
}

//Sum of differences in array
function sumOfDifferences(arr) {
  arr.sort((a, b) => a - b);
  let sum = 0;
  for(let i = arr.length - 1; i > 0; i--) {
    sum += arr[i] - arr[i - 1];
  }
  return sum;
}

//Sentence Smash
function smash (words) {
   return words.join(' ') 
};

//String Templates - Bug Fixing #5
function buildString(...template){
  return `I like ${template.join(', ') + '!'}`;
}

//Printing Array elements with Comma delimiters
function printArray(array){
  return array.join(',')
}

//CSV representation of array
function toCsvText(array) {
   return array.join('\n')
}
```