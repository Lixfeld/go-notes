# Package [unicode](https://pkg.go.dev/unicode)
Package unicode provides data and functions to test some properties of Unicode code points.  

Useful Functions:  
```go
ToLower(r rune) rune
ToUpper(r rune) rune

IsLetter(r rune) bool
IsNumber(r rune) bool
IsDigit(r rune) bool
```