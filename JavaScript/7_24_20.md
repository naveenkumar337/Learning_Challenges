### 1.[Multiply by Length](https://edabit.com/challenge/LMhRTq3hccz2D9Lax)
```javascript
const multiplyByLength=(arr)=>arr.map(x=>x*arr.length);
```
Examples
```
multiplyByLength([2, 3, 1, 0]) ➞ [8, 12, 4, 0]
multiplyByLength([4, 1, 1]) ➞ ([12, 3, 3])
multiplyByLength([1, 0, 3, 3, 7, 2, 1]) ➞  [7, 0, 21, 21, 49, 14, 7]
multiplyByLength([0]) ➞ ([0])
```
### 2.[Convert Year to Century](https://edabit.com/challenge/H3fKTSK4dgwXRbfTP)
```javascript
function centuryFromYear(year) {
	console.log(year.toString().length);
	if(year.toString().length<=3){
		return year%100!==0?parseInt([...year.toString()].slice(0,1).join(''))+1
	:parseInt([...year.toString()].slice(0,1).join(''));
	}else{
	return year%100!==0?parseInt([...year.toString()].slice(0,2).join(''))+1
	:parseInt([...year.toString()].slice(0,2).join(''));
	}
}


//Other Solutions

const centuryFromYear = year => Math.ceil(year / 100);

```
Examples
```
centuryFromYear(2005) ➞ 21
centuryFromYear(1950) ➞ 20
centuryFromYear(1900) ➞ 19
```
### 3.[Matchstick Houses](https://edabit.com/challenge/tYHkTdFrEmWfxpPKF)
```javascript
function matchHouses(step) {
	return step===0?0:step==1?6:((step-1)*5)+6;
}

//Other Solutions

function matchHouses(step) {
	return step === 0 ? 0 : 5 * step + 1;
}

```
Examples
```
matchHouses(1) ➞ 6
matchHouses(4) ➞ 21
matchHouses(87) ➞ 436
```

### 4.[Friday the 13th](https://edabit.com/challenge/98CAqzDToJdx5LGFm)
```javascript
function hasFriday13(month, year) {
	var date=new Date(`${month} 13,${year}`);
	return parseInt(date.getDay())===5;
}
```
Examples
```
hasFriday13(3, 2020) ➞ true
hasFriday13(10, 2017) ➞ true
hasFriday13(1, 1985) ➞ false
```
### 5.[Maximum Edge of a Triangle](https://edabit.com/challenge/nhXofMMyrowMyr9Nv)
```javascript
function nextEdge(side1, side2) {
	return (side1+side2)-1;
}
```
Examples
```
nextEdge(8, 10) ➞ 17

nextEdge(5, 7) ➞ 11

nextEdge(9, 2) ➞ 10
```

### 6.[Valid Zip Code](https://edabit.com/challenge/Ysk5M8XAscc4fqaAi)
```javascript
function isValid(zip) {
	console.log(parseInt(zip));
	return (zip.length===5 & Number.isInteger(Number(zip))) ? true :false;
}

//Other Solutions

const isValid = zip => /^\d{5}$/.test(zip);

function isValid(zip) {
return zip.length == 5 && !isNaN(zip);
}
```
Examples
```
isValid("59001") ➞ true

isValid("853a7") ➞ false

isValid("732 32") ➞ false

isValid("393939") ➞ false
```

### 7.[Printer Levels](https://edabit.com/challenge/QXWM2oo7rQNiyDsip)
```javascript
function inkLevels(inks) {
	var [a,b,c]=Object.values(inks);
	return Math.min(a,b,c);
}

//Others Solutions
const inkLevels = inks => Math.min(...Object.values(inks));
```
Examples
```
inkLevels({
  "cyan": 23,
  "magenta": 12,
  "yellow": 10
}) ➞ 10

inkLevels({
  "cyan": 432,
  "magenta": 543,
  "yellow": 777
}) ➞ 432

inkLevels({
  "cyan": 700,
  "magenta": 700,
  "yellow": 0
}) ➞ 0
```

### 8.[Find the Bug: Returning Valid Units of Measure](https://edabit.com/challenge/oGYGaavTNoYDjykJY)
```Javascript
function hasValidUnitOfMeasure(product = {}) {
	const { unitOfMeasure, comment } = product
	return (!!comment || unitOfMeasure === 'L' || unitOfMeasure === 'PCE')
}
```
