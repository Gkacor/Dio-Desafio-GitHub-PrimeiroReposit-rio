# Introdução Python

Created: January 7, 2022 7:26 PM
Data Inicial: 07/01/2022
Programação: Programação
Reviewed: No

# Python

Sempre cuidar com a identação. Pontuação, fechar parênteses abertos e etc.

Primeiro olá mundo:

```python
print('Olá Mundo')
Olá Mundo
```

Dados -  o que está na memória e conseguimos manipular.

Dado é o nome que damos a uma região da memória que podemos “chamar”.

```
nota = 8.5
```

Sinal de “=” significa atribuição.

```python
nota = 8.5
disciplina = 'Lógica de Programação'

print(nota)
print(disciplina)

8.5
Lógica de Programação
```

Não é possível começar variável com número.

Python é a única linguagem que aceita acentuação, mas não é recomendado.

tipos de dados:

- numérico(números inteiros - “int” e com vírgula - “float”)
- caractere(strings, textual)
- literal/booleana(true or false)

Fazer comparação de igualdade: Utiliza-se o “==”, pois somente um sinal de igual vira atribuição.

Como acessar o índice:

```python
Olá Mundo

print(frase[0])
O
print(frase[2])
á
```

Parecido com vetor, podemos acessar cada letra, pois ficam armazenadas no sistema por códigos em 8 bit.

Concatenação: Juntar.

### Composição

Utilizar o %f para trocar ou substituir pela variável que eu quero que apareça.

ex:

```python
nota = 8.5
s1 = 'Você tirou %f na prova' % nota
print(s1)
Você tirou 8.500000 na prova.

//para limitar casas decimais:

nota = 8.5
s1 = 'Você tirou %.2f na prova' % nota  
print(s1)
Você tirou 8.5 na prova.

//o ".2" limita a quantidade de casas que vão aparecer.

//várias variáveis:
nota = 8.5
disciplina = 'Algoritmos'
s1 = 'Você tirou %.2f na prova de %s' % (nota, disciplina)  
print(s1)
Você tirou 8.5 na prova de Algoritmos.
```

![Untitled](Introduc%CC%A7a%CC%83o%20Python%209aa49364738d430499da093176fd06e1/Untitled.png)

```python
Composição mais moderna:

nota = 8.5
disciplina = 'Algoritmos'
s1 = 'Você tirou {} na prova de {}' .format(nota, disciplina)  
print(s1)
Você tirou 8.5 na prova de Algoritmos.
```

Fatiar uma String:

```python
s1 = 'Lógica de programação'
print(s1[0:6]) //quais eu quero dar print. também pode só utilizar :6.
Lógica

```

Tamanho:

```python
s1 = 'Lógica de programação'
tamanho = len(s1)
print(tamanho)
34
```

### Condição

Em pseudocódigo:

```python
se(condição)   if(condição):
```

```python
##instruções
```

```python
fim-se           
```

Condicionamento simples.

```python
se(condição)      if(condição):

#Instruções A

senão                  else:

#instruçõesB

fim-se
```

Condicionamento composto.

### Booleana

operadores:

- not - negação
- and - conjunção
- or - disjunção

Not

Nega um resultado booleano. Na prática, o valor seria invertido..

And

O valor será verdadeiro somente se todas as entradas forem verdadeiras. True and True.

Or

O valor será verdadeiro se pelo menor uma entrada for verdadeira. True or false.

---

Procedência dos operadores: 

1. Parênteses
2. Multiplicação
3. Divisão
4. Adição/subtração
5. Operadores relacionais: ==, !=, <>
6. Operadores lógicos ‘not’
7. Operadores lógicos ‘and’
8. Operadores lógicos ‘or’
9. Atribuições

Na programação, temos uma sequência condicional depois deles também.

---

### Condicionais Aninhadas

As operações condicionais podem ser adicionadaas uma dentro das outras, infinitamente.

ex:

```python
if(x > y):
#instrução
else if:
#instrução
else if:
#instrução
```

### ELIF

Pode ser utilizado no lugar do ‘else if’.

```python
if(x > y):
#instrução
elif
#instrução
```

### While(Repetição, Loop)

while(x > y):

Exemplo:

```python
x = 1
while(x <= 5):
print(x)
x = x + 1 ## importante colocar, senão vira um loop infinito.
```

“Break” serve para parar o loop. Sair.

exemplos utilizando todos os conceitos até agora:

```python
print('Digite uma mensagem que irá se repetir.')
print('Para encessar escreva "sair"')
while True:
texto = input('')
print(texto)
if texto == 'sair':
break
print('Encerrando o programa')
```

“Continue” serve para continuar o comando.

ex:

```python
while True:
	 nome = input('Qual o seu nome?')
if (nome != 'login')
 continue
senha = input('Qual a senha?')
```

### Truthy and Falsey

Dados não booleanos podem ser tratados como True ou False em uma condição.

Falsey: número zero(int ou float) e string vazia.

Truthy: qualquer outro dado.

### For

Recomendado para quando sabemos a quantidade de repetição que queremos.

ex:

```python
for x in range(10)
print(x)

#for (variável) na range(quantidade de vezes)

se fosse definir a range de forma mais específica:

for x in range(1,6,2)
#for (variável) na range(de 1 a 6, a cada 2)
```

### Funções

Também chamado de rotinas de código.

print, input, range são funções pré programadas.

Funções facilitam arrumar os bugs.

Em um código compartilhado, tem várias pessoas trabalhando em diferentes funções.

Como criamos uma função:

