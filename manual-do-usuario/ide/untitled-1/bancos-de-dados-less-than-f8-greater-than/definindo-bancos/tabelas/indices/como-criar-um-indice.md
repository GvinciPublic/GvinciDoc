# Como criar um índice

Após ter criado um banco e suas tabelas, você poderá escolher campos das tabelas para inserir índices.

Ao criar um índice com chave primária \(Primary Key\), o **Gvinci** sugere o nome do índice, iniciando com PK+NOMEDATABELA, ou seja, Primary Key \(Chave primária\) seguido pelo nome da tabela.

Quando um novo índice é adicionado e que não contenha chave, pois só pode haver uma chave em cada tabela, o Gvinci adiciona automaticamente as iniciais NK\_ - que quer dizer "Not a Key", ou seja: que o índice não é uma chave.

É importante lembrar que, antes de se criar um índice, é necessário ter definido campos para a tabela e escolher um campo específico que será o índice da tabela.

Para criar um índice, siga os seguintes passos:

**1.** Com o botão direito do mouse, clique sobre **"Índices";**

![](http://www.gvinci.com.br/manual/novoind2gv5.zoom80.png)

**2.** Escolha **"Novo Índice";**

**3.** O nome sugerido pelo **Gvinci** começará com PK+NOMEDATABELA . Caso queira alterar, preencha os campos **"Nome"**, **"Apelido"**, **"Título"** e **"Descrição"**;

**4.** Escolha se o índice receberá chave primária \(campo não pode se repetir\). Será automaticamente marcado como único.

**5.** Desmarque a opção **"Cluster"**, se achar necessário. Como padrão, esta opção já vem marcada.

A porcentagem de FillFactor não precisa ser alterada. O padrão é 90. Essa porcentagem determina o espaço que poderá ser usado no banco de dados para inclusão de novos registros sem que a ordenação dos registros seja afetada. 10% será reservado para esse espaço, quando o FillFactor estiver com a porcentagem 90.

**6.** Clique no botão "Adicionar Campos" ![](http://www.gvinci.com.br/manual/adicion1gv5.png);

**7.** Clique duas vezes no primeiro campo e aparecerá uma seta **Drop-Down:** ![](http://www.gvinci.com.br/manual/setadropvg5.png).

**IMPORTANTE:** Somente os campos que tiverem a opção **Permitir nulo DESMARCADA** vão aparecer na lista. Se esta opção do campo estiver marcada, não será possível criar um índice com esse campo, pois um índice não pode se basear em um campo que pode ser vazio.

![](http://www.gvinci.com.br/manual/permitnulo1gv5.zoom100.png)

**8.** Clique na seta drop-down e escolha o campo que receberá o índice;

**9.** Se preferir o índice em ordem decrescente, marque a opção correspondente;

**10.** Após ter inserido mais de um índice, você pode usar os botões acima ![](http://www.gvinci.com.br/manual/moveacimabtgv5.png) e abaixo ![](http://www.gvinci.com.br/manual/moveabaixobtgv5.png) para mover os campos.

