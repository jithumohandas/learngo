# Chapter 1 - Hello World Program

It is considered to be a custom to start any programming course by creating a **Hello World** program. This also helps to understand the structure of a **Go** program. The feeling of running the first Go program is truly rewarding and this would act as a motivation to move forward.

This chapter has two prerequisites.

> 1.  Go shall be installed in your machine
>
> 2.  You are expected to have a Go programming editor

If the prerequisites are fulfilled, lets open the code editor and create a file named `main.go` with the following code.

```go
package main

import "fmt"

func main() {
  fmt.Println("Hello World")
}
```

> **Note:**
> This code is available in this folder as `main.go` file.

After the code is saved in a file - `main.go`, We can run the code using the following command

> **go run main.go**

This shall print the line `Hello World` in the console.

## Structure of Go Program

There are 3 main sections in the above program.

1. Defining Package
2. Importing Required Packages
3. The Executable Logic

### 1. Defining Package

The package definition is the first line of a go program.

```go
package main
```

There are 2 types of packages in Go pgramming language.

| Package Type   | Use of package                                                                                                                                                                                                    |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Executable** | The executable package shall start with `package main`. One of the files belong to this package shall contain a `main` function. This main function is the starting point of the program execution.               |
| **Reusable**   | The reusable package are those packages which can be used in other programs using the `import` statement. This packages can have any name other than the package name 'main' or any existing package names of Go. |

Our `main.go` program is an executable and hence we have used the package name `main` in the code.

> **Note:**
> Any function belongs to the same package can be called in any files belongs to the same package, even the file doesn't contain the function definition.

### 2. Importing Required Packages

The `fmt` package is imported in the program to print the output to the console. This package has everal other formatting functions which we are not using in this program.

```go
import "fmt"
```

### 3. The Executable Logic

The following section contains the logic part of the program.

```go
func main() {
  fmt.Println("Hello World")
}
```

This section is responsible for printing the `Hello World` text to the screen.
