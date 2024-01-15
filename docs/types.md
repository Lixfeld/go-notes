# Basic data types
```go
bool

string

int  int8  int16  int32  int64
uint uint8 uint16 uint32 uint64 uintptr

byte // alias for uint8

rune // alias for int32 (Unicode code point)

float32 float64

complex64 complex128
```

## Zero values
Variables declared without an initial value are set to their zero values:

- `0` for numbers
- `""` for strings
- `false` for booleans

## Type conversions
Type conversions `T(x)` must be explicit and different types need to be compatible.

```go
var f float64 = 1.2
// fraction is discarded
var i int = int(f)

var s string = "Hello World"
var r []rune = []rune(s)
var b []byte = []byte(s)
```

### [Package strconv](https://pkg.go.dev/strconv)
Conversions to and from string representations of basic data types.  

```go
// Integer To ASCII
s := strconv.Itoa(10)
// Equivalent to ParseInt(s, 10, 0)
i, err := strconv.Atoi("10")
```