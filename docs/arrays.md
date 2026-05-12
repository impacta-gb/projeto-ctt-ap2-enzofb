---
icon: simple/markdown
---

# Arrays em Go

Arrays armazenam múltiplos valores do mesmo tipo.

## Exemplo

```go
package main

import "fmt"

func main() {
    numeros := [3]int{1, 2, 3}

    fmt.Println(numeros)
}
```

---

## `docs/goroutines.md`

Conteúdo sobre concorrência.

Exemplo:

```md id="v78ktq"```

## Slices

Slices são estruturas dinâmicas derivadas de arrays.

```go
nomes := []string{"Ana", "Carlos", "Pedro"}
```

## Append

```go
nomes = append(nomes, "Lucas")
```

```md id="e2wlko"

## Maps

Maps armazenam dados em formato chave-valor.

```go
usuario := map[string]string{
    "nome": "Enzo",
    "cidade": "São Paulo",
}
```

## Acessando valores
---
```go
fmt.Println(usuario["nome"])
```

!!! warning
Arrays possuem tamanho fixo, enquanto slices possuem tamanho dinâmico.