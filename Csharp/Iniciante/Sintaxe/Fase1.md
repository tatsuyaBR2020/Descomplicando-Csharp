# Inicio dos estudos na sintaxe do c#

## <h1>Importar <Strong>Bibliotecas</Strong></h1>
para começarmos com o pé direito na liguagem vamos começar falando de como usar as <Strong>Bibliotecas</Strong><br>

Você pode importar uma biblioteca inteira assim:

```csharp
    using NomeDaBiblioteca;
```
- Lembrando dentro de uma biblioteca pode haver outra biblioteca

mas caso você apenas queira acessar somente uma coisa da biblioteca vc pode fazer assim:

```csharp
    class Teste
    {
        //vc coloca a biblioteca que quer acessar e depois coloca um ponto para poder acessar tudo que aquela biblioteca tem 
        System.Collections.Generic.List<int> lista;
    }
```

Você tambem pode fazer isso dentro de funcões dessa forma:

```csharp
    void EscreverNoConsole()
    {
        System.Console.WriteLine("Seja bem vindo :p");
    }
```

## <h1>Como usar os <Strong>namespaces</Strong></h1>

<p>Usar namespaces te ajuda a manter o seu codigo organizado e que obrige que quem queria utilizar algo dentro 
do namespace tenha que importar ele porque um namespace é uma biblioteca
</p>

Para usar o namespaces não tem muito segredo você so precisa colocar a propriedade `namespace` seguido de um nome e chaves dessa forma:

```csharp
    namespace NomeDaBiblioteca
    {
        public class HelloWorld
        {

        }
    }
```

para poder usar o conteudo que ta dentro do namesapce é so importar ele igual a uma biblioteca afinal ele tambem é uma biblioteca

- :warning: Lembrando que se você quer criar um caminho de bibliotecas você pode fazer assim:

```csharp
    namespace NomeDaBiblioteca.OutroNome
    {
        public class OutraClasse
        {

        } 
    }
```

Dessa forma é so vc importar assim:

```csharp
    using NomeDaBiblioteca.OutroNome;
```

- e lembrando que é como se fosse uma pasta por exemplo na pasta <Strong>NomeDaBiblioteca</Strong> vai ter um conteudo ai no outro caminho <Strong>NomeDaBiblioteca.OutroNome</Strong> hávera outros conteúdos

- Párabens por ter dado seu primeiro passo rumo a fluência em Csharp

[Próximo](/Csharp/Sintaxe/Fase2.md)
