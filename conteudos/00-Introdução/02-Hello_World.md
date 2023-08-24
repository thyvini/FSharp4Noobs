# Hello World

Vamos nos livrar logo da Maldição do Hello World! Para fazer seu primeiro programa em F#, abra seu editor/IDE/ambiente
favorito, crie um arquivo com a extensão `.fsx` e digite o seguinte:

```fs
printfn "Hello World"
```

Para executar o arquivo, use o seguinte comando em seu terminal:

```
dotnet fsi NomeDoArquivo.fsx
```

Simples, não? Agora, faça seu programa te cumprimentar! Para isso, são necessárias poucas alterações:

```fs
let nome = "Seu Nomito"
printfn "Hello %s" nome
```

Rode novamente o script com o mesmo comando:

```
dotnet fsi NomeDoArquivo.fsx
```

A instrução `"%s"` junto com o printfn permite a inserção de uma variável no texto, mas vamos aprender estes detalhes
mais pra frente. Por enquanto, podemos ficar tranquilos que nos livramos da maldição, e assim vamos conseguir aprender
F# sem problemas :)

