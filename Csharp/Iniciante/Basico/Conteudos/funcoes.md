## Funções

<p>Uma função é basicamente um bloco de codigo que pode ser chamado a qualquer momento, isso ajuda a manter o codigo organizado e poupar tempo já que vcocê não tera que reescrever aquele codigo</p>

## Declarar função
Para declarar uma função você tem que primiero dizer o tipo seguido de um nome depois do nome você irá abrir e fechar parenteses dentro deles nos iremos colocar o que na programação nós chamamos de `parametros` se você não quiser pedir nenhum parametro é so deixar em branco depois disso tudo você vai abrir e fechar chaves({} <= dessa forma)

- Exemplo sem parametros:
```csharp
    void EscreverNoConsole()
    {
        Console.WriteLine("Eu sou inévital :p");
    }
```

- Exemplo com parametros:
```csharp
    void EscreverNoConsole(string mensagem, int _idade, float _dinheiroNaCarteira)
    {
        idade = _idade;
        dinheiroAtual = _dinheiroNaCarteira;

        Console.WriteLine(mensagem);
    }
```

- :warning: Uma função pode ser declarada dentro de outra função mas essa função sera apenas local e so podera ser chamada dentro daquela mesma função que ela foi declarada por que o escopo dela não é global 

# Executar funções

<p>Para executar uma função você precisa apenas colocar o nome da função que você quer executar seguido de parenteses</p>

- :warning: para você conseguir executar uma função você tem que estar dentro de uma classe e de uma função dessa classe

- Jeito certo:

```csharp
    public class Idade
    {
        int idade;
        string nome;

        void PedirIdade()
        {
            nome = "Felicia";
            idade = 15;
            EscreverIdade();
        }

        void EscreverIdade()
        {
            Console.WriteLine("Olá " + nome + " você tem " + idade + " anos");
        }
    }
```

- Jeitos errados:
01:<br>
```csharp
    EscreverIdade();//<- ele vai dar erro por que você esta tentando executar uma função fora de uma classe

    public class Idade
    {
        int idade;
        string nome;

        void PedirIdade()
        {
            nome = "Felicia";
            idade = 15;
        }

        void EscreverIdade()
        {
            Console.WriteLine("Olá " + nome + " você tem " + idade + " anos");
        }
    }
```

02:<br>

```csharp
    public class Idade
    {
        int idade;
        string nome;

        EscreverIdade();//<- ele vai dar erro por que você esta tentando executar uma função fora de uma função

        void PedirIdade()
        {
            nome = "Felicia";
            idade = 15;
        }

        void EscreverIdade()
        {
            Console.WriteLine("Olá " + nome + " você tem " + idade + " anos");
        }
    }
```

## Funções com retorno

Uma função com retorno é basicamente uma função que vai te dar um valor depois de ser executada assim você podendo guarda esse "retorno" dentro de alguma variavel

exemplo:

```csharp
    public class MeuNome
    {
        void PrintarMensagem()
        {
            string mensagem = Mensagem();

            Console.WriteLine(mensagem);
        }

        string Mensagem()
        {
            return "o adm chegou gario kk";
        }
    }
```

- Como declarar uma função de retorno?
<p>Para declarar uma função com retorno é o mesmo esquema de declarar uma função normal é so não colocar o tipo como <Strong>void</Strong> (tipo que não tem retorno ele apenas executa o bloco de código)</p>

Exemplo:

```csharp
    public class EscreverNome
    {
        void PegarNome()
        {
            string nome = MeuNome();

            Console.WriteLine(nome);
        }

        string MeuNome()//<- Função de retorno 
        {
            return "josé";
        }
    }
```

<p>Para guardar o valor do retorno da função é so você setar ela a uma variavel como nos fizemos no exemplo a acima</p>

[Proximo](/Csharp/Iniciante/Basico/Conteudos/loops.md)