# C#

Created: December 17, 2021 2:46 AM
Data Inicial: 17/12/2021
Programação: Programação
Reviewed: No

C#

Principais variáveis:

![Untitled](C#%20e635accfb5644562b9c3bb5d7dd62ea4/Untitled.png)

Variáveis de referência

É possível que duas variáveis façam referência a um mesmo objeto.

![Untitled](C#%20e635accfb5644562b9c3bb5d7dd62ea4/Untitled%201.png)

Instruções(comandos entre chaves):

- variáveis e constantes locais
- if - condicional
- switch - condicional
- while - repetição
- do - repetição
- for - repetição
- foreach - repetição
- break
- continue
- return
- throw - exceptions
- try .. catch .. finally - exceptions
- using

Exemplos:

int para dar uma variável. - pode ser mudada.

const int para uma constante. - qual o uso? garantir que uma variável não será mudada ao longo do código.

### Array

o que é?

Um estrutura de dados que contém um número X de elementos, todos do mesmo tipo, que são acessados através de índices.

São tipos de referência. os índices de um elemento de array variam de 0 a comprimento do array -1.

Exemplo: 

```csharp
int[] a = new int[10] -- array de 10 posições.
for (int i = 0; i < a.lenght; i++) 
{
 a[i] = i * i; --enquanto "i" for menor que o tamanho, vai preencher o "a" com i vezes i.
}
for (int i = 0; i < a.lenght; i++) 
{
  Console.WriteLine($"a[{i}] = {a[i]}"); --pede para escrever que o "a" de tal posição, tem valor tal.
}
```

### Classes e Objetos

São os tipos mais fundamentais de C#. 

Uma classe combina estados(campos, propriedades) e ações(métodos, o que pode executar). Estrutura que eu quero. Ela gera um objeto em memória. Aceita herança, referenciar.

Objetos são instâncias de uma classe. Especializa a classe.

### Membros

Podem ser estáticos(pertencem a classe) ou parte de uma instância(pertencem ao objeto). 

Podem ser(acessibilidade):

- public
- protected
- internal
- private

### Structs

São do tipo valor.

Podem conter membros de dados e membros de ação.

Não requer alocação de referência na memória. Ela por si só já tem os dados.

Não aceita herança. 

Faz menos alocação de memória.

 

### Interfaces

Podem empregar herança multipla.

### Enums

Enumerações.

Possui um conjunto de constantes nomeadas.