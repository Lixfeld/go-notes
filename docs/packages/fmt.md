# Package [fmt](https://pkg.go.dev/fmt)
Package fmt implements formatted I/O with functions analogous to C's printf and scanf.  
The format 'verbs' are derived from C's but are simpler.  

Useful Functions:  
```
Errorf(format string, a ...any) error
Fprint(w io.Writer, a ...any) (n int, err error)
Printf(format string, a ...any) (n int, err error)
Sprintf(format string, a ...any) string
```

Common format verbs:
```
%b	    integer (base 2)
%d      integer (base 10)
%o      integer (base 8)
%q      quoted string "abc" or rune 'c'
%s      string
%T	    type of any value
%v      the value in a default format
%+v     structs: adds field names
%%      literal percent sign (no operand)
```
