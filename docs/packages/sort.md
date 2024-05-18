# Package [sort](https://pkg.go.dev/sort)
Package sort provides primitives for sorting slices and user-defined collections.  

Note: As of Go 1.22, some functions simply call the corresponding functions in the slices package.  

Useful Functions:  
```go
Ints(x []int)
Strings(x []string)
Slice(x any, less func(i, j int) bool)
```