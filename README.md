### GO 类型转换工具
```
this version fork from github.com/coderhaoxin/go-convert
````

### Install
```bash
go get github.com/xjtdy888/convert
```


### Example

```go
package main

import (
  "github.com/xjtdy888/convert"
  "reflect"
  "fmt"
)

func main() {
  var s = "10086"
  i, _ := convert.Int(s)
  i32, _ := convert.Int32(s)
  i64, _ := convert.Int64(s)
  f32, _ := convert.Float32(s)
  f64, _ := convert.Float64(s)

  fmt.Println(i, i32, i64, f32, f64)
  fmt.Println(reflect.TypeOf(i), reflect.TypeOf(i32), reflect.TypeOf(i64), reflect.TypeOf(f32), reflect.TypeOf(f64))

}
```