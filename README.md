# Number Methods

**toString()** returns a number as a string

```javascript
  let x = 123;
  console.log(typeof x);    // [output: number]
  let newX = x.toString();
  console.log(typeof newX); // [output: string]
```

**toExponential()** 
* returns a string, with a number rounded and written using exponential notation </br>
* parameter defines the number of characters behind the decimal point

```javascript
  let x = 9000;
  let y = 9.2;
  
  console.log(x.toExponential());  // [output: 9e+3]
  console.log(x.toExponential(1)); // [output: 9.0e+3]
  console.log(y.toExponential());  // [output: 9.2e+0]
  console.log(y.toExponential(2)); // [output: 9.20e+0]
```

**toFixed()** returns a string, with the number written with a specified number of decimals

```javascript
  let x = 9.567;

  console.log(x.toFixed());  // [output: 10]
  console.log(x.toFixed(1)); // [output: 9.6]
  console.log(x.toFixed(2)); // [output: 9.57] ***perfect for working with money
  console.log(x.toFixed(5)); // [output: 9.56700]
```

**toPrecision()**
* returns a string, with a number written with a specified length
* not only behind the decimal point but also the whole length

```javascript
  let x = 9.567;
  
  console.log(x.toPrecision());  // [output: 9.567]
  console.log(x.toPrecision(2)); // [output: 9.6] 
  console.log(x.toPrecision(5)); // [output: 9.5670]
```

## Converting Variables to Numbers

3 JavaScript methods(convert a variable to a number): </br>  
* **Number()**	-> Returns a number 
* **parseFloat()**	-> returns a floating point number
* **parseInt()** -> returns a whole number
</br> not **number methods** but global JavaScript methods, means can't access **.methodName**

**Number()**

```javascript
  console.log(Number(true));    // [output: 1]
  console.log(Number(false));   // [output: 0]
  console.log(Number("10"));    // [output: 10]
  console.log(Number("  10"));  // [output: 10]
  console.log(Number("10  "));  // [output: 10]
  console.log(Number(" 10  ")); // [output: 10]
  console.log(Number("10.33")); // [output: 10.33]
  console.log(Number("10,33")); // [output: NaN]
  console.log(Number("10 33")); // [output: NaN]
  console.log(Number("John"));  // [output: NaN]
```

**parseInt()**
* parses a string and returns a whole number[not decimal]
* spaces are allowed but Only the first number is returned

```javascript
  console.log(parseInt("-10"));      // [output: -10]
  console.log(parseInt("-10.33"));   // [output: -10]
  console.log(parseInt("10"));       // [output: 10]
  console.log(parseInt("10.33"));    // [output: 10]
  console.log(parseInt("10 20 30")); // [output: 10]
  console.log(parseInt("10 years")); // [output: 10]
  console.log(parseInt("years 10")); // [output: NaN]
```



**parseFloat()**
* parses a string and returns a number
* spaces are allowed but Only the first number is returned


```javascript
console.log(parseFloat("-10"));      // [output: -10]
console.log(parseFloat("-10.33"));   // [output: -10.33]
console.log(parseFloat("10"));       // [output: 10]
console.log(parseFloat("10.33"));    // [output: 10]
console.log(parseFloat("10 20 30")); // [output: 10]
console.log(parseFloat("10 years")); // [output: 10]
console.log(parseFloat("years 10")); // [output: NaN]
```


