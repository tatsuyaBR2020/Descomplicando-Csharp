## <Strong>Regras da linguagem</Strong>

<p>Em <Strong>Csharp</Srtong> nós temos algumas regras que devem ser seguidas se não nos não poderemos compilar o programa. Mas pó fica tranquilo que são bem, simples então vamos para as regras</p>

## <h1>Ponto e virgula</h1>

<p>nós temos que utilizar o <Strong>;</Strong> ao final de cada instrução nós temos que colocar para indicar que ali é o final da sua instrução como desse jeito:</p>

```csharp
    public class exemplo
    {
        int numero = 10;//<- ponto e virgula ao final
        string texto = "José";//<- ponto e virgula ao final
        float flutuante = 1.25f;//<- ponto e virgula ao final
        List<int> lista = new List<int>();//<- ponto e virgula ao final

        void teste()
        {

        }
    }
```

- :warning: você não deve por ponto e virgula em somente em declaração de função ou declaração de classe o resto você tem que colocar

## <h1>Variaveis</h1>

Para declarar uma variavel você precisara primeiro dizer a `tipagem` dela que nada mais é o tipo dessa variavel, logo em seguida você ira colocar um nome para ela e depois você poderá setar um valor a ela, mas caso não queria atribuir um valor pra ela logo de cara ele ja vem com um valor padrão

Exemplo declaração de variaveis com valores:

```csharp
    public class Exemplo
    {
        string texto = "Ola Mundo!!";
        int numeroInteiro = 2;
        float numeroQuebrado = 1.5f;
    }
```
Exemplo sem valores atribuidos:

```csharp
    public class Exemplo
    {
        string texto;//ele vai iniciar com o valor "" que não vai ter nenhum caractere
        int numeroInteiro;//começa com o valor inicial de zero
        float numeroQubrado;//começa com o valor inicial de zero
    }
```

- :warning: lembrando que você não deve colocar um nome para variavel que seja reservados da linguagem ou colocar assentos e sempre colocar o nome todo junto, você pode "separar" as palavras colocando a primeira letra da palavra maiuscula


## Orientação a objetos

- :warning: calma pequeno gafanhoto nós não iremos nos aprofundar tanto nesse assunto hoje eu vou apenas te dar um "empurraozinho" no assunto

Bem quando você deseja criar uma variavel de alguma classe voce não pode so colocar a variavel la e pronto nos temos que `instanciar` o "objeto" que no caso é uma classe. para fazer isso da forma certa voce deve setar a variavel com um new seguido do nome da classe que você deseja fazer a instancia e depois colocar parênteses dentro dos parenteses nós iremos precisar colocar alguns parâmetros mas somente se o construtor da classe pedir<br>

Exemplos:
```csharp
    public class Exemplo
    {
        public MeuNome t = new MeuNome();
    }
```

```csharp
    public class Exemplo
    {
        MeuNome t;

        void CriarInstancia()
        {
            t = new MeuNome();
        }
    }
```
- :warning: lembrando que se você quer setar a variavel depois em uma função você pode deixala `null` que significa que a variavel está vazia que é so você declarar ela mas não setar nada nela


## Escopo de váriaveis

Escopo de uma variavel é basicamente a acessibilidade dela na classe dela por exemplo:

```csharp
    public class MeuNome
    {
        string nome = "jose";

        void PrintarNome()
        {
            Console.WriteLine(nome);
        }
    }
```
<p>nesse caso a variavel <Strong>nome</Strong> ela é acessivel de qualquer lugar dessa classe nós podemos chamar ela de variavel global, mas se ela for declarada dentro de uma função ela so podera ser acessada de dentro dessa mesma função</p> <br>

- Exemplo:

```csharp
    public class MeuNome
    {
        void SetarNome()
        {
            string nome = "jose";
            PrintarNome();
        }

        void PrintarNome()
        {
            Console.WriteLine(nome);/*<- esse daqui vai dar o seguinte erro variavel não existe no contexto atual que seguinifica que essa variavel não esta em um escopo acessivel*/
        }
    }
```

:warning: Mas caso você queira acessar o valor dessa variavel pode passar ele como parametro ou setar ele dentro de uma variável "global" da classe

- Exemplo 1:
```csharp
    public class MeuNome
    {
        string nome;

        void SetarNome()
        {
            nome = "julia";
            PrintarNome();
        }

        void PrintarNome()
        {
            Console.WriteLine(nome);
        }
    }
```

<p>Nesse primeiro caso eu criei uma variavel global chamada de "nome" so que não setei nada nela, ela tá vazia, ai dentro da função "SetarNome" eu dou um valor para a variavel e logo em seguida eu peço pra ele escrever o que tiver na variavel "nome" no console</p>

- Exemplo 2:

```csharp
    public class MeuNome
    {
        void SetarNome()
        {
            string nome = "josé";
            PrintarNome(nome);
        }

        void PrintarNome(string mensagem)
        {
            Console.WriteLine(mensagem);
        }
    }
```

<p>Nesse caso aqui eu acessei o valor da varivel da função pedindo um parametro para poder executar a função, mas dessa forma a variavel não sera salva depois que a função acabar então pra isso você poderia salvar ele em uma variavel de escopo global como nós fizemos no exemplo 1</p

<h1>Finalizado por enquanto</h1>

[]