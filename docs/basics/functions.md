# Functions

The type comes after the variable name.  

```go
func add(x int, y int) int {
	return x + y
}

// same type of parameters
func sub(x, y int) int {
	return x - y
}

// named return value
func multiply(x, y int) (z int) {
	z = x * y
	return
}

// multiple return values
func divide(x, y int) (int, int) {
	return x / y, x % y
}
```

## Defer
Defer statements delay the execution until the function that contains the defer keyword has finished.  
This is similar to a `finally` block in other languages.  

```go
func main() {
	defer fmt.Print("world")
	fmt.Print("hello ")
	// Output: hello world
}

// Multiple defer statements
func main() {	
	defer fmt.Print("done")
	for i := 1; i <= 3; i++ {
		defer fmt.Printf("%v ", i)
	}
	// Output: 3 2 1 done
}

// Cleanup resources
func main() {	
	file, err := os.Create("filename")
	if err != nil {
		panic(err)
	}
	defer file.Close()
}
```

## Variadic
A variadic function accepts any number of values as a single argument.  
The type of the last parameter is preceded by an ellipsis (`...`).  

```go
func sum(nums ...int) int {
	var total = 0
	for num := range nums {
		total += num
	}
	return total
}
```

## Default
Unlike many other languages Go does not support optional/default values.  