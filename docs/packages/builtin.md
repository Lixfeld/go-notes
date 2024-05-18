# Package [builtin](https://pkg.go.dev/builtin)
Package builtin provides documentation for Go's predeclared identifiers.  
The items documented here are not actually in package builtin but their descriptions here allow godoc to present documentation for the language's special identifiers.

Useful Functions:  
```go
append(slice []Type, elems ...Type) []Type
close(c chan<- Type)
copy(dst, src []Type) int
len(v Type) int
make(t Type, size ...IntegerType) Type
```