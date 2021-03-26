# Gvinci : Inserindo tabelas auxiliares

Ao utilizarmos um controle **Grid**, por exemplo, podemos precisar de tabelas auxiliares que irão fornecer os dados que serão usados durante o processamento.

Para inserir tabelas auxiliares para o Grid, utilize a propriedade **AuxiliarTables**, em destaque na figura abaixo:

![](http://www.gvinci.com.br/manual/auxiliartbgv5.zoom73.png)

Ao clicar no botão ![](http://www.gvinci.com.br/manual/extensor-botao.png) da propriedade **AuxiliarTables**, a figura abaixo aparece:

![](http://www.gvinci.com.br/manual/auxiliartb2gv5.zoom81.png)

Siga as instruções abaixo para inserir uma tabela auxiliar para o **Grid**.

**1.** Clique sobre o botão ![](http://www.gvinci.com.br/manual/adicion1gv5.png);

**2**. Selecione a tabela desejada a partir da lista **Tabela**;

O apelido da tabela aparecerá automaticamente. Este apelido foi definido durante a definição da tabela no painel Banco de dados.

**3.** Na aba "Definição", marque a opção "Forçar relacionamento";

![](http://www.gvinci.com.br/manual/forcarelacionamento.png)

**4.** Selecione um dos índices para a tabela escolhida, a partir da lista **Índice**;

**5.** Na seção **Relacionamentos**, clique no botão ![](http://www.gvinci.com.br/manual/adicionar.png) para escolher um campo para unir a tabela básica à nova tabela auxiliar adicionada, a partir da lista apresentada.

![](http://www.gvinci.com.br/manual/relacionartabelasaux.png)

A janela **Fórmula** será exibida.

![](http://www.gvinci.com.br/manual/tbclientes-tbprod.png)

**6.** Clique no campo que deseja escolher para o relacionamento e em seguida, clique em ![](http://www.gvinci.com.br/manual/adicionar.png) para incluir o campo na expressão.

O botão ![](http://www.gvinci.com.br/manual/code-bt.png) pode ser usado para inserção manual de código CSharp.

**7.** Clique em ![](http://www.gvinci.com.br/manual/ok-bt-2.jpg).

A opção **Criticar** pode ser marcada caso o relacionamento seja forçado \(quando a opção **Forçar relacionamento** estiver marcada\). Neste caso, o **Gvinci** criará rotina na aplicação para apresentar a mensagem definida no campo **Mensagem crítica**, caso haja algum erro na realização do relacionamento durante a execução.

![](http://www.gvinci.com.br/manual/criticargv.png)

Caso esta tabela auxiliar esteja sendo aberta como alvo de um lançamento, este lançamento só será executado após a inclusão do registro na tabela básica \(origem do lançamento\) razão pela qual deve-se ter um cuidado especial com a opção **Criticar**, pois ela será executada antes que o lançamento seja efetivado. Na maioria dos casos, as tabelas auxiliares que são alvos de lançamentos devem estar com esta opção desmarcada.

A opção **Utilizar todos os campos \(SELECT \*\)** deve ser usada para selecionar todos os campos da tabela. A expressão SELECT \* serve para selecionar todos, visto que o caractere coringa \* significa "todos". Se não marcar esta opção, você poderá então definir quais os campos farão parte do relacionamento.

Vídeo explicativo disponível pelo [Canal da SSI no youtube](https://www.youtube.com/user/SSITecnologia):

[08.1 - Tabelas auxiliares em páginas de dados](https://www.youtube.com/watch?v=agG4k3aG6dY)

