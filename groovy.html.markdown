---
language: groovy
author: Gareth Davis
---

Groovy is dynamic language for the JVM and builds upon the strengths of Java but has additional power features inspired by languages like Python, Ruby and Smalltalk.

```groovy

// java style single line and 
/*
Multi line comments
*/

/*
  1. Primitive Datatypes and Operators
*/

// You have numbers
3 //=> 3
123123123123L # 64 bit number

// Math is as expected

1 + 1 //=> 2
8 - 1 //=> 7
10 * 2 //=> 20
35 / 5 //=> 7

// division can result in a decimal
5 / 2 //=> 2.5

// booleans
true
false

// negation
!true
!false

// equality is not the same as java 
// == will call .equals() or .compareTo() if implemented
1 == 1 // true
2 == 1 // false

// inequality is
1 != 1 // false
2 != 1 // true

// standard comparsions all work in a familar way
1 < 10 // => true
1 > 10 // => false
2 <= 2 // => true
2 >= 2 // => true

// and can be combined using logical operators

1 < 2 && 2 < 3 // => true
3 < 3 || 3 < 2 // => false

// String literals are defined in multiple ways
"Java Style double quotes"
'Single quotes'
"""Multiple 
line strings"""

/^regex style$/ 

// String interpolation ${}
"Strings ${10}"  // can include any expression
"10 is half of ${10 * 2}" // => 10 is half of 20

// Variables and types

def a    // variables do need to be declared, but the type is optional
String s = "FooBar" // java style prefix type 

// Generics are the same as Java
List<String> listOfStrings

Map<Integer,String> intToStringMap

// Collections

def myList = [1,2,3,4,5] // list of integers, will be a java.util.ArrayList
List<String> strings = ["foo","bar"] 
  
// collections are zero indexed
myList[0]  // => 1 
// negative indexes 
myList[-1] // => 5 
// slicing using ranges
myList[0..2] // => [1, 2, 3] 

def m1 = [ "key1":"value1", "key2":"value2" ]
def m2 = [ key1:"value1" ] // special case of string keys, the quotes can be omitted

// accessed via 'property' style
m1.key1    // => value1 
// array index style
m1["key1"] // => value1 
// printing to standard out

println("something to output")

println "parens can be omitted in somecases"
```
