# Back Tics Syntex(` `) 

* can use both single and double quotes
* multiline string
* **interpolation:**  interpolate variables and expressions into strings

```javascript
  let number = 8;

  let a = `It's mango`;
  let b = `It's mango, so
  tasty`;
  let c = `Total number of mango is ${number}`;

  console.log(a); // [output: It's mango]
  console.log(b); // [output: It's mango, so tasty]
  console.log(c); // [output: Total number of mango is 8]
  
```

**Note#0** Automatic replacing of variables/expressions with real values 
is called **string interpolation.**


