---
icon: simple/markdown
---

# Go Modules

Go Modules gerenciam dependências do projeto.

## Criando módulo

```bash
go mod init projeto
```

## Instalando dependência

```bash
go get github.com/gin-gonic/gin
```

## Arquivos importantes

| Arquivo | Função |
|---|---|
| go.mod | Dependências |
| go.sum | Verificação de integridade |

## Atualizando dependências

```bash
go mod tidy
```