# Chapter 02 - Hello World

---
#### [Previous Chapter](../ch01/README.md) | [Table of Contents](../README.md) | [Next Chapter](../ch03/README.md)
---


## Goal

Create a simple executable that says "Hello World"


## Let's Start

The template discussed in Chapter 01 has been provided in [ch02.go](ch02.go)

### Package Name
There's a special package name that indicates this is the entry point to a runnable program vs a library. It's called `main`. Let's use that.

### Imports
We need to print out some text. `"fmt"` handles I/O and can be used to write to screen, file, or any destination. If you want to look at all the standard libraries check out this [link](https://golang.org/pkg/)

```go
import "fmt"
```

### Code

#### Functions

##### sayHello()
Let's create a function that returns a string (which will be "Hello World").

```go
func sayHello() string {
	return "Hello World"
}
```

*Note: For those coming from other languages, the return value(s), is at the end of the function declaration*

##### main()
Whenever we use the package name `main`, Go is expecting you to have a `main` function which will be the entrypoint. Let's setup our program to  call the `sayHello` function and print out the returned string.

```go
func main() {
	fmt.Println(sayHello())
}

```

### Execution

`$ go run ch02.go`


### Full Code
```go
package main

import "fmt"

func sayHello() string {
	return "Hello World"
}

func main() {
	fmt.Println(sayHello())
}
```

---
#### [Previous Chapter](../ch01/README.md) | [Table of Contents](../README.md) | [Next Chapter](../ch03/README.md)
---
