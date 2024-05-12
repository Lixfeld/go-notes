# Data types
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
- `""` for strings (can not be nil)
- `false` for booleans
