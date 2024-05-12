# Loops

The `for` loop is the only loop available in Go.

```go
for initialization; condition; post {
    // code to execute
}

for condition {
    // "while" loop
}

for {
    // infinite loop
}

for index, value := range elements {
    // foreach loop
}

for i := range integer {
    // "repeat" loop
}
```

## Examples
```go
for i := 0; i < 10; i++ {
    // break or continue
}

dictionary := make(map[string]string)
for key, value := range dictionary {
    // skip key or value with '_'
}
```