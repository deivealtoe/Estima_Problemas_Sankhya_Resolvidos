### Problema: <i>Itens da nota/pedido com sequência errada</i>

Para corrigir esse problema, <b>tente primeiro</b> alterar o campo SEQUENCIA da tabela TGFITE.

Caso dê erro de chave estrangeira na tabela TGFDIN, é preciso:
 - Exportar os registros da tabela TGFDIN como inserção
 - Apagar os registros necessários da TGFDIN
 - Alterar a sequência dos itens que for preciso na TGFITE
 - Alterar no arquivo de INSERT gerado anteriormente de acordo com que foi alterado na sequência da tabela TGFITE
 - Verificar a nova sequência e executar os inserts necessários
