# Tipos de Consultas

Na definição dos campos de uma consulta, no painel **Banco de Dados**, há o botão ![](http://www.gvinci.com.br/manual/constrbtgv5.png), que chama a janela **Fórmula**, onde podemos estipular condições de filtragem:

![](http://www.gvinci.com.br/manual/constrconsgv5.zoom100.png)

Na aba **"Ligações e seleções"** da janela **Construtor de consulta**, há uma lista de quatro tipos de **Join** disponíveis, na opção **Tipo de ligação**.

Nesta aba, podemos definir como extrair informações de várias tabelas ao mesmo tempo.

![](http://www.gvinci.com.br/manual/tipoligacgv5.zoom100.png)

**INNER:** Tipo de relacionamento que seleciona os registros combinados em ambas as tabelas, isto é, para que um registro seja aceito como resultado do relacionamento, o campo que faz a ligação entre as duas tabelas deve satisfazer as condições em ambas.

Utilizamos o Inner Join quando é preciso montar um conjunto de registros \(recordset\) lendo dados de mais de uma tabela. É uma forma de unir tabelas, e para isso é preciso que haja uma relação entre elas, isto é, um campo de ligação. É importante ressaltar que estes campos não precisam ter o mesmo nome, porém devem ser do mesmo tipo.

**LEFT:** Tipo de relacionamento que inicia a análise da estrutura de uma tabela da direita para uma tabela da esquerda, no banco de dados.

**RIGHT:** Tipo de relacionamento que inicia a análise da estrutura de uma tabela da esquerda para uma tabela da direita, no banco de dados.

Observe a ilustração abaixo:

![](http://www.gvinci.com.br/manual/left-right-join.png)

**FULL:** Este tipo de relacionamento, também chamado de **FULL OUTER JOIN,** é usado para selecionar todos os registros de todas as tabelas envolvidas no relacionamento.

