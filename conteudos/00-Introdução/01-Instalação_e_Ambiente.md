# Instalação

Para programar em F#, você vai precisar instalar o SDK do .NET.

## Windows / MacOS / Linux

Acesse o [site do SDK](https://dotnet.microsoft.com/pt-br/download), baixe o executável do SDK na última versão e rode. Está instalado :)

Para o Linux, é possível utilizar o gerenciador de pacotes de sua distribuição. O .NET está disponível nas distribuições
mais famosas por padrão.

No Windows, você pode realizar a instalação junto com o Visual Studio, basta apenas instalar qualquer produto .NET.

# Ambiente

## Visual Studio

O Visual Studio já vem com suporte ao F# direto da instalação.

## Visual Studio Code

Para o VSCode, você pode instalar a extensão [Ionide](https://marketplace.visualstudio.com/items?itemName=Ionide.Ionide-fsharp), que dá 
suporte à linguagem, e também o pacote com as outras [extensões do .NET](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.vscode-dotnet-pack).

## Vim / Neovim

Para o Vim ou Neovim, você pode usar o [Ionide-vim](https://github.com/ionide/Ionide-vim), e também em conjunto o 
[neofsharp.vim](https://github.com/adelarsq/neofsharp.vim).

## Notebooks

Caso seja do seu gosto, você pode optar por utilizar Notebooks, tanto dentro do Jupyter, quanto dentro do VSCode.

### Jupyter

Você precisa ter instalado o Python e o Jupyter na sua máquina, além do SDK do .NET (instruções acima).

Após isso, você apenas precisa instalar a ferramenta global .NET Interactive e instalar o kernel do Jupyter. Pra fazer
isso, basta executar os seguintes comandos:

```
dotnet tool install -g Microsoft.dotnet-interactive
dotnet interactive jupyter install
```

Feito isso, basta executar o Jupyter e criar um novo Notebook com a linguagem F#.

### Visual Studio Code - Polyglot Notebooks

Para usar os Notebooks no VSCode, basta instalar a extensão [Polyglot Notebooks](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.dotnet-interactive-vscode),
que também está inclusa no pacote de extensões do .NET.

No VSCode, você pode ter cada célula do Notebook com uma linguagem, podendo misturar C#, F#, PowerShell e outras
linguagens.

