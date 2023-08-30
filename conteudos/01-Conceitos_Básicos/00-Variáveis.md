# Variáveis

Em F#, usamos o `let` para declarar variáveis:

```fs
let nome = "Seu Nomito"
```

Definimos uma variável chamada nome, e agora podemos utilizá-la no nosso programa normalmente:

```fs
printfn "Olá, %s" nome
```

Certo, mas e para redefini-la? A sintaxe para atribuir outro valor a uma variável é seguinte:

```fs
nome <- "Nomito Seu"
```

Porém, se você tentar executar o programa com essa instrução, vai dar erro. Mas por quê? :(

Isso acontece porque no F# todos os dados são **IMUTÁVEIS** por padrão. Ou seja, uma vez atribuído um valor para a
variável, você não pode mudá-lo. Se quiser fazer isso, precisa utilizar a instrução `mutable` antes do nome da variável.
Vamos alterar a declaração da variável `nome` para torná-la mutável:

```fs
let mutable nome = "Seu Nomito"

nome <- "Nomito Seu"
```

Agora seu programa funciona normalmente.

Você pode achar, à primeira vista, que isso imutabilidade algo ruim, e que o valor deveria ser mutável por padrão. Mas a
verdade que a mutabilidade é a fonte de muitos erros, além de que dados imutáveis são mais fáceis de paralelizar e mais
fáceis de prever o comportamento.

## Agora é a sua vez!

Em um script F# (arquivo no formato `.fsx`) crie duas variáveis, uma imutável (padrão) e outra mutável, tente atribuir
um novo valor para ambas e veja o que acontece. Para executar o script, pode usar o mesmo comando do Hello World:

```
dotnet fsi NomeDoScript.fsx
```

