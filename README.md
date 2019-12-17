
```javascript
// Keep up the hoop
function hoopCount (n) {
   if (n >= 10){return 'Great, now move on to tricks'
   } return 'Keep at it until you get it'  
}

// Chuck Norris VII - True or False? (Beginner)
function ifChuckSaysSo(){
return !true;
}

// Simple Comparison?
function add(a, b){
	if (a == b) { 
  return true
  } else { 
  return false };
}
// Is he gonna survive?
function hero(bullets, dragons){
  if (bullets >= dragons * 2 ){
  return true
  } return false;
}

// Even or Odd
function even_or_odd(number) {
  if(number % 2){
  return 'Odd'
  }
  return 'Even'
}

// Determine offspring sex based on genes XX and XY chromosomes
function chromosomeCheck(sperm) {
  if(sperm === 'XY'){
  return 'Congratulations! You\'re going to have a son.'
  } 
  return 'Congratulations! You\'re going to have a daughter.'
}

// What's the real floor?
function getRealFloor(n) {
if (n > 0 && n < 13){
return n - 1;
  }else if
    (n > 13){
return n - 2
}
return n
}

// Calculate BMI
function bmi(weight, height) {
let a = weight / (height * height);
if (a <= 18.5) return 'Underweight'
else if (a <= 25.0) return 'Normal'
else if (a <= 30.0) return 'Overweight'
else if (a > 30) return 'Obese';
}

// Alan Partridge II - Apple Turnover
function apple(x){
if (x = +x && x * x >= 1000){ 
return 'It\'s hotter than the sun!!'
}else{ 
return 'Help yourself to a honeycomb Yorkie for the glovebox.'
}
}

// Simple multiplication
function simpleMultiplication(number) {
    if (number % 2){
    return number * 9
    } else {
    return number * 8
    }
}

// Calculate Two People's Individual Ages
function getAges(sum,difference){
 if (difference < 0||sum < 0) return null;
   sum = sum / 2
   difference /= 2
   if (sum + difference < 0||sum - difference < 0) return null;
   return [sum + difference, sum - difference]
};



```