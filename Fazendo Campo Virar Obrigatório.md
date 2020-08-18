#### Fazendo um campo virar obrigatório

<p>A forma mais comum é pela tela Dicionário de Dados, mas caso a opção de alterar os atributos do campo esteja desabilitada, é necessário fazer pelo banco de dados.</p>

<p>Para alterar o campo pelo banco de dados, basta executar o comando a seguir, por exemplo:</p>

```
ALTER TABLE tgfpro MODIFY (codformprec NOT NULL);
```

#### Mas antes de executar esse comando para alterar o campo, certifique-se de que não há nenhum registro como nulo no campo alterado

#### Após mudar o campo para NOT NULL, tentei alterar um registro dos produtos, e foi me apresentado o seguinte erro, indicando que está funcionando.
<img src="https://raw.githubusercontent.com/deivealtoe/problemas_sankhya_resolvidos/master/_src/_images/fazendo_campo_virar_not_null.png">
