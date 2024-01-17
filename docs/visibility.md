# Visibility
If a name begins with an upper-case letter, it is `exported` (PascalCase).  
Any `unexported` (camelCase) names are not visible or accessible from outside the package.  

There are no access modifiers such as `public` or `private`.

## Internal packages
Put code which should not be used outside the program in a directory named `internal`.  

Go 1.4 release notes: <https://golang.org/doc/go1.4#internalpackages>  
