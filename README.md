
```javascript
// What is my name score? #1
function nameScore(name) {
	let nameList = name.replace(/\s+/gi, '').toUpperCase().split('');
	let score = 0,
		result = {};
	for (let x in alpha) {
		for (let i = 0; i < nameList.length; i++) {
			if (x.indexOf(nameList[i]) !== -1) {
				score += alpha[x];
			}
		}
	}
	result[name] = score;
	return result;
}

//The Office I - Outed
function outed(meet, boss){
  let res = 0;
  for (let x in meet) {
    res += (x === boss ? 2 * meet[x] : meet[x]);
  }
  return res / Object.keys(meet).length <= 5 ? 'Get Out Now!' : 'Nice Work Champ!';
}

//Most valuable character
function solve(st) {
  let obj = {};
  for (let i = 0; i < st.length; i++) {
    obj[st[i]] = st.lastIndexOf(st[i]) - st.indexOf(st[i]);
  }
  let arr1 = Object.values(obj);
  let v = Math.max(...arr1);
  let arr2 = [];
  for (let key in obj){
    if (obj[key] === v) arr2.push(key);
  }
  let arr3 = arr2.sort();
  return arr3[0];
}

//Permute a Palindrome
function permuteAPalindrome (input) { 
    let x = {};
    for(let i = 0; i < input.length; i++){
        if(!x[input[i]])x[input[i]] = 1;
        else x[input[i]]++;
    }
    let count = 0;
    for(j in x){
        if(x[j]%2 !== 0 )count++;
        if(count > 1)return false
    }
    return true
}

//The Office II - Boredom Score
function boredom(staff){
  let arr = []
  let sum = 0
  let score = {
    'accounts': 1,
    'finance': 2,
    'canteen': 10,
    'regulation': 3,
    'trading': 6,
    'change': 6,
    'IS': 8,
    'retail': 5,
    'cleaning': 4,
    'pissing about': 25
  }

  for(key in staff){
    sum += score[staff[key]]
  }

  if(sum <= 80) return 'kill me now'
  else if(sum >= 100) return 'party time!!'
  else return 'i can handle this'
}

```