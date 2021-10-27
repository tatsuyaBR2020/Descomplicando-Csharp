## <h1>Como um programa em Csharp é construido</h1>

Bem basicamente em um projeto Csharp nos teremos um arquivo Chamado <Strong>Program.cs</Strong><br>
que séra por onde o seu programa séra inicializado

- dentro dele vc tera o seguinte conteudo:

```csharp
    using System;

    namespace NomeDoProjeto
    {
        class Program
        {
            static void Main(string[] args)
            {
                Console.WriteLine("Hello World!");
            }
        }
    }
```

- :warning: Lembrando que esse é o padrão de projeto de console

Bem vamos começar com o básico na parte superior nos temos as nossas bibliotecas
logo em seguinda nos temos a classe <Strong>Program</Strong> elá sera a classe que precisamos para o programa iniciar e dentro dessa classe nós teremos que ter uma void estática chamada Main e vc pode deixar o que ta entre parenteses em branco ou colocar como parametro um <Strong>string[] args</Strong>

agora dentro dessa void irá acontecer a "Mágica", que nada mais é onde nosso codigo será executado

[3 Fase](/Csharp/Iniciante/Sintaxe/Fase3.md)
