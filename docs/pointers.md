# Pointers
A pointer variable stores the memory address of a value. There is no pointer arithmetic in Go.  

```go
// Declaration
var ptr *type

// Zero value is nil
var p *int

// Address-of operator (&)
var x = 10
p = &x

// Dereference operator (*)
fmt.Println(*p) // 10
*p = 20

fmt.Println(*p) // 20
fmt.Println(x)  // 20
```