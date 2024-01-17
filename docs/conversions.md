# Type conversions
Type conversions `T(x)` must be explicit and different types need to be compatible.

```go
var f float64 = 1.2
// fraction is discarded
var i int = int(f)

var s string = "Hello World"
var r []rune = []rune(s)
var b []byte = []byte(s)
```

## [Package strconv](https://pkg.go.dev/strconv)
Conversions to and from string representations of basic data types.  

```go
// Integer To ASCII
s := strconv.Itoa(10)
// Equivalent to ParseInt(s, 10, 0)
i, err := strconv.Atoi("10")
```