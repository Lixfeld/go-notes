# If statements
There is no ternary operator in Go.

```go
if condition1 {
    // condition1 is true
} else if condition2 {
    // condition2 is true
} else {
    // both conditions are false
}
```

## If with a short statement
Variables declared at the start are available inside all branches.

```go
if assignment; condition {
    // code to execute
}
```

### Example
```go
if number, err := strconv.Atoi("10"); err == nil {
    sum += number
}
```
