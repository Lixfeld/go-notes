# Structs
A struct can group data with different types.  

```go
// Declaration
type name struct{}

// Named fields in a struct
type Point struct {
	X int
	Y int
}

// New struct
var p1 = Point{1, 2}
var p2 = Point{X: 1, Y: 2}

// Zero values
var p3 Point = Point{}
```

Fields can be accessed with a struct pointer without explicit dereference.  
Example: Write `p.X` instead of `(*p).X`.  