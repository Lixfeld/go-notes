# Package [fmt](https://pkg.go.dev/fmt)
Package fmt implements formatted I/O with functions analogous to C's printf and scanf.  
The format 'verbs' are derived from C's but are simpler.  

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
