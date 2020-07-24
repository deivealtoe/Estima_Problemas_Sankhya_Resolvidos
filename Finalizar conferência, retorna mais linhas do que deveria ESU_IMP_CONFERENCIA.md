### Erro: Ao tentar finalizar conferência, é exibido o erro "a extração exata retorna mais do que o número solicitado de linhas"

<p>Isso acontece pois a consulta deveria retornar apenas um registro, mas retona dois ou mais</p>
<p>Nesse erro específico da imagem, o produto 803 tinha lote (controle) e código de barras iguais, então retorna duas linhas na consulta, ocasionando o erro</p>
<p>Isso aconteceu pois o pedido inicial foi digitado de maneira errada, foi inserido no pedido duas vezes</p>
<p>O pedido foi carregado errado e tivemos que ligar para o cliente e ver se ele vai querer mesmo ou fazer alguma devolução</p>

```
select ite.CODPROD, pro.CODVOL, pro.TIPCONTEST, ite.CONTROLE
from TGFPRO pro
join TGFITE ite on ite.CODPROD=pro.CODPROD
where pro.REFERENCIA = 'Cód. de Barra do prod aqui'
and ite.NUNOTA = 'Nro. Único da Nota aqui'
and ite.CONTROLE = 'LOTE do produto (CONTROLE) AQUI';
```

<img src="https://raw.githubusercontent.com/deivealtoe/problemas_sankhya_resolvidos/master/_src/_images/finalizar_conferencia_erro.png">
