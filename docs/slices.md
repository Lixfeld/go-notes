# Slices
A slice is like a reference to an array.  
The length of a slice can change by re-slicing or appending items.  

```go
// Create a slice from an array
var array = [5]int{0, 1, 2, 3, 4}
// The "end" element is excluded
var slice = array[start:end]

// Slice literal
var hello = []byte{'h', 'e', 'l', 'l', 'o'}

// Make a slice with zero values
var name = make([]type, length, capacity)
```

## Appending to a slice
The built-in append function also works on nil slices.

```go
var slice []int
slice = append(slice, 1)

var slice2 = []int{2, 3}
// ... unpacks the second slice
slice = append(slice, slice2...)
```
## Empty slice
Check for an empty slice with `len(s) == 0` and not `s == nil` because for example `s := []int{}` is not nil.
