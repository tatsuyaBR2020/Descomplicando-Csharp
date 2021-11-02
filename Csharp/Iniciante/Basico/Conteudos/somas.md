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

    }
```