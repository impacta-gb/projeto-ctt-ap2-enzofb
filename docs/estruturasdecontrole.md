---
icon: simple/markdown
---

# Estruturas de Controle

## If

```go
idade := 18

if idade >= 18 {
fmt.Println("Maior de idade")
}
```

## Else

```go
if idade >= 18 {
fmt.Println("Maior")
} else {
fmt.Println("Menor")
}
```

## For

```go
for i := 0; i < 5; i++ {
fmt.Println(i)
}
```

## While em Go

Go não possui `while`.

```go
contador := 0

for contador < 5 {
contador++
}
```

## Switch

```go
dia := 1

switch dia {
case 1:
fmt.Println("Domingo")

case 2:
fmt.Println("Segunda")
}
```