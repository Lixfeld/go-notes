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