### Condições

- Agora você ira aprender a usar condições, você provalvemente ira precisar dela pra fazer diversos programas, então não pula so por que você acha que não vai ser nessésario beleza, até por que ele é

# sinais utilizados em codicionais

|Sinal|O que significa|
| --- | --- |
| == | igual a alguma coisa|
| != | diferente de alguma coisa|
| >= | maior ou igual que um numero|
| <= | menor ou igual que um numero|
| > | maior que um numero|
| < | menor que um numero|

# if , else e else if

- a sigla `if` em C#(Csharp) ela significa que você esta impondo uma condição para que uma ação aconteca, bem vamos pensar o seguinte digamos que você quer checar se um jogador tem uma chave para abrir uma porta você <Strong>Poderia</Strong> fazer assim:

- a sigla `else` em C# ela significa basicamente se não, se uma condição não for atendida ela entrara no else

- a sigla `else if` em c# ela significa que se essa condição 
Exemplo:

```csharp
    void AbrirPorta(bool temChave)
    {
        if(temChave == true)// esta checando se a variavel "temChave" é igual a "true"(verdadeiro)
        {
            Console.WriteLine("Você abriu a porta!!");
        }else//se a variavel "temChave" não for igual a true nesse caso se ela for falsa ela vai executar esse outro boloco de codigo
        {
            Console.WriteLine("Você não tem a chave vassilão");
        }
    }
```