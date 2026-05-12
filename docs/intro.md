---
icon: lucide/rocket
---

# Introdução e Instalação

Go (ou Golang) é uma linguagem criada pelo Google focada em:

- simplicidade
- desempenho
- concorrência
- produtividade

## Instalação

A instalação pode ser feita pelo site oficial:

```bash
https://go.dev/dl/
```

## Verificando instalação

Após instalar:

```bash
go version
```

Exemplo de saída:

```bash
go version go1.22 windows/amd64
```

## Primeiro programa

```go
package main

import "fmt"

func main() {
fmt.Println("Olá, Go!")
}
```

## Estrutura do programa

- `package main` define o pacote principal
- `import` importa bibliotecas
- `func main()` é o ponto de entrada