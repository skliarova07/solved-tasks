
```javascript
// Regex count lowercase letters
function lowercaseCount(str){
  let newStr = str.replace(/[^a-z]/g, '');
  return newStr.length;
}

//Double Char
function doubleChar(str) {
  let newStr = '';
  for (let i = 0; i < str.length; i++) {
    newStr += str.charAt(i) + str.charAt(i);
  }
  return newStr;
};

//Remove First and Last Character
const removeChar = str =>
  str
    .split('')
    .slice(1, str.length - 1)
    .join('')


//Triple Trouble
function tripleTrouble(one, two, three) {
  let result = '';
  one = one.split('');
  two = two.split('');
  three = three.split('');
  
  for (let i = 0; i < one.length; i++) {
    result += one[i] + two[i] + three[i];
  }
  return result;
}

//Remove String Spaces
function noSpace(x){
  return x.split(' ').join('');
}

//Spacify
function spacify(str) {
  return str.split('').join(' ')
}

//Reversed Strings
function solution(str) {
return str.split("").reverse().join("").split(" ").reverse().join(" ");
}

//Is it a palindrome?
const isPalindrome = (x) => {
  return x.split("").reverse().join("").toLowerCase() === x.toLowerCase() ? true : false
}

//The Wide-Mouthed frog!
const mouthSize = animal => (/alligator/gi.test(animal) ? 'small' : 'wide')

//Find the capitals
var capitals = function (word) {
  let a = word.split('')
	let arr = [];
  for(let i = 0; i < word.length; i++){
  if (a[i] === a[i].toUpperCase()){
    arr.push(i)
    }
  }
  return arr
};

//Mumbling
function accum(s) {
  return s.split('').map((c, i) => (c.toUpperCase() + c.toLowerCase().repeat(i))).join('-');
}

//Thinking & Testing : Something capitalized
function testit(s){
  let str = '';
  for (i = 0; i < s.length; i++) {
     if (s[i + 1] === ' ' || i === s.length - 1) {
        str += s[i].toUpperCase();
     } else {
        str += s[i]
     }
  }
  return str;
}

// MakeUpperCase
function makeUpperCase(str) {
  return str.toUpperCase();
}

//Capitalization and Mutability
function capitalizeWord(word) {
  return word[0].toUpperCase() + word.slice(1);
}
```