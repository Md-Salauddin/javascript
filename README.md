# Array

can also create an array, and then provide the elements. <br/>
<br/>
elements can store:  
* objects in an Array 
* functions in an Array 
* arrays in an Array

```javascript
  function  message() {
    return "JS in 30 Day's"
  }
  
  const elements = [];
  
  elements[0] = "kawser";
  elements[1] = "sk";
  elements[2] = 100;
  elements[3] = message();

  console.log(elements[3]); // [output: JS in 30 Day's]
```

**arrays** are objects

```javascript
  console.log(typeof elements) // [output: object]
```

**access** last element

```javascript
  console.log(names[names.length - 1])
```

**push & forEach** method

```javascript
  function  print(value) {
    console.log(value);
  }

  elements.push("Md.")
  elements.forEach(print); 
  // [output:
  // kawser
  // sk
  // 100
  // JS in 30 Day's
  // Md.
  //]
```

**adding elements with high indexes can create undefined "holes" in an array**

```javascript
const fruits = ["Banana", "Orange", "Apple"];
fruits[6] = "Lemon";

console.log(fruits) // [output: [ 'Banana', 'Orange', 'Apple', <3 empty items>, 'Lemon' ]]
```
