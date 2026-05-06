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

# Goroutines

Goroutines permitem executar funções concorrentemente.

## Exemplo

```go
package main

import (
    "fmt"
    "time"
)

func tarefa() {
    fmt.Println("Executando...")
}

func main() {
    go tarefa()

    time.Sleep(time.Second)
}
```

---

## `docs/markdown.md`

Pode ser uma página explicando:

- sintaxe markdown
- como documentar
- exemplos

ou outro tema da atividade.

---

# 2. `site/`

IMPORTANTE:

Você NÃO escreve nada aqui manualmente.

Essa pasta é gerada automaticamente pelo Zensical.

Ela contém:

- HTML
- CSS
- sitemap
- páginas compiladas

Então:

✅ pode existir  
❌ não precisa editar manualmente

---

# 3. `zensical.toml`

Esse arquivo configura o site.

Aqui você define:

- nome
- diretório docs
- saída
- tema

Exemplo simples:

``` toml id="g0fq5u"
title = "Documentação Go" ```

``` [build]
source = "docs"
output = "site" ```