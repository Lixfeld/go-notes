# Project Layout
Small and simple projects can have all their code in one directory:  

```
project-root-directory/
  go.mod
  modname.go
  modname_test.go
```

Large server project example:  
```
project-root-directory/
  go.mod
  internal/
    auth/
      ...
    metrics/
      ...
    model/
      ...
  cmd/
    api-server/
      main.go
    metrics-analyzer/
      main.go
    ...
  ... the project's other directories with non-Go code
```

For more information about the layout, see [Organizing a Go module](https://go.dev/doc/modules/layout) and [Standard Go Project Layout](https://github.com/golang-standards/project-layout).  
