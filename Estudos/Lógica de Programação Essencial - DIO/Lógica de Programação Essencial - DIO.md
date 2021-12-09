# Lógica de Programação Essencial - DIO

Created: December 2, 2021 2:04 AM
Data Inicial: 02/12/2021 2:08
Programação: Lógica de Prog
Reviewed: No

# Lógica de Programação

---

- Fundamentos
    - Entender que é ESSENCIAL compreender que a lógica é mais importante do que entender a codear.
    - Abstração. Achar o melhor método para resolver o problema após criar o mapa mental inicial.

## Algoritmos

O que é? 

Uma sequência de passos que resolve um problema.

Exemplo: 

```jsx
Início-dia
  Acordei
  Levantei
  Troquei de Roupa
  Fui a padaria
  Dormi novamente
Fim-dia
```

<aside>
💡 Qualquer programa é uma sequência de passos.

</aside>

Joguinho para entender a ideia: 

[Check out what I made](https://studio.code.org/s/mc/lessons/1/levels/4)

## Pseudocódigo

O que é?

Uma forma genéria de escrever um algoritmo, de forma a entender por qualquer pessoa.

[Wolf, Sheep And Cabbage Game](https://www.proprofsgames.com/wolf-sheep-and-cabbage/)

Exemplo.

### Fluxograma

O que é? 

Representação gráfica de um algoritmo. 

![Exemplo de fluxograma.](Lo%CC%81gica%20de%20Programac%CC%A7a%CC%83o%20Essencial%20-%20DIO%20a10b7c7547f84d0092550841769dd8b1/Untitled.png)

Exemplo de fluxograma.

### Variáveis

O que é?

Um objeto (uma posição, frequentemente localizada na memória) capaz de reter e representar um valor ou uma expressão. É escrito sem espaço e sempre começa com uma letra, nunca com um número. Apenas alguns programas aceitam acento.

Exemplos: 

```jsx
aluno = "José da Silva" -- Texto, expressão.
ou
aluno1 = 7 -- Valor declarado na variável aluno1. Comum ser mudado ao longo do código.
```

<aside>
💡 Tipos de variáveis: numérico, caractere, alfanumérico(nome, por exemplo) ou lógico(true or false).

</aside>

<aside>
💡 Tipos de dados: números inteiros(sem decimais), numeros reais(números com decimais), caracteres(tanto letra quanto números) e lógico(true or false).

</aside>

### Constantes

O que é? 

São valores imutáveis durante o código, e não podem ser alterados durante o programa.

```jsx
inicio
declara pi=3,14  --constante
declara raio: número --variável
fim
```

Exemplo de lógica no Flowgorithm:

![Untitled](Lo%CC%81gica%20de%20Programac%CC%A7a%CC%83o%20Essencial%20-%20DIO%20a10b7c7547f84d0092550841769dd8b1/Untitled%201.png)

### Expressões aritméticas

O que é?

Expressões que usam operadores aritméticos e funções aritméticas envolvendo constantes e variáveis.

Exemplo: 

```jsx
50+50 --o programa retorna o valor 100.
ou
total+50 --digamos que o valor total seja 100, o programa retorna o valor 150.
```

Operadores aritméticos:

![Os mais utilizados.](Lo%CC%81gica%20de%20Programac%CC%A7a%CC%83o%20Essencial%20-%20DIO%20a10b7c7547f84d0092550841769dd8b1/Untitled%202.png)

Os mais utilizados.

Expressões Literais:

o que é?

Expressões com constantes e/ou variáveis que tem como resultado valores literais.

Exemplo:

```jsx
nome="José da Silva" ---dando um valor.
nome<-"José da Silva" ---pode ser encontrado em pseudocódigo.
media=(nota1+nota2+nota3+nota4)/4 ---atribuindo valor.
```

Sempre que for atribuir valor a uma variável, utiliza-se o operador =.

Sempre que for dar uma valor para uma variável, tenho que utilizar "".

![Exemplos.](Lo%CC%81gica%20de%20Programac%CC%A7a%CC%83o%20Essencial%20-%20DIO%20a10b7c7547f84d0092550841769dd8b1/Untitled%203.png)

Exemplos.

Expressões Relacionais

O que é?

Expressões compostas por outras expressões ou variáveis numéricas com operadores relacionais. Essas expressões retornam valores lógicos(true or false).

![Outros operadores.](Lo%CC%81gica%20de%20Programac%CC%A7a%CC%83o%20Essencial%20-%20DIO%20a10b7c7547f84d0092550841769dd8b1/Untitled%204.png)

Outros operadores.

Não confundir com atribuição de valores utilizando apenas um sinal de igual(=). Quando igualdade(valor tal é igual a valor tal? resposta: true or false) sempre utiliza-se dois sinais de igual(==). 

![Exemplo. O primeiro é false e o segundo é true.](Lo%CC%81gica%20de%20Programac%CC%A7a%CC%83o%20Essencial%20-%20DIO%20a10b7c7547f84d0092550841769dd8b1/Untitled%205.png)

Exemplo. O primeiro é false e o segundo é true.

### Tomadas de Decisão

O que é?

Enquando criando programas, ocorre a necessidade de decidir o que fazer dependendo da condição encontrada na execução.

Exemplo: Minha loja só aceita cartão de crédito e o cliente só pode pagar de outra forma. Tenho que enviá-lo para outra local ou adaptar o programa.

![Exemplo.](Lo%CC%81gica%20de%20Programac%CC%A7a%CC%83o%20Essencial%20-%20DIO%20a10b7c7547f84d0092550841769dd8b1/Untitled%206.png)

Exemplo.

### Concatenação

O que é?

Termo utilizado para designar a operação de unir o conteúdo de duas strings(uma sequência de caracteres).

Exemplo: duas strings nome e sobrenome, posso exibir as duas junto.

<aside>
💡 Dependendo da linguagem de programação, pode ser utilizado o operador &, . ou +.

</aside>

![Augumentação do exemplo anterior utilizando concatenação e exibindo informações para o usuário.](Lo%CC%81gica%20de%20Programac%CC%A7a%CC%83o%20Essencial%20-%20DIO%20a10b7c7547f84d0092550841769dd8b1/Untitled%207.png)

Augumentação do exemplo anterior utilizando concatenação e exibindo informações para o usuário.

### Estrutura de Repetição

O que é?

Um estrutura que pode repetir mais de uma vez um comando dependendo da condição expressada.

Exemplo: Imprimir mais de um relatório.

![Exemplo.](Lo%CC%81gica%20de%20Programac%CC%A7a%CC%83o%20Essencial%20-%20DIO%20a10b7c7547f84d0092550841769dd8b1/Untitled%208.png)

Exemplo.

Tabuada do 9, exemplo:

![Um das formas, simples.](Lo%CC%81gica%20de%20Programac%CC%A7a%CC%83o%20Essencial%20-%20DIO%20a10b7c7547f84d0092550841769dd8b1/Untitled%209.png)

Um das formas, simples.

![Outro exemplo, utilizando strings.](Lo%CC%81gica%20de%20Programac%CC%A7a%CC%83o%20Essencial%20-%20DIO%20a10b7c7547f84d0092550841769dd8b1/Untitled%2010.png)

Outro exemplo, utilizando strings.

 

### Linguagens de Programação

O que é?

Linguagem que utilizamos para "conversar" com a máquina.

Existem dois tipos:

Alto nível: Linguagem mais próxima da humana, da nossa linguagem.

Baixo nível: Mais aproximada da linguagem da máquina. Precisa ter conhecimento direto da arquitetura/hardware do computador para utilizar.

Compiladas: Utiliza compilador(.exe), é traduzida para o sistema operacional utilizar.

Interpretadas: O código fonte é executado por um programa chamado de interpretador, que em seguida é executado pelo sistema operacional.

### Portugol

O que é?

Uma pseudolinguagem que permite ao leitor desenvolver algoritmos estruturados em português de forma simples e intuitiva, independetemente de linguagem de programação.

```jsx
programa
{
	
	funcao inicio()
	{
		real janeiro, fevereiro, marco, abril, total, media
		cadeia vendedor

		escreva("Digite o nome do vendedor:")
		leia(vendedor)
		escreva("O seu nome é: " + vendedor)
		
		escreva(" Digite o valor da venda de janeiro: ")
		leia(janeiro)
		escreva("Digite o valor da venda de fevereiro: ")
		leia(fevereiro)
		escreva("Digite o valor da venda de março: ")
		leia(marco)
		escreva("Digite o valor da venda de abril: ")
		leia(abril)

		total = (janeiro+fevereiro+marco+abril)
		media = (janeiro+fevereiro+marco+abril)/4
		escreva("A total das vendas do vendedor " + vendedor + " é: " + total + " e a média das vendas é: " + media)
	}
}
```

### Desvio condicional "se"

O que é?

Palavra reservada(utilizada para uma função específica no código) se, testa e executa as instruções entre as chaves se o desvio for verdadeiro(true).

exemplo:

```jsx
se(media>=7){
				escreva("Parabéns Você foi aprovado!!")
}
```

### Se-senao

Se a condição anterior for falsa, executa um novo conjunto de comandos.

exemplo:

```jsx
se(media>=7){
				escreva("Parabéns você foi aprovado!!")
}
senao{
				escreva("Infelizmente você foi reporvado.")
}
```

exemplo utilizando se-senao adicionado no código anterior:

```jsx
programa
{
	
	funcao inicio()
	{
		real janeiro, fevereiro, marco, abril, total, media
		cadeia vendedor

		escreva("Digite o nome do vendedor:")
		leia(vendedor)
		escreva("O seu nome é: " + vendedor)
		
		escreva("\nDigite o valor da venda de janeiro: ")
		leia(janeiro)
		escreva("Digite o valor da venda de fevereiro: ")
		leia(fevereiro)
		escreva("Digite o valor da venda de março: ")
		leia(marco)
		escreva("Digite o valor da venda de abril: ")
		leia(abril)

		total = (janeiro+fevereiro+marco+abril)
		media = (janeiro+fevereiro+marco+abril)/4
		escreva("A total das vendas do vendedor " + vendedor + " é: " + total + " e a média das vendas é: " + media)

		se(media>=500) {
			escreva("\n" + "Boa média mensal!")
		}
		senao {
			escreva("\n" + "Infelizmente esse mês foi fraco.")
			}
		
	}
}
```

### Desvio condicional Caso

Utilizado para guardar várias opções de uma escolha.

```jsx
programa
{
	
	funcao inicio()
	{
		escreva("1 - abrir Netflix 2 - abrir Prime 3 - abrir HBO 4 - Sair")
		inteiro menu = 0
		escreva("\n" + "Qual a sua opção? ")
		leia(menu)

		escolha(menu)
		{
			caso 1:
			escreva("Abrindo Netflix.")
			pare

			caso 2:
			escreva("Abrindo Prime.")
			pare

			caso 3:
			escreva("Abrindo HBO.")
			pare

			caso 4:
			escreva("Saindo.")
			pare

			caso contrario:
			escreva("Escolha uma das opções.")
		}
		
	}
}
```

### Laços de repetição no Portugol

Utilização da variável "faca"(faça) e enquanto.

```jsx
programa
{
	
	funcao inicio()
	{
		inteiro contador, limite, resultado, numero
		escreva("\n" + "Para qual número você quer a tabuada?")
		leia(numero)
		
		contador = 0
		limite = 50

		faca{
			resultado = numero* contador		
			escreva(numero + " x " + contador + " = " + resultado + "\n")
			contador ++
			
		}enquanto(contador<=limite)
	}
}
```

### Matrizes e Vetores

o que é?

Matriz é uma coleção de variáveis do mesmo tipo(não pode ter uma variável do tipo "cadeia" ou do tipo "caracteres" ao mesmo tempo), são acessíveis com um nome e armazenados na memória. Pode ter linhas e colunas.

Os vetores são acessados individualmente através de um índice. São matrizes de uma só dimensão, só colunas, por exemplo.

```jsx
programa
{
	
	funcao inicio()
	{
		inteiro contador = 0
		cadeia pessoa[][] = {{"João", "São Paulo", "(11)9999-5241"},{"Maria", "Ribeirão Preto","(16)9999-8596"},{"Ana","Manaus","(92)9999-8574"}}

		faca{
			escreva("Pessoa: " + pessoa[contador][0] + " Local: " + pessoa[contador][1] + " Tel: " + pessoa[contador][2] + "\n")
			contador++
			
		}enquanto(contador<=2)
	}
}
```

A chaves fechadas sem número dentro não importam, o programa já reconhece a quantidade que tem nelas considerando o tanto de informação que você coloca dentro.

A primeira chave é a coluna e a segunda é a linha. Então por exemplo, João e São Paulo seriam "[0][1]" para fazer o programa escrever na tela.