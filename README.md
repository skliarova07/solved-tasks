
```javascript
// Detect Pangram
function isPangram(string){
  let str = string.toLowerCase().replace(/[^a-z]/g, '');
  let obj = {};
  for (let el of str){
    obj[el] = obj[el] ? obj[el]++ : 1;
   }
  let count = 0;
  for (let i in obj){
    if (obj[i] === 1) count++;
    else return fals;
   }
  return count === 26;
  }

// Exclamation marks series #2: Remove all exclamation marks from the end of sentence
function remove(s){
  return s.replace(/!+$/, ''); 
}

// Complementary DNA
function DNAStrand(dna){
  let res = '';
  for(let x of dna){
    if(x === 'A') res += 'T';
    if(x === 'T') res += 'A';
    if(x === 'C') res += 'G';
    if(x === 'G') res += 'C';
  }
  return res;
}
```