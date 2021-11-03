### Matématica Básica Em Csharp

Olá hoje nós iremos aprender hoje como nos podemos fazer calculos em Csharp e acredite ou não isso é <Strong>MUITO</Strong> importante por que se você não sabe nem somar dois números quem dira fazer um software, Ahh então quer dizer que todo programa que eu fizer vai ser pura matématica, bem algumas coisas realmente não precisaram de calculos por que a linguagem ja vem com muita coisa pronta para você poder utilizar más bem vamos para a aula que vocês veram na prática

# Somar

- Somar: Para somar dois números em `C#` basta apenas colocar dois numeros entre o sinal de `+` dessa forma

Exemplo com numeros:

```csharp
    void Somar()
    {
        int result = 1 + 1;
        Console.Writeline(result);
    }
```

Exemplo com Variaveis:

```csharp
    void Somar(int num1,int num2)
    {
        int result = num1 + num2;
        Console.WriteLine(result);
    }
```

Agora digamos que você tem uma variavel e você quer somar o que tem dentro dela com outro numero você pode fazer isso de 2 formas:

Forma 1:

```csharp
    void Somar()
    {
        int num = 10;
        num = num + 2;

        Console.WriteLine(num);
    }
```

Forma 2:

```csharp
    void Somar()
    {
        int num = 10;
        num += 2;
        
        Console.WriteLine(num);
    }
```

Se você decidir somar um numero com uma variavel string(texto) você ira concatenar o numero com a string, isso siginifica que você ira juntar os dois

Exemplo Concatenação:

```csharp
    void Somar()
    {
        int result = 1 + 1;
        string message = "o resultado da soma foi " + result;
    }
```

O que ira ser empresso no Console séra isso: <Strong>o resultado da soma foi 2</Strong>



# Subtrair

- Subtração: para você subtrair dois numeros basta você utilizar o sinal de `-` dessa forma:

Exemplo com numeros:

```csharp
    void Diminuir()
    {
        int result = 1 - 1;
        Console.WriteLine(result);
    }
```

Exemplo com variaveis:

```csharp
    void Diminuir(int num1, int num2)
    {
        int result = num1 - num2;
        Console.WriteLine(result);
    }
```

- Caso você queria diminuir o proprio numero da variavel, é so fazer o seguinte:

Forma 1:

```csharp
    void Diminuir(int num1, int num2)
    {
        int result = num1 - num2;
        result -= 1;//<- aqui ele ta pegando o valor que ta dentro da variavel result e diminuindo 1
    }
```

Forma 2:

```csharp
    void Diminuir(int num1, int num2)
    {
        int result = num1 - num2;
        result = result - 1;//<- aqui ele ta pegando o valor que ta dentro da variavel result e diminuindo 1
    }
```

# Multiplicação

- Multiplicação: para você multiplicar é so você colocar o sinal de `*` entre os números

<p>ele funciona igual a subtração e diminuição é o mesmo método blz</p>

# Divisão

- Divisão: para você dividir um numero por outro é so você usar o sinal de `/` entre os números

<p>ele funciona igual a subtração e diminuição é o mesmo método blz</p>

# Resto da divisão

- Para você calcular o resto da divisão basta utilizar o sinal de porcentagem(`%`)

Ahh mas para que eu irei utilizar isso

ahh meu pequeno gafanhoto mas fazer nosso primeiro exemplo pratico, digamos que você quer saber se um número é par ou impar você checara o resto da divisão do numero que você quer checar por 2, ai se ele for zero ele é par se ele for 1 é impar

Exemplo:

```csharp
    void EPar(int numero)
    {
        int restoDaDivisao = numero % 2;

        if(restoDaDivisão == 0)
        {
            Console.WriteLine("é par");
        }else
        {
            Console.WriteLine("é impar");
        }
    }
```

- :warning: olha não se preocupe com esse if e else você ira aprender a como utilizar esses carinhas logo em breve mas, por equanto apenas entenda que um if é uma condição se ela não for atendida ele vai cair no else

[Proximo Conteúdo](/Csharp/Iniciante/Basico/Conteudos/condicoes.md)