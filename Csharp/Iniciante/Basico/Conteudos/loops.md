#### Loops em C#

- Ola nessa aula nós iremos descobrir os tipos de loops possivéis na linguagem <Strong>C#</Strong>

## Tipos de loops

- Em C# nós temos 3 tipos de loops póssiveis entre eles nós temos `for`, `foreach` e `while`. para cada um desses tipos vão ter certas ocaciões que um vai se sair melhor então é bom você ter o conhecimento de cada um desses 3 beleza.

- :warning: lembrando que vocês devem ter cuidado ao usarem loops por quê se a condição que vocês colocarem nunca for atendida o seu codigo ira ficar travado pra sempre até você fechar o programa, e o C# so ira continuar lembro as proximas linhas so depois que o loop seja terminado

# For

- o for é mais utilizados quando nós temos que repetir uma tarefa um tanto de vezes ou percorrer uma lista, digamos que você quer fazer um loop 10 vezes o melhor caso seria utilizar o for que a sintaxe é bem simples de se aplicar

- <Strong>Sintaxe</Strong>

```csharp
    for(int i = 0; i < 10; i++)
    {
        //o codigo que você quer repetir aqui....
    }
```

<p>
    basicamente para você declarar um for é so usar a sigla <Strong>For</Strong> seguida de pârenteses dentro dos parenteses nós iremos precisar fazer umas coisas primeiro você vai declarar uma variavel de tipo númerico e poe um ponto e virgula depois você ira colocar a condição para que o loop esteja acontecendo, por ultimo você ira precisar colocar a forma que o loop vai ser encerrado
</p>

:warning: Se você colocar uma condição que nunca vai ser atendida o loop vai ser eterno

exemplo:

```csharp
    for(int i = 0; i < 10; i--)
        {
            //o codigo que você quer repetir aqui....
        }
```

<p>nesse caso a condição é que a variavel local i seja menor que 10 mas o ultimo argumento do for esta subtraindo i ao invés de somar ele sou seja, i sempre séra menor que 10</p>

# Foreach

- o foreach so tem uma função que é percorrer uma lista

- <Strong>Sintaxe</Strong>

```csharp
    public class Exemplo
    {
        private string[] nomes;

        void PrintarTodosOsNomes()
        {
            foreach(string nome in nomes)
            {
                Console.WriteLine(nome);
            }
        }
    }
```

<p>Para declarar um <Strong>foreach</Strong> basta utilizar a sigla foreach seguido de parenteses, dentro dos parenteses você ira declarar a variavel que vai conter o valor do item da lista que o foreach esta assesando, em seguida nos iremos utilizar a sigla <Strong>in</Strong> para indicar a lista que nós desejamos percorrer e por ultimo colocamos a lista a ser percorrida</p>

# While

- O while é utilizado quando nós queremos que enquanto uma condição esteja sendo atendida ele ira ficar executando o bloco de código

<p>:warning: Um bloco de código nada miasé tudo que está entre chaves!!</p>

- Exemplo:
```csharp
    bool jaCagouHoje = false;

    while(jaCagouHoje == false)//enquanto a variavel seja falso ele vai ficar executando o bloco de códiigo
    {
        Console.WriteLine("Digite `cagar` para fazer você sabe");

        if(Console.ReadLine() == "cagar" || Console.ReadLine() == "Cagar")
        {
            jaCagouHoje = true;
        }
    }

    Console.Writeline("Você ja cagou hoje, ai sim fera :P");
```

<p>Nesse caso eu criei uma variavel bool ou booleana como você quiser chamar, e fiz uma condição que enquanto a variavel jaCagouHoje seja false(Falsa) ele vai ficar repetindo o bloco de codigo até que o usuario digite no console "cagar" para assim nós podermos mudar o valor da variavel para true(verdadeira) e assim fazendo a condição do loop não ser mais atendida e fazendo com que ele saia do loop</p>

[Aula Classes](/Csharp/Iniciante/Basico/Conteudos/classes.md)