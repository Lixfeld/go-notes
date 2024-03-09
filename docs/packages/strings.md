# Package [strings ](https://pkg.go.dev/strings)
Package strings implements simple functions to manipulate UTF-8 encoded strings.  
For information about UTF-8 strings in Go, see <https://blog.golang.org/strings>.  

Useful Functions:  
```
Contains(s, substr string) bool
HasPrefix(s, prefix string) bool
HasSuffix(s, suffix string) bool
Index(s, substr string) int
Join(elems []string, sep string) string
Repeat(s string, count int) string
ReplaceAll(s, old, new string) string
Split(s, sep string) []string
ToLower(s string) string
ToUpper(s string) string
TrimSpace(s string) string
```

Useful Types:  
```
Builder
Replacer
```