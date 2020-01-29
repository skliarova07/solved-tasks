
```javascript
// Reversed Words
function reverseWords(str){
  return str.split(" ").reverse().join(" ");
}

//Name Shuffler
function nameShuffler(str){
  return str.split(' ').reverse().join(' ');
}

//Squash the bugs
function findLongest(str) {
  let spl = str.split(" "),
      longest = 0;
  
  for (var i in spl) {
    if (spl[i].length > longest) {
      longest = spl[i].length;
    }
  }

  return longest;
}

//Reversing Words in a String
function reverse(string){
  return string.split(' ').reverse().join(' ');
}

//Convert a string to an array
function stringToArray(string){
	return string.split(' ')
}

//Descending Order
function descendingOrder(n){
    return parseInt((n+'').split('').sort().reverse().join(''))
}

//Highest and Lowest
function highAndLow(numbers){
  num=numbers.split(' ');
  let max = parseInt(num[0]);
  let min = parseInt(num[0]);
  for (let i = 0; i < num.length; i++) {
    if(parseInt(num[i]) > max){
      max = parseInt(num[i]);
    }
  }
  for (let i = 0; i < num.length; i++) {
    if(parseInt(num[i]) < min){
      min = parseInt(num[i]);
    } 
 }
 return (max + ' ' + min);
}

//Can Santa save Christmas?
function determineTime(durations){
   let sec = 0;
   let str = [];
   for (let i = 0; i < durations.length; i++) {
     str = durations[i].split(":");
     sec += +str[0] * 3600 + +str [1] * 60 + +str[2];
    }
    return sec/3600 <=24 ? true : false;
}
```