## Table of Contents

- [Java CheatSheet for Developers](#java-cheatsheet-for-developers)
	- [Data Types](#data-types)
	- [Data Conversion](#data-conversion)
		- [String to Number](#string-to-number)
		- [Any Type to String](#any-type-to-string)
		- [Numeric Conversions](#numeric-conversions)
	- [Operators](#operators)
	- [Statements](#statements)
		- [If Statement](#if-statement)
		- [While Loop](#while-loop)
		- [Do-While Loop](#do-while-loop)
		- [For Loop](#for-loop)
		- [For Each Loop](#for-each-loop)
		- [Switch Statement](#switch-statement)
		- [Exception Handling](#exception-handling)
	- [String Methods](#string-methods)
	- [Math Library Methods](#math-library-methods)
	- [Types of Variables](#types-of-variables)
	- [Java Regex](#java-regex)
		- [Matcher Class](#matcher-class)
	- [Inheritance in Java](#inheritance-in-java)
		- [Single Inheritance:](#single-inheritance)
		- [Multi-Level Inheritance:](#multi-level-inheritance)
		- [Hierarchical Inheritance](#hierarchical-inheritance)
		- [Hybrid Inheritance:](#hybrid-inheritance)
	- [NOTE](#note)
  - [Collections](#collections)

# Java CheatSheet for Developers

## Data Types
| Data Type | Size |
|--|--|
| boolean | 1 bit |
| char | 2 byte |
| int | 4 byte |
| short | 2 byte| 
|long |8 byte |
|float|4 byte|
|double|8 byte |

**[🔼Back to Top](#table-of-contents)**

## Data Conversion

### String to Number

```java
    int i = Intege­r.p­ars­eInt(_str_);  
	double d = Double.pa­rse­Double(_str_);
```

**[🔼Back to Top](#table-of-contents)**

### Any Type to String

```java
	String s = String.va­lueOf(_value_);  

```

**[🔼Back to Top](#table-of-contents)**

### Numeric Conversions

```java
	int i = (int) _numeric expression_; 

```

**[🔼Back to Top](#table-of-contents)**

## Operators

| Operator Category | Operators |
|--|--|
| Arithmetic operators |+, -, /, *, %  |
|Relational operators|<, >, <=, >=,==, !=|
|Logical operators|&&, \|\||
|Assignment operator|=, +=, −=, ×=, ÷=, %=, &=, ^=, \|=, <<=, >>=, >>>=|
|Increment and Decrement operator|++ , - -|
|Conditional operators|?, :|
|Bitwise operators|^, &, \||
|Special operators|. (dot operator to access methods of class)|

**[🔼Back to Top](#table-of-contents)**

## Statements

### If Statement

```java
if ( _expression_ ) {  
­ _statements_  
} else if ( _expression_ ) {  
­ _statements_  
} else {  
­ _statements_  
}  
```

**[🔼Back to Top](#table-of-contents)**

### While Loop 

```java
while ( _expression_ ) {  
­ _statements_  
}  
```

**[🔼Back to Top](#table-of-contents)**

### Do-While Loop 

```java
do {  
­ _statements_  
} while ( _expression_ ); 
```

**[🔼Back to Top](#table-of-contents)**

### For Loop

```java
for ( int i = 0; i < _max_; ++i) {  
­ _statements_  
}  
```

**[🔼Back to Top](#table-of-contents)**

### For Each Loop

```java
for ( _var_ : _collection_ ) {  
­ _statements_  
} 
```

**[🔼Back to Top](#table-of-contents)**

### Switch Statement

```java
switch ( _expression_ ) {  
­ case _value_:  
­ ­ ­ _statements_  
­ ­ ­ ­break;  
­ case _value2_:  
­ ­ ­ _statements_  
­ ­ ­ ­break;  
­ ­def­ault:  
­ ­ ­ _statements_  
} 
```

**[🔼Back to Top](#table-of-contents)**

### Exception Handling

```java
try {  
­ ­sta­tem­ents;  
} catch (_Except­ionType_  _e1_) {  
­ ­sta­tem­ents;  
} catch (Exception _e2_) {  
­ ­cat­ch-all statem­ents;  
} finally {  
­ ­sta­tem­ents;  
}
```

**[🔼Back to Top](#table-of-contents)**

## String Methods

| Command |Description  |
|--|--|
|length | length of string |
|charAt(_i_) |extract _i_th character  |
|subst­ring(_start_, _end_) |substring from _start_ to _end_-1  |
|toUpp­erC­ase() |returns copy of _s_ in ALL CAPS  |
|toLow­erC­ase() |returns copy of _s_ in lowercase  |
|indexOf(_x_) |index of first occurrence of _x_  |
|replace(_old_, _new_)|search and replace  |
|split(_regex_) |splits string into tokens  |
|trim()  |trims surrounding whitespace  |
|equals(_s2_)  |true if s equals s2  |
|equalsIgnoreCase(_s2_) | true if s equals s2 ignoring the upper/lowercase |
|compareTo(_s2_)  | 0 if equal/+ if s > s2/- if s < s2 |
|concat(_s2_) | appends s2 to the end of s |
|contains(_s2_) | Checks whether a s contains a sequence of characters (s2) |
|replace(_s2_) | Searches the specified string s2 , and returns a new string where the specified values are replaced |
|toCharArray() | Converts the string to a new character array |

**[🔼Back to Top](#table-of-contents)**

## Math Library Methods

|Command|Description|
|--|--|
|abs(_x_)|abstract value of x|
|max(a, b|maximum of a and b|
|min(a, b)|minimum of a and b|
|E|value of _e (constant)_|
|sin(theta)| sine of theta|
|cos(theta|cosine of theta|
|tan(theta)|tangent of theta|
|round(_x_)| Returns the value of x rounded to its nearest integer|

**[🔼Back to Top](#table-of-contents)**

## Types of Variables

|Variable Type|Scope|Lifetime|
|--|--|--|
|Instance variable|Throughout the class except in<br /> static methods|Until the object is available in the<br />memory|
|Class variable|Throughout the class|Until the end of the program|
|Local variable|Within the block in which it is<br />declared|Until the control leaves the block<br />in which it is declared| 

**[🔼Back to Top](#table-of-contents)**

## Java Regex 

### Matcher Class

|Method|Description|
|--|--|
|matches()|tests whether the regex matches the pattern|
|find()|finds the next expression that matches the pattern|
|find(int a)| finds the next expression that matches from the start number _a_|
|group()|returns the matched subsequence |
|start()|returns the starting index of the matched subsequence|
|end()|returns the ending index of the matched subsequence|

**[🔼Back to Top](#table-of-contents)**

## Inheritance in Java

> Inheritance - It is the property of a child/derived/subclass, allowing it to inherit the properties() and functionalities or data members methods from its parent/base/superclass.  

___Java supports 4 types of inheritance:___

1.	Single Inheritance
2.	Multi-level Inheritance
3.	Hierarchical Inheritance
4.	Hybrid Inheritance 

**[🔼Back to Top](#table-of-contents)**

### Single Inheritance: 

> As the title indicates, just one class is subject to this kind of inheritance. The parent class gives rise to just one child class. 

___Syntax:___

```java
Class A{
  //your parent class code
}
Class B extends A {
   //your child class code
} 
```

**[🔼Back to Top](#table-of-contents)**

### Multi-Level Inheritance:

> In multi-level inheritance, one class has more than one parent class but at different levels of inheritance.  

___Syntax:___

```java
Class A{
  //your parent class code
}
Class B extends A {
   //your code
}
Class C extends B {
    //your code 
} 
```

**[🔼Back to Top](#table-of-contents)**

### Hierarchical Inheritance

> In hierarchical inheritance, one parent can have one or more child/sub/derived classes.

___Syntax:___

```java
Class A{
  //your parent class code
}
Class B extends A {
   //your child class code
}
Class C extends A {
    //your child class code 
}
```

**[🔼Back to Top](#table-of-contents)**

### Hybrid Inheritance:

> Hybrid Inheritance is the combination of more than one type of inheritance in a single program. 

**[🔼Back to Top](#table-of-contents)**

## NOTE

> Multiple inheritance is not supported in Java as it leads to the diamond problem. <br /> We can achieve Multiple inheritance in Java by using the concept of Abstraction.

**[🔼Back to Top](#table-of-contents)**

## Collections

|Collection|Description|
|-----|-----|
|Set| Set is a collection of elements which can not contain duplicate values. Set is implemented in HashSets, LinkedHashSets, TreeSet etc|
|List| List is a ordered collection of elements which can have duplicates. Lists are classified into ArrayList, LinkedList, Vectors|
|Queue| FIFO approach, while instantiating Queue interface you can either choose LinkedList or PriorityQueue.|
|Stack| LIFO approach, stack is a sub ordinate of vector which helps in performing different functions.|
|Deque| Deque(Double Ended Queue) is used to add or remove elements from both the ends of the Queue(both head and tail)|
|Map| Map contains key-values pairs which don't have any duplicates. Map is implemented in HashMap, TreeMap etc.|

**[🔼Back to Top](#table-of-contents)**
