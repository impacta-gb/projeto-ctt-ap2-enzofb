---
icon: simple/markdown
---

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

``` toml
`[build]`
source = "docs"
output = "site" ```

## Concorrência

Go possui suporte nativo a concorrência.

As goroutines executam funções simultaneamente.

## Vantagens

- Melhor desempenho
- Execução paralela
- Escalabilidade

## WaitGroup

```go
package main

import (
"fmt"
"sync"
)

func tarefa(wg *sync.WaitGroup) {
defer wg.Done()

fmt.Println("Executando")
}

func main() {
var wg sync.WaitGroup

wg.Add(1)

go tarefa(&wg)

wg.Wait()
}
```