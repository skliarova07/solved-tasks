
```javascript
// Find the odd int


function findOdd(arr) {
  let count = 0;
  for(let i=0; i<arr.length; i++){
    for(let j=0; j<arr.length; j++){
      if(arr[i] === arr[j]) count++;
    } if(count % 2 !== 0) return arr[i]
  } return count;
}

//Multiples of 3 or 5

 function solution(number) {
let sum = 0;
  for(let i = 1; i < number; i++){
    if((i % 3 === 0 )||(i % 5 === 0)||(i % 3 === 0 && i % 5 === 0)){
      sum += i;
    }
  }
  return sum;
}

//Persistent Bugger.

function persistence(num) {
   let i = 0;
   while (num.toString().length !== 1) {
     num = num.toString().split("").reduce((a,b)=>a*b);
     i++;
   }
   return i;
}

```