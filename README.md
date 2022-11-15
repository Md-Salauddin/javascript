
## Statement

instruction are called statement, js program is list of statement.
composed of values, operators, expressions, keywords, comments. 
execute one by one, the same order as it written.


## Value 

two type, one is literal(Fixed)[10, 10.5, "hello"]
other is variable [store data value, use keyword like var, let, const] 

```bash
  var a; [declaration]
  a = 5; [assign]
```

## Operator

```bash
  arithmetic: +, -, *, /
  assignment: =
```

## Let & Var & Const

var: we can declar it many time as we want

```bash
  var a = 5;
  var a = 10;
```

let

* cann't be redeclared
* must be declar before use

const

* can't be  redeclared & reassigned
* have Block Scope

```bash
  const a = 5; // allowed
  a = 10; // not allowed

  const b; // not allowed
  b = 10; // not allowed
```
Use of const: array, object, function, regExp [note#2]

note 2# const directly locked the memory address that cann't be changed. but
value can.

```bash
|___|___|___|___|___|
 10* 20  30   40  50
 
 const a = [1, 2, 3]; // will lock the address[10]
 a[0] = 3; // allowed
 a.push(4); // allowed
 
 a = [5, 6, 7, 8]; // not allowed
```

## Block scope

```bash
{
  // global scope
  {
    // block scope
    let x = 5;
    var y = 10;
  }
  // x can't be used here
  // but y can be [note#1]
}
```
note#1: for that reasone 'let' introduced into js


```bash
{
  const a = 10;
  // can be access a = 10 here
  {
    const a = 20;
    // can be access a = 20 here
  }
}
```

## Redeclaring

Example 1#
```bash
   let x = 1; //allowed
   let x = 2; //not allowed
```
Example 2#
```bash
   let x = 1; // allowed
  {
	 let x = 2; // allowed
	 let x = 3; // not allowed
  }
  {
	 let x = 3; // allowed
	 let x = 4; // not allowed
  }
```

Example 3#
```bash
  let x = 1; // allowed
  {
	 let x = 2; // allowed
  }
  {
	 let x = 3; // allowed
  }
```

Example 4#
```bash
  const x = 1; // allowed
  var x = 1; // not allowed
  {
         const x = 10; // allowed
	 let x = 2; // not allowed
  }
  {
	 const x = 3; // allowed
	 const x = 10; // not allowed
  }
```

Example 5#
```bash
  const x = 1; // allowed
  x = 1; // not allowed
  {
         const x = 10; // allowed
	 x = 2; // not allowed
  }
```

## Host

Var
```bash
        |``` [in compile time, it hosted(in top) like 
	|    var x;
	|    x = undifined]
	|
	|    | x = 10;
	|    | var x;
	|--{ | console.log(x);  [output: 10]
```

Let
```bash
        |``` [in compile time, it hosted(in top) like 
	|    let x;
	|    
	|
	|    | x = 10;
	|    | let x;
	|--{ | console.log(x);  [output: ReferenceError]
	
Const
```bash
        |``` [in compile time, it hosted(in top) like 
	|    const x;
	|    
	|
	|    
	|    | console.log(x);  [output: ReferenceError]
	|--{ | const x = 10;
