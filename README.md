# String Methods

```javascript
  const name = "banana"; 
```

This is primitive type data but when we use . (dot) then it treats as an 
object by the compiler and is able to access the properties of the String class

```javascript
console.log(name.length);
```

## String slice(a, b)
a = start position, b = end position

**Note#** b must be grater than a

```javascript
  let str = "Apple, Banana, Kiwi"; 
  console.log(str.slice(7, 13)); // [output: banana]
  console.log(str.slice(-12, -6)); // [output: banana]
```

**Note#** for short cut start counting with 1 to last

```javascript
-------------------------------------------------------
 A |p |p |l |e |, |B |a |n |a |n |n |a |, |K |i |w |i |
------------------------------------------------------
|1 |2 |3 |4 |5 |6 |7 |8 |9 |10|11|12|13|14|15|16|17|18|  -> for positive
------------------------------------------------------
|18|17|16|15|14|13|12|11|10|9 |8 |7 |6 |5 |4 |3 |2 |1 |  <- for negative
-------------------------------------------------------

//7 to 13   = banana
//-12 to -6 = banana
```
