# Methods
Methods are similar to functions but they operate on instances of a specific type (receiver).  
There is no `this` or`self` keyword in Go but it is a convention to use the first letter of the receiver.

```go
type rectangle struct {
    width, height float64
}

func (r rectangle) Area() float64 {
	return r.Width * r.Height
}
```

## Value and pointer receivers
A value receiver `(t T)` uses a copy of the original value.  
To modify the original value a pointer receiver  `(t *T)` is needed.  
For consistency, all methods on a type should use the same receiver type, even if not needed.  