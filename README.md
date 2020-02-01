
```javascript
// makeBackronym
//preload variable: dict

let makeBackronym = function(string){
string = string.toUpperCase();
let arr = [];
for (let i = 0 ; i < string.length; i++){
  arr.push(dict[string[i]])
  }
  return arr.join(' ');
};

//Make a function that does arithmetic!
function arithmetic(a, b, operator) {
  switch (operator) {
    case 'add':
      return a + b
    case 'subtract':
      return a - b
    case 'multiply':
      return a * b
    case 'divide':
      return a / b
    default:
      return 'Unknown operation'
  }
}

//Check three and two
function checkThreeAndTwo(array) {
  let el1 = 0, el2 = 0, el3 = 0;
  for (let i = 0; i < array.length; i++) {
    if (array[i] === 'a') {
      el1++;
    } else if (array[i] === 'b') {
      el2++;
    } else if (array[i] === 'c') {
      el3++;
    }
  }
  return (el1 == 2 || el2 == 2 || el3 == 2) && (el1 == 3 || el2 == 3 || el3 == 3);
}

//Job Matching #1
function match(candidate, job) {
  if (job.maxSalary == undefined || candidate.minSalary == undefined) {
    throw "Error"
  }
  return job.maxSalary >= candidate.minSalary * 0.9;
}

//Add property to every object in array
for (i=0; i<questions.length; i++) {
questions[i].usersAnswer = null;
};

```