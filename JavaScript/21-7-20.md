1.[No Conditionals?](https://edabit.com/challenge/WjXHgXLAvMxNvD6h2)
 ```javascript
 function flip(y) {
	return Number(y==0);
}
 ```

2.[Filter out Strings from an Array](https://edabit.com/challenge/b2NdDSdkjqFnCTfS8)
```javascript
function filterArray(arr) {
	return arr.filter(q=>typeof q==='number');
}
```
3.[Repeating Letters](https://edabit.com/challenge/Mc6Xi4PRw7fDzeMDB)
```javascript
function doubleChar(str) {
	return Array.from(str).map(x=>x.repeat(2)).join('').toString();
}
```
4.[Recursion to Repeat a String n Number of Times](https://edabit.com/challenge/MjqneMZ7aZa8AxXZG)
```javascript
function repetition(txt, n) {
	if(n!==1){
	return txt + repetition(txt,n-1);
	}
	else{
		return txt;
	}
}
```
5.[Highest Digit](https://edabit.com/challenge/YJuhHKSmNCaKNHcD3)
```javascript
function highestDigit(number) {
	console.log(...number.toString());
	return Math.max(...number.toString());	
}
```

6.[Summing a Slice](https://edabit.com/challenge/B3FR3P7g8NyTg7t8b)
```javascript
function highestDigit(number) {
	console.log(...number.toString());
	return Math.max(...number.toString());	
}
```

7.[Algorithms I: Introduction to Recursion](https://edabit.com/challenge/vtDnynHfWCnMaKYym)
```javascript
function factorial(num) {
if(num!==0){
	return num * factorial(num-1);
}	
	return 1;
}
```
```
Examples

>factorial(5) ➞ 120
>factorial(3) ➞ 6
>factorial(2) ➞ 2
```

8.[Factorial of a Positive Integer](https://edabit.com/challenge/Ju7AK9rAGjz86hjxo)
```javascript
function factorial(z) {
	if(z==0 || z==1){
		return 1;
	}
	return z * factorial(z-1);
}
```
9.[Sum of Cubes](
https://edabit.com/challenge/XdAR3KohR5w7rjrFg)
```javascript
function sumOfCubes(nums) {
	return	nums.reduce((a,b)=>a+Math.pow(b,3),0);
}
```
