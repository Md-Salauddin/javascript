# Number Methods

**toString()** returns a number as a string

```javascript
  let x = 123;
  console.log(typeof x); // [output: number]
  let newX = x.toString();
  console.log(typeof newX); // [output: string]
```

**toExponential()** 
* returns a string, with a number rounded and written using exponential notation </br>
* parameter defines the number of characters behind the decimal point

```javascript
  let x = 9000;
  let y = 9.2;
  
  console.log(x.toExponential()); // [output: 9e+3]
  console.log(x.toExponential(1)); // [output: 9.0e+3]
  console.log(y.toExponential()); // [output: 9.2e+0]
  console.log(y.toExponential(2)); // [output: 9.20e+0]
```


