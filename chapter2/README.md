# Chapter 2 - Variable Types and Declarations

There are four basic variable types in go. This chapter discuss these variable types and how the variable declaration is done in go programs.
We also take a deeper look at some of the very useful and handy go commands.

## Basic Go Data Types

| Date Type         | Potential Values                                                                          |
| ----------------- | ----------------------------------------------------------------------------------------- |
| string            | This data type can hold string values.Example: "some string", "Google" etc.               |
| int               | This type variables can contain whole numbers.Example: 125, 100234, -1001 etc.            |
| float32 / float64 | A decimal value can be assigned to this type of variables only.Example: 555.90, 3.14 etc. |
| bool              | To store a boolean state like `true` or `false`. Example: true, false                     |

An example program with declaration and value assignment for different type of variables is shown below.

```go
package main

import "fmt"

func main() {
	var name string = "Google"
	var age int = 24
	var cost float64 = 112.65
	var onStatus bool = true

	fmt.Println(name)
	fmt.Println(age)
	fmt.Println(cost)
	fmt.Println(onStatus)
}
```

The type annotations are explicitly mentioned with each variable above. The next approach to declare and initialize a variable is as shown below. Here the type is inferred by the value assigned to the variable.

```go
var name = "Google"
var age = 24
var onStatus = true
var cost = 112.65
```

There is a better and short way of declaring variables and assigning value. The type is inferred by go based on the value assigned to the variable.

```go
// var name string = "Google"
name := "google"

// var age int = 24
age := 24

// var cost float64 = 112.65
cost := 112.65

// var onStatus bool = true
onStatus := true
```

> **Note:**
> The `:=` is only required for the first assignment of the value. When the variable is reassigned with a new value, we can just use `=`.

```go
name := "Google"

name = "Microsoft"
```

> **Complex Types**
> Go has complex variables as one of the types. Since it is not a widely used option. there are some discussions to remove it in the upcoming versions of Go.

## Useful Go Commands
