## first go project

- `go mod init module_name` to create a `go.mod` file and make a Go project, a module
- a module in the context of Go is the Go project + it's dependencies
- `go.mod` file is similar to `requirements.txt` in python or `Gemfile` in Ruby so it should not be edited manually
- `go get` or `go mod tidy` to manage changes for the `go.mod` file

### chapter one

- every Go program is made up of packages
- Go programs start running from the package `main`
- in Go, names are only _exported_ if they begin with **captial letters**.
- functions can take zero or more parameters.
- function parameters have the type and return type declared (if the function returns data)
- if _consecutive parameters_ share a type, the type can be omited and the only set on the last
- functions can return any number of results
- return values in Go can be named. named values are defined at the top of a function.
- `naked return` statement (_a return without values_) returns the named values.
- `var` is used to declare variables. _var statement_ can be at package or function level.
- `var` declaration can include an _initializer_. if an _initializer_ is present, the variable takes up the _initializer_ data type and type declaration can be skipped.
- in functions, `:=` can be used in place of `var`
- `bool`, `string`, `int, int8,16,32 and 64`, `uint, uint8, 16, 32 and 64`,`byte (alias for uint8)`, `rune (alias for int32), represents Unicode code point`, `float32`, `float64`, `complex64` and `complex128` are the basic types in Go.
- variables without an explicit initial value are given their _zero value_ i.e `0` for numerics, `false` for booleans and `""` for strings
- assignment between items of different type requires explicit conversion.
- constants are declared with `const` keyword. constants can not be declared using `:=` syntax.
