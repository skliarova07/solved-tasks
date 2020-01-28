
```javascript
// Credit Card Mask
// return masked string
function maskify(cc) {
  return '#'.repeat(cc.slice(0, -4).length) + cc.slice(-4);
}

//Tail Swap
function tailSwap(arr) {
  const [aa, ab] = arr[0].split(":")
  const [ba, bb] = arr[1].split(":")
  return [`${aa}:${bb}`, `${ba}:${ab}`]
}

//Vowel remover
function shortcut(string){
return string.replace(/[aeiou]/g, '')
}

//DNA to RNA Conversion
function DNAtoRNA(dna) {
  return dna.replace(/t/gi, 'U')
  }

//Correct the mistakes of the character recognition software
function correct(string){
	return string.replace(/5/g, 'S').replace(/0/g, 'O').replace(/1/g, 'I')
}

//Get number from string
function getNumberFromString(s) {
  return +s.replace(/\D/g, '');
}

//Fake Binary
function fakeBin(x){
  let result = '';
  for(let i = 0; i < x.length; i++){
    x[i] < 5 ? result += 0 : result += 1;
  }
  return result;
}

//FIXME: Replace all dots
var replaceDots = function(str) {
  return str.replace(/[.]/g, '-');
}
```