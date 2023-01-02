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

**JavaScript does not support arrays with named indexes**
arrays with named indexes are called associative arrays (or hashes), in JavaScript, arrays always use numbered indexes. <br/>
if we use named indexes, JavaScript will redefine the array to an object. after that, some array methods and properties <br/>
will produce incorrect results.

```javascript
  const person = [];
  person["name"] = "Babul";
  person["mobile_no"] = "01674000000";
  person["age"] = 32;
  
  console.log(person.length);     // [output: 0]
  console.log(person[0]);         // [output: undefined]
```

**A Common Error**

1. const names = [40]; & </br>
2. const names = new Array(40); </br>
- is not the same as </br>

* first one create an array with one element
* second one create an array with 40 undefined elements


