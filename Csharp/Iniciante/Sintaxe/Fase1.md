## <h1>Importar e criar <Strong>Bibliotecas</Strong></h1>
para começarmos com o pé direito na liguagem vamos começar falando de como usar as `Bibliotecas`

para importar uma biblioteca você so precisa colocar primeiro a propriedade using e sm seguida colocar o `nome` da biblioteca dessa forma:

```csharp
    using System;
```
- Lembrando dentro de uma biblioteca pode haver outra biblioteca como por exemplo:
```csharp
    using System.Collections.Generic
```
<p>nesse caso eu indiquei o caminho para a biblioteca <Strong>Generic</Strong></p>

mas caso você não queria importar a biblioteca inteira pro seu codigo você pode fazer dessa forma:

```csharp
    class Teste
    {
        //vc coloca a biblioteca que quer acessar e depois coloca um ponto para poder acessar algo daquela biblioteca
        System.Collections.Generic.List<int> lista;
    }
```

Você tambem pode fazer isso dentro de funcões dessa forma:

```csharp
    void EscreverNoConsole()
    {
        System.Console.WriteLine("Que começe a revolução das máquinas!!!");
    }
```

## <h1>Como usar os <Strong>namespaces</Strong></h1>

<p>Usar namespaces te ajuda a manter o seu codigo organizado e que obrige a quem quiser utilizar algo de dentro
do namespace tenha que importar ele porque um namespace é uma biblioteca
</p>

Para usar o namespaces não tem muito segredo você so precisa colocar a propriedade `namespace` seguido de um nome e chaves , dentro das chaves você coloca o seu conteúdo dessa jeito:

```csharp
    namespace ONomeQueVoceEscolher
    {
        public class HelloWorld
        {
            
        }
    }
```

para poder usar o conteudo que ta dentro do namesapce é so importar ele igual a uma biblioteca afinal ele tambem é uma biblioteca quem diria não é mesmo

- :warning: Lembrando que se você quer criar um caminho de bibliotecas você pode fazer assim:

```csharp
    namespace exemplo.OutroNome
    {
        public class OutraClasse
        {

        } 
    }
```
para você criar um caminho de bibliotecas é so você colocar um nome seguido de um . e depois outro nome

- e lembrando que é como se fosse uma pasta por exemplo na pasta <Strong>MinhaBiblioteca</Strong> vai ter um conteudo ja em outro caminho por exemplo <Strong>MinhaBiblioteca.Calculadora</Strong> hávera outros conteúdos e assim por diante

- Párabens por ter dado seu primeiro passo rumo a fluência em Csharp

[Próximo](/Csharp/Sintaxe/Fase2.md)
