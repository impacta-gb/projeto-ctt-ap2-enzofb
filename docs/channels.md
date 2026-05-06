---
icon: simple/markdown
---

# Channels em Go

Channels permitem comunicação entre goroutines.

## Exemplo

```go
package main

import "fmt"

func main() {
    mensagem := make(chan string)

    go func() {
        mensagem <- "Olá do channel!"
    }()

    texto := <-mensagem

    fmt.Println(texto)
}
```

## Vantagens

- Comunicação segura
- Sincronização entre goroutines
- Concorrência eficiente