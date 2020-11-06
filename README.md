# mypack
test go modules

# use v0
```go
package main

import (
	"log"

	"github.com/esieke/mypack/pack"
)

func main() {
	
	log.Printf("%T, %v\n", pack.GetIntFromInt(1), pack.GetIntFromInt(1))
}

```
with go mod
```
module github.com/esieke/usemypackage

go 1.15

require github.com/esieke/mypack v0.0.8
```

# use v2
```go
package main

import (
	"log"

	"github.com/esieke/mypack/v2/pack"
)

func main() {
	
	log.Printf("%T, %v\n", pack.GetIntFromInt(1), pack.GetIntFromInt(1))
}

```
with go mod
```
module github.com/esieke/usemypackage

go 1.15

require github.com/esieke/mypack/v2 v2.0.8
```
