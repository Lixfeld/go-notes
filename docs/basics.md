# Basics
Program execution begins by initializing the `main` package and then invoking the function `main`.

## Hello World
```go
package main

import "fmt"

func main() {
    fmt.Println("Hello, World!")
}
```

## Exported names
If a name begins with an upper-case letter, it is `exported` (PascalCase).  
Any `unexported` (camelCase) names are not visible or accessible from outside the package.  

There are no access modifiers such as `public` or `private`.

## Keywords
Language Specification: https://go.dev/ref/spec#Keywords
```
break        default      func         interface    select
case         defer        go           map          struct
chan         else         goto         package      switch
const        fallthrough  if           range        type
continue     for          import       return       var
```
