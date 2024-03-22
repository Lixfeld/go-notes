# Interfaces
An interface contains a collection of method signatures.  
Interfaces are implemented implicitly. There is no `implements` keyword.  

```go
// Declaration
type name interface{}

type Shape interface {
	Area() float64
}

type rectangle struct {
    width, height float64
}

func (r rectangle) Area() float64 {
    return r.Width * r.Height
}
```

## The empty interface

An empty interface (`interface{}` or `any` with Go 1.18+) is implemented by all types.  
