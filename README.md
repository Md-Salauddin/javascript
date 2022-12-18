# Numbers

JavaScript numbers are always stored as double precision floating point numbers 

```javascript
  // scientific (exponent) notation
  console.log(1000e-3) // 1000/1000 [output: 1]
  console.log(1000e3)  // 1000*1000 [output: 1000000]
```

**Integers:** accurate up to 15 digits </br>
**Decimals:** The maximum number of decimals is 17 but not accurate always

```javascript
  console.log(0.2 + 0.1)  // [output: 0.30000000000000004]
  console.log(0.3 + 0.1)  // [output: 0.4]
```

**[Common mistake]** Adding Numbers and Strings
* interpreter start from left->to right
* First 10 + 10 is added because x and y are both numbers.
* Then 20 + "total amount is: " is concatenated because "total amount is: " is a string.

```javascript
  let a = 10;
  let b = 10;
  console.log(a + b + " total amount is: ") // [output: 20 total amount is:]
  console.log("total amount is: " + a + b)  // [output: total amount is: 1010]
```

## Numeric value

try to convert strings to numbers in all numeric operations expect '+'

```javascript
let x = "100";
let y = 10;

console.log(x - y)  // [output: 90]
console.log(x * y)  // [output: 1000]
console.log(x / y)  // [output: 10]
```
