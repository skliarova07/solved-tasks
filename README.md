
```javascript
//101 Dalmatians - squash the bugs, not the dogs!
function howManyDalmatians(number){ 
return `${number <= 10 ? 'Hardly any': number <= 50 ? 'More than a handful!': 
number === 101 ? '101 DALMATIANS!!!': 'Woah that\'s a lot of dogs!'}`
}

// Do I get a bonus?
function bonusTime(salary, bonus) {
return bonus === true? `£${salary * 10}` :`£${salary}` 
}

// Training JS #7: if..else and ternary operator
function saleHotdogs(n){
  return n < 5 ? n * 100 : n >= 5 && n < 10 ? n * 95:  n * 90 
}

// Basic Mathematical Operations
function basicOp(operation, value1, value2){
switch (operation){
case '+' : return (value1 + value2);
case '-' : return (value1 - value2);
case '*' : return (value1 * value2);
case '/' : return (value1 / value2);
}
}

// Switch it Up!
function switchItUp(number){
switch (number){
  case 0: return 'Zero';
  case 1: return 'One';
  case 2: return 'Two';
  case 3: return 'Three';
  case 4: return 'Four';
  case 5: return 'Five';
  case 6: return 'Six';
  case 7: return 'Seven';
  case 8: return 'Eight';
  case 9: return 'Nine';
}
}

// simple calculator
function calculator(a,b,sign){
if (typeof a !== 'number' || typeof b !== 'number') return 'unknown value'
  switch (sign){
  case '+': return (a + b); 
  case '-': return (a - b);
  case '*': return (a * b);
  case '/': return (a / b);
  default:
      return 'unknown value'
  }
}

// No zeros for heros
function noBoringZeros(n) {
  while(n % 10 == 0 && n != 0){n /= 10;}
  return n;
}

// Power of two
function isPowerOfTwo(n){
 if (n === 1) return true;
 while (n > 1){
 n = n / 2
 }
 if (n === 1)
 return true;
 else
 return false
}
```