---
icon: simple/markdown
---

# Tratamento de Erros

Go utiliza retornos explícitos de erro.

## Exemplo

```go
package main

import (
"fmt"
"os"
)

func main() {
arquivo, err := os.Open("teste.txt")

if err != nil {
fmt.Println("Erro ao abrir arquivo")
return
}

fmt.Println(arquivo.Name())
}
```

## Error Handling

Em Go, erros são tratados utilizando:

```go
if err != nil
```

!!! warning
Ignorar erros pode causar falhas inesperadas.