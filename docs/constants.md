# Constants
Declaration: const name type = expression

```go
const greeting string = "Hello World"
```

## Untyped Constants
Constants can be untyped which is useful for numbers.  
The constant will be implicitly converted to the required type.  

Examples from package [math](https://pkg.go.dev/math#pkg-constants):  

```go
const (
	E        = 2.71828182845904523536028747135266249775724709369995957496696763
	Pi       = 3.14159265358979323846264338327950288419716939937510582097494459
	MaxInt8  = 1<<7 - 1 // 127
	MinInt32 = -1 << 31 // -2147483648
)
```

## Enums
Go has no enumerations but they can be mimicked by using constants.  
The value for the keyword `iota` is incremented by one after each line.  

```go
const (
	Summer int = iota // 0
	Autumn            // 1
	Winter            // 2
	Spring            // 3
)

type Direction int

const (
	North Direction = iota // 0
	East                   // 1
	South                  // 2
	West                   // 3
)
```