# Índices

A criação de índices não é obrigatória. Às vezes, os índices são criados para que haja integridade e relacionamento nas tabelas ou, ainda, para proporcionar uma ordem de navegação dentro da tabela correspondente, bem como pesquisas rápidas aos seus registros. No entanto, o usuário da aplicação final poderá estabelecer seu próprio critério de ordenação de registros, independente dos índices criados no projeto. Existe, ainda, o caso especial da tabela do tipo parâmetro, que não pode conter índice definido, uma vez que tabelas desse tipo contêm somente um registro.

![](http://www.gvinci.com.br/manual/indprod1gv5.zoom80.png)

        Índices da tabela TB\_PRODUTOS do exemplo Controle de Estoque. 

  
Um índice sem chave \(NK=Non-key\) e um chave-primária = \(PK=Primary Key\).

![](http://www.gvinci.com.br/manual/adicion1gv5.png)        Permite incluir um novo índice.

![](http://www.gvinci.com.br/manual/excluibtgv5.png)        Permite excluir o índice selecionado.

**Nome:** Insira o nome desejado para o índice. O **Gvinci** sugere o nome iniciando com PK\_+nomedatabela.

**Apelido:** Permite inserir um apelido para o índice. O apelido sugerido inicia com PK\_+nomedatabela.

**Título:** Insira o título do índice. O Gvinci sugere o título iniciando com PK\_+nomedatabela. Os índices são utilizados em relacionamento entre tabelas e muito úteis quando se trata de localização de registros.

**Descrição:** Coloque aqui a descrição, com explicações sobre o índice.

**Primário:** Esta opção deverá ser marcada quando o índice possuir chave primária.

Em uma tabela, somente um índice primário poderá ser definido mas não é obrigatório. Porém, se um índice primário for definido, este, obrigatoriamente, deverá ser único. O **Gvinci** marca automaticamente a opção **Unico** quando a opção **Primário** é marcada. Quando um índice com chave primária é adicionado, o **Gvinci** adiciona as iniciais PK\_ \(Primary Key ou chave primária \) ao nome do índice.

**Unico:** Esta opção deverá ser marcada se a chave do índice em definição tem este tipo de atributo. Diversos índices  podem ser definidos como únicos para uma tabela.

**Cluster:** Esta opção já vem marcada como padrão.

Em **SQL Server,** qualquer tabela pode ter um índice cluster e um ou vários índices não cluster. Os dados de uma tabela que possui índice cluster são organizados como uma lista, sendo ordenados pela coluna que possui o índice cluster. Em tabelas que não possuem índice cluster os dados não são organizados.

Em Oracle, quando inserimos um índice cluster as tuplas \(sequências de elementos\) são organizadas de acordo com a chave definida para o índice e caso o índice seja não cluster, a chave do índice não vai influenciar no armazenamento das tuplas.

**FillFactor:** O FillFactor varia de 0% a 100%, e tem a tarefa de alocar espaços em branco em cada página para reservar espaço para a inserção de novas linhas. O valor padrão de porcentagem utilizado no **Gvinci** é 90.

**Campos:** Ao definir o índice, é necessário marcar as opções **Primário** ou **Único** e em seguida determinar qual serão os campos que receberão os índices.

![](http://www.gvinci.com.br/manual/ind2gv5.png)

![](http://www.gvinci.com.br/manual/adicion1gv5.png)        Acrescenta um campo ao índice.

![](http://www.gvinci.com.br/manual/excluibtgv5.png)        Apaga o campo selecionado, no índice.

![](http://www.gvinci.com.br/manual/moveabaixobtgv5.png)        Move o campo selecionado para baixo.

![](http://www.gvinci.com.br/manual/moveacimabtgv5.png)        Move o campo selecionado para cima.

Clique duas vezes no primeiro campo e aparecerá uma seta Drop-Down: ![](http://www.gvinci.com.br/manual/dropdown.png)

**Campo:** Clique na seta Drop-Down para exibir a lista de campos existentes.

**Decrescente:** Marque esta caixa se quiser que o índice fique em ordem decrescente, após acrescentar um campo.

**Abreviações dos índices:**

**PK = Primary Key :** Chave primária.

**FK = Foreign Key:** Chave estrangeira.

**NK = Non-Key :** Indica que o campo não funciona como chave.

