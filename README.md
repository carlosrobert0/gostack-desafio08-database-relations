# gostack-desafio08-database-relations
Desenvolver uma nova aplicacao Node.js junto ao TypeScript, incluindo banco de  dados com TypeORM e relacionamentos ManyToMany!

🚀 Sobre o desafio

Nesse desafio, você vai estar criando uma nova aplicação para aprender novas coisas e treinar o que você aprendeu até agora no Node.js junto ao TypeScript, incluindo o uso de banco de dados com o TypeORM, e relacionamentos ManyToMany!

Essa será uma aplicação que deve permitir a criação de clientes, produtos e pedidos, onde o cliente pode gerar novos pedidos de compra de certos produtos, como um pequeno e-commerce.

Rotas da aplicação

    POST /customers: A rota deve receber name e email dentro do corpo da requisição, 
    sendo o name o nome do cliente a ser cadastrado. Ao cadastrar um novo cliente, 
    ele deve ser armazenado dentro do seu banco de dados e deve ser retornado o cliente criado. 
    Ao cadastrar no banco de dados, na tabela customers deverá possuir os campos name, email, created_at, updated_at.

    POST /products: Essa rota deve receber name, price e quantity dentro do corpo da requisição,
    sendo o name o nome do produto a ser cadastrado, price o valor unitário e quantity a quantidade 
    existente em estoque do produto. Com esses dados devem ser criados no banco de dados um novo produto 
    com os seguintes campos: name, price, quantity, created_at, updated_at.

    POST /orders/: Nessa rota você deve receber no corpo da requisição o customer_id e um array de products,
    contendo o id e a quantity que você deseja adicionar a um novo pedido. 
    Aqui você deve cadastrar na tabela order um novo pedido, que estará relacionado ao customer_id informado, 
    created_at e updated_at . Já na tabela orders_products, você deve armazenar o product_id, order_id, price e quantity, created_at e updated_at.
