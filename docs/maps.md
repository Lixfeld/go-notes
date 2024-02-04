# Maps
A map stores a collection of key/value pairs.  
In other languages a map is called a hash table or dictionary.   
The key type in a map (`map[keyType]valueType`) must be a comparable type.  

```go
// Create a map
var m = make(map[string]string)

// Insert or update
m["key"] = "value"

// Get element or zero value
var value = m["key"]

// Contains key
v, ok := m["key"]

// Delete
delete(m, "key")

// Map Literal
var table = map[int]string{
    1: "A",
    2: "B",
    3: "C",
}
```

## Nil map
Writing to a nil map will panic.  
Initialize a map with the built in `make` function.  
