### Exercicio 01

- Bem como esse séra seu primeiro programa em C# vamos fazer algo bem simples e aqui você ira aprender mais aprofundado de como usar condições e variaveis então vamos lá

Pois bem vamos começar fazendo uma calculadora simples, uma coisa que é muito importante antes mesmo de você começar a escrever um codigo é você imaginar na sua cabeça os passos que você tem que seguir bom vamos pensar da seguinte forma primiero eu tenho que pedir para o úsuario que estiver usando a aplicação digite dois numeros e a operação que ele quer executar, so depois que tiver esse valores você faz os calculos e devolvo o resultado em uma mensagem para o úsuario.

- Bem vamos começar com o primiero passo, que é pedir para o úsuario digitar os dois números e a operação que ele deseja quer fazer

```csharp
    using System;

    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Digite um número");// <-- aqui você pede para o seu programa "imprimir" no console uma messagem
            string num1 = Console.ReadLine();// aqui você esta lendo o que o usuario digitou no console
            Console.WriteLine("Digite outro número");// <-- aqui você pede para o seu programa "imprimir" no console uma messagem
            string num2 = Console.ReadLine();// aqui você esta lendo o que o usuario digitou no console

            Console.WriteLine("qual o operador da conta? \n +, -, * ou /");// <-- aqui nesse caso nos usamos o \n para ele quebrar para a próxima lina e não ficar tudo em uma so linha
            string operadorDaConta = Console.WriteLine();// lemos o que ele escreveu no console
        }
    }
```

- Pronto conseguimos as informações que precisamos para podermos fazer os calculos mas agora nós temos um pequeno problema, o problema é o seguinte o comando `Console.ReadLine()` ele retorna uma `string` que é texto ou seja você não pode fazer operações matématicas com texto você tem que converter esses valores para números em C# nos utilizamos a classe `Convert` que esta dentro da biblioteca `System` nós podemos converter em vários tipos númericos mas os mais utilizaods são int, float e double nesse caso aqui nos vamos utilizar o tipo float

```csharp
    using System;

    class Program
    {
        static void Main(string[] args)
        {
            //---------------------------------PARTE 1-----------------------------------------------
            Console.WriteLine("Digite um número");// <-- aqui você pede para o seu programa "imprimir" no console uma messagem
            string num1 = Console.ReadLine();// aqui você esta lendo o que o usuario digitou no console
            Console.WriteLine("Digite outro número");// <-- aqui você pede para o seu programa "imprimir" no console uma messagem
            string num2 = Console.ReadLine();// aqui você esta lendo o que o usuario digitou no console

            Console.WriteLine("qual o operador da conta? \n +, -, * ou /");// <-- aqui nesse caso nos usamos o \n para ele quebrar para a próxima lina e não ficar tudo em uma so linha
            string operadorDaConta = Console.WriteLine();// lemos o que ele escreveu no console

            //---------------------------------PARTE 2-----------------------------------------------

            float numero1 = Convert.ToSingle(num1);// aqui nós convertemos a primiera string e guardamos o retorno da função na variavel local "numero1" agora é so fazer isso com a outra string

            float numero2 = Convert.ToSingle(num2);
        }
    }
```

- Bem depois de converter as strings(Textos) para némeros agora nós vamos para a etapa final da nossa programagem aqui qué é checar qual operador ele escolheu para a conta e fazer ela realmente

```csharp
    using System;

    class Program
    {
        static void Main(string[] args)
        {
            //---------------------------------PARTE 1-----------------------------------------------
            Console.WriteLine("Digite um número");// <-- aqui você pede para o seu programa "imprimir" no console uma messagem
            string num1 = Console.ReadLine();// aqui você esta lendo o que o usuario digitou no console
            Console.WriteLine("Digite outro número");// <-- aqui você pede para o seu programa "imprimir" no console uma messagem
            string num2 = Console.ReadLine();// aqui você esta lendo o que o usuario digitou no console

            Console.WriteLine("qual o operador da conta? \n +, -, * ou /");// <-- aqui nesse caso nos usamos o \n para ele quebrar para a próxima lina e não ficar tudo em uma so linha
            string operadorDaConta = Console.WriteLine();// lemos o que ele escreveu no console

            //---------------------------------PARTE 2-----------------------------------------------

            float numero1 = Convert.ToSingle(num1);// aqui nós convertemos o primiero numero e guardamos o retorno da função na variavel "numero1" agora é so fazer isso com o outro número

            float numero2 = Convert.ToSingle(num2);

            //---------------------------------PARTE 3-------------------------------------------------

            if(operadorDaConta == "+")
            {
                float result = numero1 + numero2;// aqui nós estamos somando
                Console.WriteLine("O resultado da conta foi: " + result);
            }else if(operadorDaConta == "-")
            {
                float result = numero1 - numero2;// aqui nós estamos subtraindo
                Console.WriteLine("O resultado da conta foi: " + result);
            }else if(operadorDaConta == "*")
            {
                float result = numero1 * numero2;// aqui nos estamos multiplicando
                Console.WriteLine("O resultado da conta foi: " + result);
            }else if(operadorDaConta == "*")
            {
                float result = numero1 / numero2;// aqui nos estamos dividindo
                Console.WriteLine("O resultado da conta foi: " + result);
            }else
            {
                Console.WriteLine("Desculpe senhor mas o operador que você inseriu é invalido ;-;");
            }

            Console.ReadKey(true); // aqui nos pedimos que o usuario aperte qualquer tecla para fechar a aplicação
        }
    }
```