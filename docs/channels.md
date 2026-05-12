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

## Tipos de Channels

### Unbuffered Channel

```go
canal := make(chan string)
```

### Buffered Channel

```go
canal := make(chan string, 2)
```

## Enviando dados

```go
canal <- "Olá"
```

## Recebendo dados

```go
mensagem := <-canal
```

## Fechando channel

```go
close(canal)
```

!!! note
Channels ajudam a evitar problemas de concorrência.