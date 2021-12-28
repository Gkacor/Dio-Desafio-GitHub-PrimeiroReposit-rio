# SQL Server

Created: December 22, 2021 7:04 PM
Data Inicial: 27/12/2021
Programação: Programação
Reviewed: No

# SQL Server

o que é?

Uma forma de guardar informações para o futuro. Aramazenamento de dados de clientes, por exemplo. Banco de dados.

### SGBD

São softwares que padronizam banco de dados. Uma interface padronizada para o armazenamento de dados. 

Tipos:

Relacionais(para sistemas que precisam de uma maior confiança dos dados, controle de estoque por exemplo.)

- SQL Server
- Oracle
- MySQL

NoSQL(Armazenam grande quantidade de dados como vídeos e etc, possibilita deletar dados mais facilmente.)

- MongoDB
- Neo4j
- Firebase

### Bancos Relacionais

Cada tabela vai ter um tipo. Tem estrutura rígida, então só pode ter um tipo de informação. 

Ex: char, varchar, bit, int, bigint

null - Aceita nulos, notnull - não aceita nulos.

float - “flutuante”, aceita casas decimais.

Exemplo de código:

```sql
use ecommerce
select * from clientes

select TipoPessoa, Nome from clientes where TipoPessoa = 'J'

update clientes
set Codigo = 7,
	Nome = 'José'
where TipoPessoa = 'J'

delete
from clientes
where Codigo in(5, 4, 3, 2)

select * from Produto 

insert Produto values(1, 'Caneca', 'Caneca Azul', 1.5)
insert Produto values(2, 'Caderno', 'Caderno Materias', 21.5)

select * from Pedido
insert Pedido values(1, getdate(), 0, 3, 7)

select * from PedidoItem

insert PedidoItem values(1, 1, 1.5,2 )
```

“*” Seleciona tudo da tabela.

### Chave primária e estrangeira

o que é?

Chave primária: Uma forma de identificar um registro, uma chave única. Ex: cpf de um cliente.

Chave estrangeira: Faz a relação de uma tabela com outra. Sempre será uma cópia de uma chave primária.