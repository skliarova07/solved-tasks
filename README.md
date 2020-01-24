
```javascript
// repeatIt
var repeatIt = function(str, n) {
return (typeof str !== 'string') ? 'Not a string' : str.repeat(n);
  }

//String repeat
function repeatStr (n, s) {
  return s.repeat(n);
}

//Don't give me five!
function dontGiveMeFive(start, end){
let count = 0;
for (let i = start; i <= end; i++){
  if (i.toString().includes("5") === false) {
      count++;
    }
  }
  return count;
}

//Do you speak "English"?
function spEng(sentence){
return (sentence.toLowerCase().includes('english'))? true : false;
}

//Find the position!
function position(letter){
  const alphabet = 'abcdefghijklmnopqrstuvwxyz';
  return 'Position of alphabet: ' + (alphabet.indexOf(letter) + 1);
}

//validate code with simple regex
const validateCode = code => /^[1-3]/g.test(code)

//String ends with?
function solution(str, ending){
  return str.endsWith(ending);
}
```