```python
def(palavra chave)realce(nome da função)():

def realce():
#corpo da função
   print('|','_'* 10,'|')
   print('|','_'* 10,'|')

#Agora a função foi criada. Pode ser chamada no programa principal.

#Chamando no prog. principal:
realce()
print('      MENU')
realce()

#Dentro da função também pode ser colocado uma variável
ex:

def realce(x, y):
    res = x - y
    print(res)

#Programa Principal

realce(5, 7)
#Quando rodar, apareceria -2, ou qual for o resultado.
#Os dados são atribuídos na ordem, ou seja, 5 é x e 7 é y.

```

Variável local: Funciona apenas naquela função.

- criado sempre que uma função é “chamada”.
- não consigo acessar em outra função, nem mesmo global.

Variável gloval: Funciona em todo o programa(main).

- criado quando o programa principal é criado.
- existe em todas as funções do programa.

exemplos:

```python
def comida()
  print(ovos)

#programa principal(identação a direita)
ovos = 12
comida()
```

Como retornar o “resultado” de uma função?

Utilizando o “return”

ex:

```python
#exercício pra confirmar se a string é entre 10 e 30 caracteres.
def valida_string(pergunta, min, max)
   s1 = input(pergunta)
   tam = len(s1)
   while ((tam < min) or (tam > max)):
     s1 = input(pergunta)
     tam = len(s1)
   return s1

#programa principal
x = valida_string('Digite uma string', 10, 30)
print('Você digitou a string {}. \n dado válido. Encerrando... .format(x))

```

### Erros

mais comuns:

- ZeroDivisionError: erro de divisão por zero.
- ValueError: dado não esperado foi digitado.
- IndexError: índice inexistente sendo acessado.

como tratar esses erros no código:

```python
while True:
 try:
  x = int(input('Digite um número'))
  break
 except ValueError:
  print('Valor errado. Digite outro.')
#ou seja, se ele pede um número inteiro e eu digito outra coisa,
#ao invés de dar o erro, ele pergunta novamente.
  
```

### Estruturas de Dados

- Tuplas: () - Estática(não será alterado na memória), imutável (dado não será alterado depois de alocado)

ex: 

```python
mochila = ('Machado', 'Camisa', 'Comida')
print(mochila) #mostra todos os dados.

print(mochila[0])
print(mochila[2])
#Mostra os dados selecionados.

for item in mochila:
   print('Na minha mochila tem: {}'.format(item))
#Mostraria dessa forma:
Na minha mochila tem: Machado
Na minha mochila tem: Camisa
#etc

tam = len(mochila)
for i in range(0, tam, 1):
   print('Na minha mochila tem: {}'.format(mochila[i]))
#Mesmo resultado de acima.

mochila = ('Machado', 'Camisa', 'Comida')
upgrade = ('Queijo', 'Faca')
mochila_grande = mochila + upgrade
print(mochila_grande)
#Adicionando itens
```

### Desempacotamento de parâmetros em funções

```python
def soma(*num): #*num será uma tupla, que será manipulada na função.
   soma = 0
   print('Tupla: {}'.format(num))
   for i in num:
      soma += i
   return soma

print('Resultado: {}\n'.format(soma(1,2)))
#Ou seja, transforma os dados em um "pacote" para manipular.
```

- Listas: [] - Estrutura de dados dinâmica. Dados podem ser alterados. Indexadas por valores numéricos inteiros.

ex:

```python
mochila = ['Machado', 'Camisa', 'Comida']

mochila[2] = 'Laranja'
print(mochila)
 ['Machado', 'Camisa', 'Laranja'] #Trocou o 2(comida) pela laranja.
```

Manipulando:

```python
mochila.append('Dinheiro') #adiciona para o fim da lista mochila. 
print(mochila)
 ['Machado', 'Camisa', 'Laranja', 'Dinheiro']

mochila.insert(1, 'Bola') #adiciona para um lugar específico da lista, no caso, o 1.
print(mochila)
 ['Machado', 'Bola', 'Camisa', 'Laranja', 'Dinheiro'] #lembrando que a contagem começa do 0.

del mochila[0]#para apagar usando o lugar na lista.
print(mochila)
 ['Bola', 'Camisa', 'Laranja', 'Dinheiro']

mochila.remove('Camisa') #deleta direto pela string.
print(mochila)
 ['Bola','Laranja', 'Dinheiro']

#Criar cópia de uma lista para manipular somente ela:
mochila = ['Machado', 'Camisa', 'Comida']
mochila2 = mochila[:] #cria uma cópia da lista indepedente da original.
```

indexação dupla:

```python
mochila = ['Machado', 'Camisa', 'Comida']
print(mochila[0][2])#selecionando uma letra em uma string.
#vai aparecer:
c 
```

- Dicionários: {} - Estrutura de dados dinâmica. Podem ser alterados dados e tamanho. Indexados por palavras.(podem ser utilizados paravras como índice, ao invés de números.

ex:

```python
game = {'nome': 'Mario', 'desenvolvedora' : 'nintendo'}
#a "chave" ou índice é o que está antes dos dois pontos.

#para chamar:

print(game['nome'])
Mario
```

Métodos próprios:

values: obtém somente os dados

keys: obtém somente as chaves

items: obtém chave:dado

ex:

```python
print(game.values)
dict_values(['Mario', 'nintendo'])

for x in game.values():
print(x)
Mario
nintendo
```

Variáveis simples: Armazenam somente um dado.

Variáveis compostas: Armazenam um conjunto de dados.