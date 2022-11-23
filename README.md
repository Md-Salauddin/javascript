
# Function

```javascript
  function functionName(param1, param2, ...) {
    // body
    // returnType or none [for none, by default return undefined]
  }
  // function calling(invocation)
  functionName(argument1, argument2, ...)
```

* Parameters are listed inside the parentheses ()
* Arguments are the values received by the function 

```javascript
  function add(a, b) {
	console.log("hello");
	// by default return undefined   
	// return undefined
  }

  console.log(add(2,2)); // [output: hello undefined]
```

# Object

```javascript
  const student = {
  	name: "Mr. Xyz",
	age: 20,
	mobile: "0000000000",
	getName: function() {
		console.log(this.name);
	} // object method
  } // -> literal syntax
  
  console.log(student.mobile); // [output: 00000000000]
  car.getName(); // [output: Mr. Xyz] 
  
  // method without (), it will return function definition
  console.log(car.start); // [output: [Function: getName]]
```
note#1 this -> owner of the function, getName() function owner is student


```javascript
  let x = 5; // literal syntex, it will give number
  let y = new Number(5); // it will give a object

  console.log(typeof x); // [output: number]
  console.log(typeof y); // [output: object]
```


