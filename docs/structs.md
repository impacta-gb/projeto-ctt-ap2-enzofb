---
icon: simple/markdown
---

# Structs em Go

Structs são estruturas utilizadas para agrupar diferentes tipos de dados em um único objeto.

## Exemplo básico

```go
package main

import "fmt"

type Pessoa struct {
    Nome  string
    Idade int
}

func main() {
    usuario := Pessoa{
        Nome:  "Enzo",
        Idade: 17,
    }

    fmt.Println(usuario.Nome)
    fmt.Println(usuario.Idade)
}
```

## Como funcionam

Uma struct permite criar tipos personalizados.

No exemplo acima:

- `Nome` é do tipo string
- `Idade` é do tipo int

## Vantagens

- Organização de dados
- Reutilização de código
- Melhor estruturação do programa

## Métodos em Structs

Também é possível criar métodos para structs.

```go
package main

import "fmt"

type Pessoa struct {
    Nome string
}

func (p Pessoa) Saudacao() {
    fmt.Println("Olá,", p.Nome)
}

func main() {
    usuario := Pessoa{
        Nome: "Enzo",
    }

    usuario.Saudacao()
}
```