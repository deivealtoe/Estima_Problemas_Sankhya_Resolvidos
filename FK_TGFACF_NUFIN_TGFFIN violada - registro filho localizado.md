#### Problema: <i>FK_TGFACF_NUFIN_TGFFIN violada - registro filho localizado</i>

<p>Esse erro quer dizer que existe um título do financeiro na tebela TGFACF</p>
<p>Para procurar esse registro podemos usar a consulta</p>

```
SELECT *
FROM tgfacf
WHERE nufin = '???'
```

<img src="https://raw.githubusercontent.com/deivealtoe/problemas_sankhya_resolvidos/master/_src/_images/FK_TGFACF_NUFIN_TGFFIN.png">
