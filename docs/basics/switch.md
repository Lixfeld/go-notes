# Switch statement
In Go a `break` statement is added implicitly at the end of each case.  
The `fallthrough` keyword can be used to also execute the next case.  

```go
// Multiple values
switch month {
case 1, 2, 3:
	fmt.Println("Spring")
case 4, 5, 6:
	fmt.Println("Summer")
case 7, 8, 9:
	fmt.Println("Autumn")
case 10, 11, 12:
	fmt.Println("Winter")
}

// No condition
switch {
case hour < 12:
	fmt.Println("AM")
case hour < 24:
	fmt.Println("PM")
default:
	fmt.Println("Invalid")
}
```
