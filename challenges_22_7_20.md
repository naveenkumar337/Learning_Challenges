1.[RegEx XIV: Group Ranges x|y](https://edabit.com/challenge/7KbZc8QvzqrJPaE6Q)
```javascript
const REGEXP =/(blue|red)\s\w+/g
```
Examples
```
>"red flag blue flag".match(REGEXP) ➞ ["red flag", "blue flag"]
>"yellow flag red flag blue flag green flag".match(REGEXP) ➞ ["red flag", "blue flag"]
>"pink flag red flag black flag blue flag green flag red flag ".match(REGEXP) ➞ ["red flag", "blue flag", "red flag"]
```

2.[RegEx: Boundary Assertions I](https://edabit.com/challenge/AWENJSwyhcceiKvQX)
```javascript
function isJS(path) {
	var regex=/(jsx$|js$)/g
	return regex.test(path);
}
```
Examples
```
>isJS("/users/user.jsx") ➞ true
>isJS("/users/user.js") ➞ true
>isJS("/users/user.ts") ➞ false
```
