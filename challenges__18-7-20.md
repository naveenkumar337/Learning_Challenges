### 1.[Truthy or Falsy?](https://edabit.com/challenge/czEAQio8zr9HjZsQn)
```javascript
function isTruthy(input) {
	if(input===false || input===null || input===undefined || input===0 || input==="" || input.toString()==="NaN"){
	return 0;	
	}	
	else{
		return 1;
	}
}
```
### 2.[Sandwich Fillings](https://edabit.com/challenge/W8z2EghwmjQYhwM2D)
```javascript
function getFillings(sandwich) {
	return sandwich.slice(1,sandwich.length-1);
}
```
### 3.[Are the Numbers Equal?](https://edabit.com/challenge/Tbvjwh5GKRbxd3vyD)
```javascript
function isEqual(num1, num2) {
	return typeof num1=='string'?false: typeof num2=='string'?false:num1===num2?true:false;
}
```
### 4.[Is the String in Order?](https://edabit.com/challenge/9GcCezhbB3DxoJ6fL)
```javascript
function isInOrder(str) {
	return Array.from(str).sort().join('')===str;
}
```
### 5.[Difference of Max and Min Numbers in Array](https://edabit.com/challenge/v9DwaeR6NQoapEvHh)
```javascript
function diffMaxMin(arr) {
	var maxnum=arr[0];
	var minnum=arr[0];
	for(let i=0;i<arr.length;i++){
		if(maxnum>arr[i]){
			maxnum=arr[i];
		}
		if(minnum<arr[i]){
			minnum=arr[i];
		}
	}
	return minnum-maxnum;
}
```
### 6.[Find the Largest Number in an Array](https://edabit.com/challenge/HTbRYCmPwfZGnBcxW)
```javascript
function findLargestNum(arr) {
	return Math.max(...arr);
}
```
### 7.[Return 4 letter word](https://edabit.com/challenge/havnWL4BimvoaXNMn)
```javascript
function isFourLetters(arr) {
	return arr.filter(a=>a.length==4);
}
```
### 8.[Filter by Digit Length](https://edabit.com/challenge/RXNybvGHLuvFiWKvq)
```javascript
const filterDigitLength=(arr, num) =>arr.filter(x=>x.length==num);
```
### 9.[Maximum Difference](https://edabit.com/challenge/4vvFr9ZTK2AdyswXH)
```javascript
const difference=(nums)=>Math.Max(...nums)-Math.min(...nums);
```
