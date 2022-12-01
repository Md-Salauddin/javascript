# String Methods

```javascript
  const name = "banana"; 
```

This is primitive type data but when we use . (dot) then it treats as an 
object by the compiler and is able to access the properties of the String class

```javascript
console.log(name.length);
```

## slice(a, b)
a = start position, b = end position

**Note 1#** b must be grater than a </br>
**Note 2#** if we pass one param, it will start from that position and select till the end

```javascript
  let str = "Apple, Banana, Kiwi"; 
  console.log(str.slice(7, 13));   // [output: Banana]
  console.log(str.slice(-12, -6)); // [output: Banana]
  console.log(str.slice(7));       // [output: Banana, Kiwi]
  console.log(str.slice(-12));     // [output: Banana, Kiwi]
```

```javascript
-------------------------------------------------------------
 A |p |p |l |e |, |  |B |a |n |a |n |n |a |, |  |K |i |w |i |
-------------------------------------------------------------
|0 |1 |2 |3 |4 |5 |6 |7 |8 |9 |10|11|12|13|14|15|16|17|18|19|  -> for positive
-------------------------------------------------------------
|19|18|17|16|15|14|13|12|11|10|9 |8 |7 |6 |5 |4 |3 |2 |1 |0 |  <- for negative
-------------------------------------------------------------
//7 to 13   = banana
//-12 to -6 = banana
```

## substring(a, b)

substring is similar to slice(), but not supported negative value. if we provide any, it would be **zero**.

```javascript
  let str = "Apple, Banana, Kiwi"; 
  console.log(str.substring(7, 13));       // [output: Banana]
  // act as str.substring(0)
  console.log(str.substring(-12));         // [output: Apple, Banana, Kiwi]
  console.log(str.substring(7));           // [output: Banana, Kiwi]
``` 

## substr(a, b)

substr is similar to slice(), but b specifies the **length** of the extracted part.

```javascript
  let str = "Apple, Banana, Kiwi"; 
  console.log(str.substring(7, 6));        // [output: Banana]
  console.log(str.substring(-4, 2));       // [output: Ki]
  console.log(str.substring(-4));          // [output: Banana, Kiwi]
  console.log(str.substring(7));           // [output: Banana, Kiwi]
``` 





