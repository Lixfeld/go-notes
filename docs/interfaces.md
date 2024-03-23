# Interfaces
An interface contains a collection of method signatures.  
Interfaces are implemented implicitly. There is no `implements` keyword.  

```go
// Declaration
type name interface{}

type Shape interface {
	Area() float64
}

// Struct for implementation
type rectangle struct {
    width, height float64
}

func (r rectangle) Area() float64 {
    return r.Width * r.Height
}
```

## The empty interface

An empty interface (`interface{}` or `any` with Go 1.18+) is implemented by all types.  

## Type assertions
Access the underlying concrete type of an interface with type assertion.  

```go
var i interface{} = "text"

// panic if type is wrong
var s string = i.(string)

// check type
s, ok := i.(string)
```

## Type switches
Instead of the specific type, the keyword `type` is used.  

```go
var i interface{} = 1

switch v := i.(type) {
case int:
    // type of v = int
case string:
    // type of v = string
default:
    // type of v = same type as i
}
```