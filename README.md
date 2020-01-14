
```javascript
// Numbers to Objects
function numObj(s){
let obj = {};
let arr = [];
for (let i = 0; i < s.length; i++){
  obj[s[i]] = String.fromCharCode(s[i]);
  console.log(s[i]);
  console.log(obj[s[i]]);
  s[i] += ''
  let res = {}
  res[s[i]] = obj[s[i]]
  arr.push(res)
  }
return arr  
}

//How many days are we represented in a foreign country?
function daysRepresented(trips){
let res = {};
 for(i = 0; i < trips.length; i++){
   for(j = trips[i][0]; j <= trips[i][1]; j++) {
     if(!res[j]){
       res[j] = 1
     }
    }
  }
  return Object.keys(res).length
}

//Coding Meetup #5 - Higher-Order Functions Series - Prepare the count of languages
function countLanguages(list) {
  let res = {};
  for (i = 0; i < list.length; i++){
    if(!res[list[i].language]){
      res[list[i].language] = 1;
    }else{
      res[list[i].language] ++;
    }
  }
  return res;
}

//Remove the minimum
function removeSmallest(numbers) {
  if (!numbers.length)
    return [];
  let inx = 0;  
  const nums = Array.from(numbers, (x, i) => {  
    if (x < numbers[inx])
      inx = i;
    return x;
  });
  nums.splice(inx, 1);
  return nums;
}

//Every possible sum of two digits
function digits(num){
  let numStr = num.toString();
  let result = [];
  for(let i = 0; i < numStr.length - 1; i++) {
    for (let j = i + 1; j < numStr.length; j++) {
      result.push( parseInt(numStr[i]) + parseInt(numStr[j]) );
    }
  }
  return result;
}

//Is every value in the array an array?
const arrCheck = value =>
value.every(Array.isArray)
```