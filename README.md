
```javascript
// Sleigh Authentication
function Sleigh() {}

Sleigh.prototype.authenticate = function(name, password) {
  if (name === 'Santa Claus' && password === 'Ho Ho Ho!'){
  return true
  } else if (name !== 'Santa Claus' || password !== 'Ho Ho Ho!'){
  return false
  }
};

// Is n divisible by x and y?
function isDivisible(n, x, y) {
if (n % x === 0 && n % y === 0){
return true
} else if (n % x !== 0 || n % y !== 0){
return false
}
}

// Is this a triangle?
function isTriangle(a,b,c){
 if (a < b + c && b < a + c && c < a + b){
  return true
} else {
  return false;
  }
}

// Rock Paper Scissors!
const rps = (p1, p2) => {
if (p1 === p2){
return ('Draw!');
}else if (p1 === 'paper' && p2 === 'rock'){
return ('Player 1 won!');
}else if (p1 === 'rock' && p2 === 'scissors'){
return ('Player 1 won!');
}else if (p1 === 'scissors' && p2 === 'rock'){
return ('Player 2 won!');
}else if (p1 === 'rock' && p2 === 'paper'){
return ('Player 2 won!');
}else if (p1 === 'paper' && p2 === 'scissors'){
return ('Player 2 won!');
}else if (p1 === 'scissors' || p2 === 'paper'){
return ('Player 1 won!');
}
}

// L1: Set Alarm
function setAlarm(employed, vacation){
return employed === true && vacation === false
}

// Can we divide it?
function isDivideBy(number, a, b) {
  return number % a === 0 && number % b === 0
}

// Student's Final Grade
function finalGrade (exam, projects) {
  if (exam > 90 || projects > 10){
  return 100
    } else if (exam > 75 && projects >= 5){
    return 90
      } else if (exam > 50 && projects >= 2){
      return 75
        } else {
      return 0
    }
}

// Convert boolean values to strings 'Yes' or 'No'.
function boolToWord( bool ){
  return bool ? 'Yes' : 'No';
  }

// Be Concise I - The Ternary Operator
function describeAge(age) {
return `You\'re a(n) ${age<=12?'kid':age<=17?'teenager':age<=64?'adult':'elderly'}`
}

```