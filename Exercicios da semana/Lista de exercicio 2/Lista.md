Faça um diagrama ER para um sistema de empréstimos de livros de uma biblioteca, a
partir das seguintes informações:
 A biblioteca possui um cadastro de livros e, para cada livro, são necessárias as
seguintes informações: código ISBN (código internacional de livros, único no
sistema), título, nome(s) do(s) autor(es), edição, ano de publicação e editora (CNPJ,
nome, endereço, site e e-mail). A biblioteca possui vários exemplares de cada livro
disponíveis para empréstimo. Cada exemplar possui um número de identificação,
que é único no sistema, uma localização dentro da biblioteca, o tipo de empréstimo
(uso exclusivo na biblioteca, uso fora da biblioteca) e uma situação (emprestado,
disponível).
 Para cada exemplar de livro que for emprestado pela biblioteca, devem ser
armazenadas as seguintes informações: os dados do exemplar, os dados do usuário
que toma o livro emprestado (número de matrícula, nome, endereço e telefones), a
data do empréstimo, a data limite para devolução e a data real de devolução, quando
o livro for devolvido.
2. Faça um diagrama ER para um sistema de controle bancário a partir das seguintes
informações:
 Cada banco tem um nome e um código de identificação no sistema bancário. Ambos
são únicos no sistema;
 Cada banco possui um conjunto de agências, onde os clientes abrem suas contas.
Cada agência possui um código de identificação, que é único dentro de cada banco
(agências de bancos diferentes podem ter o mesmo código), um nome e um
endereço (logradouro, no
, complemento, bairro, cidade, cep, estado);
 Dos clientes são necessárias as seguintes informações: cpf, nome e endereço
(logradouro, no
, complemento, bairro, cidade, cep, estado). Considere que o cpf
identifica unicamente cada cliente;
 As contas são somente do tipo conta-corrente e possuem um número de
identificação, que é único dentro do sistema, e um saldo. As contas podem ser
individuais (de um único cliente) ou conjuntas (pertencerem a mais de um cliente).
Um cliente pode ter mais de uma conta em uma mesma agência. É necessário saber
também a data em que cada conta foi aberta. As contas possuem movimentações (ou
transações) para as quais deve-se manter um controle histórico. Cada movimentação
possui um número de identificação, que é único dentro do sistema, a data e o
horário em que ela ocorreu, o tipo de movimentação (débito ou crédito), a descrição
da movimentação e o valor movimentado.
3. Faça um diagrama ER para um sistema de controle de estoque, compra e venda de uma
loja de produtos de informática, a partir das seguintes informações:
 A loja possui um cadastro de produtos. Cada produto possui um código (único no
sistema), uma descrição e um preço de venda. Também é necessário saber-se a
quantidade disponível em estoque de cada produto;
 A loja vende produtos para seus clientes através de pedidos, que do ponto de vista
da loja são os pedidos de venda. Em cada pedido de venda consta um número de
identificação do pedido, a data do pedido, os dados do cliente (cpf, nome,
endereço (logradouro, no
, complemento, bairro, cidade, cep, estado) e telefones de
contato) e a relação de produtos pedidos, incluindo o preço de venda e a
quantidade pedida. Cada pedido de venda também possui uma situação indicando
se ele está pendente, já foi entregue ou foi cancelado.
 A loja paga mensalmente os vendedores por meio de comissão de venda. Cada
vendedor possui um número de registro na loja, um nome e uma data de admissão.
Cada vendedor recebe um percentual sobre as vendas que ele efetua. Esse
percentual varia de vendedor para vendedor dependendo do tempo de trabalho na
loja. O percentual começa com 0,5% e aumenta em 0,5% a cada seis meses, até o
limite de 3%.
 Para comprar um produto, a loja faz orçamentos com diversos fornecedores. Em
cada orçamento consta os dados do fornecedor (cnpj, razão social, nome fantasia,
endereço (logradouro, no
, complemento, bairro, cidade, cep, estado) e telefones de
contato), os dados do produto cotado, o preço de compra, a data de cotação, a data
de validade do preço cotado e o prazo de entrega. Com base nos orçamentos, são
feitos pedidos de compra para os fornecedores que oferecem as melhores
condições. Em cada pedido de compra consta um número de identificação do
pedido, a data do pedido, os dados do fornecedor e a relação de produtos pedidos,
incluindo o preço e a quantidade pedida. Cada pedido possui também uma situação
indicando se ele está pendente, já foi entregue ou foi cancelado. Não é necessário
relacionar os pedidos de compra aos orçamentos;
4. Altere o diagrama do exercício anterior, criando uma hierarquia para os tipos de
entidades Fornecedor, Cliente e Vendedor. Considere que os fornecedores da loja são
sempre pessoas jurídicas (empresas), os clientes podem ser pessoas jurídicas ou pessoas
físicas e os vendedores são sempre pessoa física. Nada impede que fornecedores e
vendedores sejam também clientes da loja. Considere, ainda, que vendedores também
possuem os atributos endereço e telefones, como definidos para clientes e fornecedores.
5. Faça um diagrama ER para um sistema de um museu de artes, a partir das seguintes
informações:
 O museu tem uma coleção de obras de arte. Cada obra de arte tem um número de
identificação, um artista (se conhecido), um ano (quando a obra foi criada, se
conhecido), um título e uma descrição. As obras de arte são categorizadas como
pintura, escultura, estátua e outros (obras que não são dos três tipos anteriores).
Uma pintura tem um tipo (óleo, água etc), um material no qual foi desenhada
(papel, madeira, canvas etc) e um estilo (moderna, abstrata etc). Uma escultura
tem o material em que foi criada (madeira, pedra etc), a altura, o peso e o estilo.
Uma estátua tem um estilo. Uma obra de arte na categoria outros também tem um
um estilo;
 As obras de arte também são categorizados como coleção permanente que são de
propriedade do museu (neste caso guarda-se informações sobre data de aquisição,
se a obra está em exposição ou está guardada e o custo da obra) ou como
emprestados (que guarda informações sobre a coleção a que ela pertence, a data de
empréstimo e a data de devolução);
 As obras de arte também guardam informações sobre o seu país/cultura de origem
(italiana, egípcia etc) e a época em que foram criadas (renascimento, modernismo
etc);
 O museu mantém informações sobre os artistas (se conhecidos): nome, data de
nascimento, data de falecimento (se não está vivo), país de origem, época,
principal estilo e descrição. O nome é tido como único;
 Ocorrem diferentes exibições, cada uma tem nome (único), data de início, data de
término e uma relação de todas as obras de arte que foram mostradas durante a
exibição;
 Das coleções com que o museu interage também são mantidas informações sobre
nome (único), tipo (museu, pessoal etc), descrição, endereço, telefone e pessoa de
contato.
6. Faça os exercícios do livro texto (Elmasri & Navathe, 6a
 edição), Capítulo 7.
7. Descreva, em forma de texto, o minimundo representado pelo diagrama EER da Figura
8.8 do livro texto (Elmasri & Navathe, 6a
 edição), Capítulo 8.
8. Descreva, em forma de texto, o minimundo representado pelo diagrama EER da Figura
8.9 do livro texto (Elmasri & Navathe, 6a
 edição), Capítulo 8.
9. Faça os exercícios do livro texto (Elmasri & Navathe, 6a
 edição), Capítulo 8.