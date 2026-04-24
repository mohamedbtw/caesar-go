# caesar-go

An extremely simple and fast implementation of the Caesar cipher in Go.

> **⚠️ This is no longer maintained**
> 
> Realistically, it'll still work fine, mostly because it's just the Caesar
> cipher and literally nothing special, but I'm not going to be updating or working on this
> unless I absolutely feel like it for whatever reason.
>
> There are plenty better solutions and implementations, this one was just made for the
> learning experience (and fun aspect).

## Basic Usage
Example:
```go
package main

import (
	"fmt"

	caesar "github.com/writepoems/caesar-go"
)

func main() {
	message := caesar.Encode("hello", 7)
	fmt.Printf("Encoded: %s\n", message)
	fmt.Printf("Decoded: %s\n", caesar.Decode(message, 7))
}
```

## Reference

| Function | Arguments                    | Description                         | Return Type |
|----------|------------------------------|-------------------------------------|-------------|
| `Encode` | text (string), shift (int)   | Encode a text string with a shift   | `string`    |
| `Decode` | text (string), deshift (int) | Decode a text string with a deshift | `string`    |
