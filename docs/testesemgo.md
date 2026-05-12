---
icon: simple/markdown
---

# Testes Automatizados

Go possui suporte nativo para testes.

## Arquivo de teste

```go
package main

import "testing"

func Soma(a int, b int) int {
return a + b
}

func TestSoma(t *testing.T) {
resultado := Soma(2, 2)

if resultado != 4 {
t.Error("Erro no teste")
}
}
```

## Executando testes

```bash
go test
```

## Benefícios

- Maior confiabilidade
- Menos bugs
- Facilidade de manutenção