
```javascript
// Be Concise IV - Index of an element in an array
const find = (array, element) =>
  array.includes(element) ? array.indexOf(element) : 'Not found'

//A wolf in sheep's clothing
function warnTheSheep(queue) {
    let sheepIndex = queue.length - queue.indexOf('wolf') - 1;
    if (sheepIndex === 0)
        return 'Pls go away and stop eating my sheep';
    return `Oi! Sheep number ${sheepIndex}! You are about to be eaten by a wolf!`;
}

//Array.diff
function array_diff(a, b) {
    let newArr = [];
    for(let i = 0; i < a.length; i++){
        if(b.indexOf(a[i])<0){
            newArr.push(a[i]);
        }
    }
    return newArr;
}

//JavaScript Array Filter
function getEvenNumbers(numbersArray){
  // filter out the odd numbers
  return numbersArray.filter(function(el){return el % 2 == 0});
}

//Find numbers which are divisible by given number
function divisibleBy(numbers, divisor) {
  return numbers.filter(el => el % divisor === 0);
}

//Removing Elements
function removeEveryOther(arr){
 return arr.filter ((el, i) => i % 2 === 0);
}

//Well of Ideas - Easy Version
function well(x) {
  switch (x.filter(i => i === 'good').length) {
    case 0:
      return 'Fail!'
    case 1:
    case 2:
      return 'Publish!'
    default:
      return 'I smell a series!'
  }
}

//Find how many times did a team from a given country win the Champions League?
function countWins(winnerList, country) {
  return  winnerList.filter(v=>v.country==country).length
}

//filterEvenLengthWords
function filterEvenLengthWords(words) {
  return words.filter(v => v.length % 2 === 0)
}

```