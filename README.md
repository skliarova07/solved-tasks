
```javascript

// Чистая арифметика
// I love you, a little , a lot, passionately ... not at all
  const phrases = [
    'I love you',
    'a little',
    'a lot',
    'passionately',
    'madly',
    'not at all',
]
function howMuchILoveYou(nbPetals) {
     return phrases[(nbPetals - 1) % phrases.length] 
}
console.log(howMuchILoveYou(7));
//"I love you"
console.log(howMuchILoveYou(3));
//"a lot"
console.log(howMuchILoveYou(6));
//"not at all"
console.log(howMuchILoveYou(2));
//"a little"
console.log(howMuchILoveYou(5));
//"madly"

// Third Angle of a Triangle
function otherAngle(a, b) {
  return (180 - a - b);
}

// Breaking chocolate problem
function breakChocolate(n,m) {
  if(n > 0 && m > 0) {
  return m * n - 1
  } else {return 0}
}

// Sum of angles
function angle(n) {
  if (n > 2) return 180 * (n - 2)
}

// For Twins: 2. Math operations
function iceBrickVolume(radius, bottleLength, rimLength) {
 let sideOfSquare = (2 * radius) / (2 ** 0.5);
return Math.round((bottleLength - rimLength) * sideOfSquare ** 2) 
}
console.log(iceBrickVolume(1, 10, 2));
console.log(iceBrickVolume(5, 30, 7));

```