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
