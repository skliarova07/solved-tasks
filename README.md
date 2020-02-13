
```javascript
// Counting Duplicates
function duplicateCount(text){
  let result = 0,
      newObject = {};
  text.toLowerCase().split('').map(str => {
      if (!newObject.hasOwnProperty(str)) {
        newObject[str] = 0;
      } else {
        if (newObject[str] === 0) {
          result += 1;
        }
        newObject[str] += 1;
      }
  });
  return result;
}

//Take a Ten Minute Walk
function isValidWalk(walk) {
	if(walk.length == 10) {
		let arr = [0,0,0,0];
		for (let i = 0; i < walk.length; i++) {
			if (walk[i] == 'n') {
				arr[0]++;
			} else if (walk[i] == 's') {
				arr[1]++;
			} else if (walk[i] == 'w') {
				arr[2]++;
			} else if (walk[i] == 'e') {
				arr[3]++;
			}
		}
		if (arr[0] == arr[1] && arr[2] == arr[3]) {
			return true;
		} else {
			return false;
		}
	} else {
		return false;
	}
}

//Bit Counting
let countBits = function(n) {
  let counter = 0;
  while(n > 0){
    let binaryNumber = 1;
    while(binaryNumber*2 <= n){
      binaryNumber = binaryNumber * 2;
    }
    n -= binaryNumber;
    counter++;
  }
  return counter;
};

```