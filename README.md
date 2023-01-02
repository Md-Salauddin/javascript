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

**Arrays** are Objects

```javascript
  console.log(typeof elements) // [output: object]
```

**access** last element

```javascript
  console.log(names[names.length - 1])
```
