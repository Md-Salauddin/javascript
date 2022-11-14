
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

## Let & Var

var: we can declar it many time as we want

```bash
  var a = 5;
  var a = 10;
```

let

* cann't be redeclared
* must be declar before use

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
