# Exemplo de Ecommerce com Hiberate e Annotations

Este projeto servirá como base para podermos explorar as quatros situações classicas que existem em relacionamentos entre tabelas em um banco de dados e como isso se aplica ao Hibernate.

Relacionamentos utilizados:

uma-para-um           @OneToOne
um-para-muitos        @OneToMany
muitos-para-um        @ManyToOne
muitos-para-muitos    @ManyToMany

Ao executar o projeto após a criação do banco de dados com o nome comercio e o mapeamento das classes, o Diagrama de Dados deve ficar assim:

![image](https://user-images.githubusercontent.com/10384482/166235996-d695a476-fd69-4c5a-8e96-3be900dfb9d8.png)

Analisando o modelo de dados temos as seguintes regras de negócio:

Um produto sempre pertence a uma categoria.
Um produto pode constrar como item de um ou vários pedidos.
Um item do pedido representa uma tabela associativa entre produtos e pedidos.
Um pedido tem associado a ele um cliente e um empregado.
Um empregado está associado a um pedido além de estar subordinado a outro empregado.
Um cliente pode ter um ouvarios pedidos.
Um cliente tem um único endereço.
Um endereço pertence a um único cliente
