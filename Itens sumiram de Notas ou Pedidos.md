### Problema: <i>Itens de uma Nota ou de um Pedido sumiram</i>

Para resolver esse problema, é preciso verificar se os itens dessa nota/pedido está na na tabela TGFITE_EXC

Caso esteja, é necessário
 - Exportar no modo INSERT os dados dos itens contidos na tabela TGFITE_EXC
 - Tratar os dados, deixar apenas os que serão inseridos na outra tabela
 - Inserir na TGFITE os itens/dados tratos
 - Excluir os itens da TGFITE_EXC

