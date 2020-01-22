
```javascript
// Jenny's secret message
function greet(name){
  if(name === 'Johnny'){
    return 'Hello, my love!'
  } return `Hello, ${name}!`;
}

//Template Strings
var TempleStrings = function(obj, feature) {
  return `${obj} are ${feature}`;
}

//Returning Strings
function greet(name){
  return `Hello, ${name} how are you doing today?`;
}

//Grasshopper - Combine strings
function combineNames(firstName,lastName){
  return firstName + ' ' + lastName;
}

//Grasshopper - Debug sayHello
function sayHello(name) {
  return `Hello, ${name}`;
}

//If you can't sleep, just count sheep!!
var countSheep = function (num){
  let str = '';
  for(let i = 1; i <= num; i++) {
  str+= `${i} sheep...`;
  }
  return str;
}

//get character from ASCII Value
function getChar(c){
  return String.fromCodePoint(c);
}

//Regex validate PIN code
function validatePIN(pin) { 
    let value = false; 
    if (/^[0-9]{4}$/.test(pin) === true || /^[0-9]{6}$/.test(pin) === true) { 
        value = true; 
    }
    return value; 
}
 
//Is this my tail?
function correctTail(body, tail){
  return (body[body.length - 1] === tail)? true: false;
  }

//Abbreviate a Two Word Name
function abbrevName(name){
  var nam = name.split(' ');
  return nam[0].charAt(0).toUpperCase()+'.' + nam[1].charAt(0).toUpperCase();
}

//Numbers to Letters
function switcher(x){
  const obj={1:'z',2:'y',3:'x',4:'w',5:'v',6:'u',7:'t',8:'s',9:'r',10:'q',
11:'p',12:'o',13:'n',14:'m',15:'l',16:'k',17:'j',18:'i',19:'h',20:'g',
21:'f',22:'e',23:'d',24:'c',25:'b',26:'a',27:'!',28:'?',29:' '}
  return x.map(v=>obj[v*1]).join('')
}

//5 without numbers !!
function unusualFive() {
  let str = 'Hello';
return(str.length);
}

//Unique In Order
function uniqueInOrder(it){
  let result = [];
  let last = '';
  
  for(let i = 0; i < it.length; i++){
    if(it[i] !== last){
      last = it[i]
      result.push(last);
    }
  }
  return result;
}
```