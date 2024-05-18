# Package [strconv](https://pkg.go.dev/strconv)
Package strconv implements conversions to and from string representations of basic data types.  

Useful Functions:  
```go
Atoi(s string) (int, error)
Itoa(i int) string
ParseInt(s string, base int, bitSize int) (i int64, err error)
FormatInt(i int64, base int) string
```