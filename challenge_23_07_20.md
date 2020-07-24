### 1.[Find the Largest Numbers in a Group of Arrays](https://edabit.com/challenge/h7LTMAFeNz79rXB2Y)
```javascript
function findLargestNums(arr) {
	return arr.map(x=>Math.max(...x));
}
```
Examples
```
findLargestNums([[4, 2, 7, 1], [20, 70, 40, 90], [1, 2, 0]]) ➞ [7, 90, 2]
findLargestNums([[-34, -54, -74], [-32, -2, -65], [-54, 7, -43]]) ➞ [-34, -2, 7]
findLargestNums([[0.4321, 0.7634, 0.652], [1.324, 9.32, 2.5423, 6.4314], [9, 3, 6, 3]]) ➞ [0.7634, 9.32, 9]
```
### 2.[Sort Numbers in Ascending Order](https://edabit.com/challenge/SS23vniCZ6ssGwsQP)
```javascript
function sortNumsAscending(arr) {
	return arr==null || arr==[] ? [] :arr.sort((a,b)=>a-b);
}
```
Examples
```
sortNumsAscending([1, 2, 10, 50, 5]) ➞ [1, 2, 5, 10, 50]
sortNumsAscending([80, 29, 4, -95, -24, 85]) ➞ [-95, -24, 4, 29, 80, 85]
sortNumsAscending(null) ➞ []
sortNumsAscending([]) ➞ []
```
### 3.[Secret Society](https://edabit.com/challenge/zQm9YZTTFPhNtYjDr)
```javascript
function societyName(friends) {
	return friends.sort().map(x=>x.charAt(0)).join('');
}
```
Examples
```
societyName(["Adam", "Sarah", "Malcolm"]) ➞ "AMS"
societyName(["Harry", "Newt", "Luna", "Cho"]) ➞ "CHLN"
societyName(["Phoebe", "Chandler", "Rachel", "Ross", "Monica", "Joey"]) ➞ "CJMPRR"
```
### 4.[Amplify the Multiples of Four](https://edabit.com/challenge/FPHnbisnLwrQFYyAg)
```javascript
function amplify(num) {
	var arr=[];
	for(var i=1;i<=num;i++){
		if(i%4!==0) arr.push(i);
		else arr.push((i*10));
	}
	return arr;
}
```
Examples
```
amplify(4) ➞ [1, 2, 3, 40]
// Create a sequence from 1 to 4
// 4 is exactly divisible by 4, so it will be 4*10 = 40

amplify(3) ➞ [1, 2, 3]
// Create a sequence from 1 to 3
// There are no numbers that can be exactly divided by 4

amplify(25) ➞ [1, 2, 3, 40, 5, 6, 7, 80, 9, 10, 11, 120, 13, 14, 15, 160, 17, 18, 19, 200, 21, 22, 23, 240, 25]
// Create a sequence from 1 to 25
// The numbers exactly divisible by 4 are: 4 (4*10 = 40), 8 (8 * 10 = 80)... and so on.
```
Other Solutions
```javascript
//1
function amplify(num) {
	return Array(num).fill(1)
		.map((v,i) => v + i)
		.map(v => v % 4 == 0 ? v * 10 : v)
}
//2
const amplify = num => [...Array(num).keys()].map(x => (x + 1) % 4 == 0 ? (x + 1) * 10 : x + 1);

//3
const amplify = num =>
  Array.from({ length: num }, (_, i) => {
    const num = i + 1;
    return num % 4 === 0 ? num * 10 : num;
  });
```

### 5.[Transform into an Array with No Duplicates](https://edabit.com/challenge/Mo6Coy4PpTbZgtDKd)
```javascript
function set(arr) {
	return arr.filter((value,index)=>arr.indexOf(value)===index);
}
```

### 6.[Sort an Array by String Length](https://edabit.com/challenge/Gz27eKkMcLarzE5Rj)
```javascript
function sortByLength(arr) {
	return arr.sort((a,b)=>a.length-b.length);
}
```
Examples
```
sortByLength(["Google", "Apple", "Microsoft"])
➞ ["Apple", "Google", "Microsoft"]

sortByLength(["Leonardo", "Michelangelo", "Raphael", "Donatello"])
➞ ["Raphael", "Leonardo", "Donatello", "Michelangelo"]

sortByLength(["Turing", "Einstein", "Jung"])
➞ ["Jung", "Turing", "Einstein"]
```
