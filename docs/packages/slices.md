# Package [slices](https://pkg.go.dev/slices)
**Released in Go 1.21**  
Package slices defines various functions useful with slices of any type.  

Useful Functions:  
```
Contains[S ~[]E, E comparable](s S, v E) bool
Index[S ~[]E, E comparable](s S, v E) int

Compare[S ~[]E, E cmp.Ordered](s1, s2 S) int
Equal[S ~[]E, E comparable](s1, s2 S) bool

Min[S ~[]E, E cmp.Ordered](x S) E
Max[S ~[]E, E cmp.Ordered](x S) E

Reverse[S ~[]E, E any](s S)
Sort[S ~[]E, E cmp.Ordered](x S)
```