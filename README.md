# Operator

* Arithmetic
* Assignment
* Comparison 
* Logical 
* Conditional
* Type

## Arithmetic
+, -, *, /, %, ++, --,	
**	(Exponentiation [power])

```javascript
  console.log(2**2); [output: 4]
```

## Assignment

=, +=, -=, *=, /=, %=,	
**= (x **= y [x = x ** y])

* Note#1 When used on strings, the + operator is called the concatenation operator.


## Comparison
==, ===, !=, !==, >, <, >=, <=, ?

* !== [not equal value or not equal type]
1. Same value and different type = 'true'.
2. Same value and same type = 'false'.
3. Diffrent value and differnt type = 'true'.
4. Differnt value and same type = 'true'.

```javascript
  a = 2;
  b = "3"
  console.log(a !== 2); [output: false]
  console.log(a !== 1); [output: true]
  console.log(b !== "2"); [output: true]
  console.log(b !== 3); [output: true]
```

* === [not equal value or not equal type]
1. Same value and different type = 'false'.
2. Same value and same type = 'true'.
3. Diffrent value and differnt type = 'false'.
4. Differnt value and same type = 'false'.

```javascript
  a = 2;
  b = "3";
  console.log(a !== 2); [output: true]
  console.log(a !== 1); [output: false]
  console.log(b !== "2"); [output: false]
  console.log(b !== 3); [output: false]
```

## Logical
&&, ||, !

## Type
* typeof [Returns the type of a variable]

```javascript
  a = 2;
  b = "3"
  console.log(typeof(a)); [output: number]
  console.log(typeof(b)); [output: string]
```

* instanceof  [Returns true if an object is an instance of an object type]


## Bitwise 
&, |, ~, ^, <<, >>, >>> [unsign right shift]


## Operators & Operands
The numbers (in an arithmetic operation) are called operands.

| operand  | operator | operand |
| -------- | -------- |-------- |
|    100   |     +    |  100    |

