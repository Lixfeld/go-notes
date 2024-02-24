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