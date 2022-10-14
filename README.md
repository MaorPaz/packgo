# packgo


Learn how to Go

1. Install go lang (Ubuntu)
```shell
sudo apt install golang-go
```

2. Create main directory fo go app 
```shell
mkdir  ~/go/src/packgo

cd ~/go/src/packgo
```

Enable auto go install mod
```shell
go env -w GO111MODULE=auto
```

```shell
go install
```


Create First app

```shell
touch packgo.go
```
```go
package main

import (
	"fmt"
)

func main() {
	x := 7
	if x > 6 {
		fmt.Println("More than 6")
	}
}
```

Build executable:
```shell
go build .
```

Runtime runner:
```shell
go run packgo.go
```


#### Example:
```go
package main

import (
"fmt"
)

func main() {
	
	//var x int = 7  same as:
	//x := 7
	//var x int = 5  same as:
	//x := 5
	// var sum int = x + y same as: 
	//sum := x + y
	
    x := 7
	if x > 6 {
		fmt.Println("More than 6")
	}
}
```


## Arrays:

Array can hold multiple elements of the same type, The number of elements is fixed, is ha a specific length  

#### Example:


```go
package main

import (
"fmt"
)

func main() {
	var a [5]int
	fmt.Println(a)
}
```

When runs it will output:
```text
[0 0 0 0 0]
```

All the types in that array will be initialized with 0 type value

### Index in array
```go
package main

import (
"fmt"
)

func main() {
	var a [5]int
	a[2] = 7
	fmt.Println(a)
}
```
When runs it will output:
```text
[0 0 7 0 0]
```

### Index in array Shorten 
```go
package main

import (
"fmt"
)

func main() {
	a := [5]int{2,7}
	fmt.Println(a)
}
```



