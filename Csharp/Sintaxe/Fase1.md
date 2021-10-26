# Inicio dos estudos na sintaxe do c#

## <h1>Bibliotecas</h1>
para começarmos com o pé direito na liguagem vamos começar falando de como usar as <Strong>bibliotecas</Strong><br>

Você pode importar uma biblioteca inteira assim:

```csharp
    using NomeDaBiblioteca;
```
-Lembrando dentro de uma biblioteca pode haver outra biblioteca

mas caso você apenas queira acessar somente uma coisa da biblioteca vc pode fazer assim:

```csharp
    class Teste
    {
        //vc coloca a biblioteca que quer acessar e depois coloca um ponto para poder acessar tudo que aquela biblioteca tem 
        System.Collections.Generic.List<int> lista;
    }
```
- Lembrando que uma biblioteca pode conter outra biblioteca dentro dela OK

Você tambem pode fazer isso dentro de funcões dessa forma:

```csharp
    void EscreverNoConsole()
    {
        System.Console.WriteLine("Seja bem vindo :p");
    }
```